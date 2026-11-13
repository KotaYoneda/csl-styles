---
title: CSLスタイル確認用サンプル
lang: ja-JP
bibliography: refs.bib
link-citations: true
---

# 本文中の引用

## 括弧内引用

和文・単著 [@yamada2021]。和文・2名 [@sato2019]。和文・4名 [@tanaka2022]。

欧文・単著 [@smith2020]。欧文・2名 [@brown2018]。欧文・8名 [@wilson2021]。

## 文中引用（著者名を地の文に出す）

@yamada2021 は〜を示した。@tanaka2022 によれば〜。

@smith2020 reported that ... @wilson2021 replicated ...

## 複数文献の同時引用（並び順・区切り記号の確認）

和文のみ [@yamada2021; @sato2019; @tanaka2022]。

欧文のみ [@smith2020; @brown2018; @wilson2021]。

和欧混在 [@smith2020; @yamada2021; @brown2018; @sato2019]。

## 曖昧さ回避

同一著者・同一年 [@lee2020a; @lee2020b]。

同姓・別人・同年 [@lee2020a; @lee2020c]。

同姓・別人（和文） [@yamada2021; @yamada2018]。

## ページ指定・前置き・後置き

ページ指定 [@nakamura2020, p. 45]、範囲 [@miller2012, pp. 10--12]。

前置きと後置き [例えば, @kobayashi2017, 第3章を参照]。

著者名の省略 中村 [-@nakamura2020] によれば〜。

## 文献タイプ別

書籍 [@nakamura2020; @miller2012]。編著書の章 [@kobayashi2017; @evans2019]。

翻訳書 [@miller2016ja]。学位論文 [@kimura2023]。

論文番号形式 [@garcia2023]。印刷中 [@clark_inpress]。

団体著者 [@mext2024; @who2022]。

## 同一文献の連続引用（ibid. 系スタイルの確認）

最初の引用 [@smith2020]。直後の再引用 [@smith2020]。ページ違いの再引用 [@smith2020, p. 130]。

# 引用文献

::: {#refs}
:::
