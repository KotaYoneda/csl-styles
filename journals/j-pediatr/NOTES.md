# The Journal of Pediatrics

- 投稿規定: https://www.sciencedirect.com/journal/the-journal-of-pediatrics/publish/guide-for-authors
- 規定確認日: 2026-11-13
- 参照した掲載論文: Brunsch CL, et al. J Pediatr 2026;297:115222.

## 方針
- 実際の掲載論文の体裁（上付き番号）に合わせる
- 理由: 投稿規定には次の2つの記述があり、角括弧での投稿は必須ではない
  - 「Reference format」の節: 投稿時の書式は自由（一貫していれば可）。採択後の校正段階で出版社がジャーナルの書式に直す
  - 「Reference style」の節: 角括弧 [1] の形式が書かれているが、実際の掲載論文は上付き番号で、この記述と一致しない（Elsevier共通の定型文と思われる）

## 掲載形式の要点
- 本文中は上付き番号（例: dysfunction.2,3 / 7-10）、出現順
- 文献リストは「1.」形式
- 著者7名以上は最初の6名 + et al.
- 雑誌名は略記、号は省略: Clin Perinatol 2016;43:423-38.
- 末尾ページは短縮形、DOIは https://doi.org/ 形式で後ろにピリオドなし
- 章: In: Rajendram R, Preedy VR, Patel VB, eds. 書名. Cham: 出版社; 2023. p. 199-222.
- 書籍: 著者. 書名. 地名: 出版社; 年.

## 公式版
- 公式のJ Pediatrスタイルは elsevier-vancouver を参照する dependent スタイル（2017年更新）
- official.csl は親の elsevier-vancouver.csl（角括弧形式で、掲載形式とは異なる）
- 取得元コミット: b5a5d009681b851163f051357a00080a6ec2e300
- 取得日: 2026-11-13

## 公式版からの変更点
- 本文中を上付き番号に、文献リストの番号を「1.」に変更
- DOIの後のピリオドを削除
- 章の編者表記を eds に
- 論文番号フォールバック（page が空なら number）を追加
- 掲載論文の文献（雑誌論文・7名以上の著者・論文番号・"33-40.e2"・章・書籍）で一致を確認

## 注意
- 上付き番号はピリオドの後に置く（Word上の挿入位置で決まる）
- Pandocでは番号範囲がエンダッシュ（7–10）になる。Paperpile/Wordではハイフンになるはず
- ウェブページの形式は掲載論文に例がなく未確認
