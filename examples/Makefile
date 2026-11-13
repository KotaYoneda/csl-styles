# Usage:
#   make JOURNAL=j-pediatr          build with your own CSL
#   make compare JOURNAL=j-pediatr  build with both your CSL and official.csl
#   make clean
#
# Works on both Windows (cmd) and macOS/Linux (sh).

JOURNAL  ?= j-pediatr
DIR      := ../journals/$(JOURNAL)
CSL      := $(DIR)/$(JOURNAL).csl
OFFICIAL := $(DIR)/official.csl
OUT      := out
FORMAT   ?= html

PANDOC := pandoc sample.md --citeproc --standalone

ifeq ($(OS),Windows_NT)
  SHELL       := cmd
  .SHELLFLAGS := /c
  MKDIR_OUT   := if not exist $(OUT) mkdir $(OUT)
  RM_OUT      := if exist $(OUT) rmdir /s /q $(OUT)
else
  MKDIR_OUT   := mkdir -p $(OUT)
  RM_OUT      := rm -rf $(OUT)
endif

.PHONY: all compare clean

all: $(OUT)/$(JOURNAL).$(FORMAT)

$(OUT)/$(JOURNAL).$(FORMAT): sample.md refs.bib $(CSL)
	@$(MKDIR_OUT)
	$(PANDOC) --csl $(CSL) -o $@

compare: all
ifneq ($(wildcard $(OFFICIAL)),)
	$(PANDOC) --csl $(OFFICIAL) -o $(OUT)/$(JOURNAL)-official.$(FORMAT)
else
	@echo official.csl not found: $(OFFICIAL)
endif

clean:
	@$(RM_OUT)
