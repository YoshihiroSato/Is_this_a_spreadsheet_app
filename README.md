# これはスプレッドシートですか？ / Is This a Spreadsheet App?

**動作デモ / Live Demo:**
[https://yoshihirosato.github.io/Is_this_a_spreadsheet_app/SPRv3.html](https://yoshihirosato.github.io/Is_this_a_spreadsheet_app/SPRv3.html)

---

## 概要

このアプリケーションはClaude（Anthropic）との対話によって生成されました。
「Excelとは何か」を問うEuSpRIG 2026発表のデモとして使用しています。
[https://eusprig.org/about/about-eusprig/]
(The European Spreadsheet Productivity & Risks Interest Group – EuSPRIG –)

スプレッドシートの最小定義を探る実験です。
バグがあります。不完全です。それが目的です。

## できること

- セルが縦横に並んでいる
- セルに値を入力できる
- セルにセル参照を含んだ計算式を手入力で入れられる
- 範囲選択するとその集計値（合計・平均・最大・最小・個数）がステータスバーに表示される
- 1セルの値や計算式をコピーし1セルに貼り付けでき、セル参照は相対参照として調整される
- SUM・AVERAGE・MAX・MIN・COUNT・IF・ROUND・ABS・SQRT・POWER・MOD関数を扱える
- Ctrl+C / Ctrl+V によるコピー＆ペースト
- 自動再計算
- 文字は左揃え、数値は右揃え
- 数値精度: 15桁（IEEE 754 倍精度、`toPrecision(15)` で表示）

## できないこと

- オートフィル
- 絶対参照（`$A$1` 形式）
- ほとんどの関数
- ファイルを開く・保存する
- CSVデータのダウンロード（ボタンは存在するが機能しない）
- セルの書式設定と表示形式
- フィルター・並べ替え

---

## About

This application was generated through dialogue with Claude (Anthropic).
It serves as a demonstration for a EuSpRIG 2026 presentation exploring the question: *What is Excel?*
[https://eusprig.org/about/about-eusprig/]
(The European Spreadsheet Productivity & Risks Interest Group – EuSPRIG –)

This is an experiment in finding the minimal definition of a spreadsheet.
It has bugs. It is incomplete. That is the point.

## What it can do

- Cells arranged in rows and columns
- Input values into cells
- Enter formulas with cell references manually
- Display aggregates (sum, average, max, min, count) in the status bar when a range is selected
- Copy a single cell value or formula and paste it to another cell, with relative reference adjustment
- Handle SUM, AVERAGE, MAX, MIN, COUNT, IF, ROUND, ABS, SQRT, POWER, MOD functions
- Copy and paste via Ctrl+C / Ctrl+V
- Automatic recalculation
- Text aligned left, numbers aligned right
- Numeric precision: 15 significant digits (IEEE 754 double, displayed via `toPrecision(15)`)

## What it cannot do

- Autofill
- Absolute references (`$A$1` syntax)
- Most functions
- Open or save files
- Download CSV data (button exists but does not work)
- Cell formatting and display formats
- Filter and sort

---

## 研究背景 / Research Context

**EuSpRIG 2026** — University of Greenwich, July 9–10, 2026

Yoshihiro Sato (Independent researcher, Sendai, Japan)

このデモは「Excelに見える境界線はどこか」を問う実験として制作されました。
セルがあり、値が入力でき、セル参照で計算できる——それだけでExcelに見えたとしたら、私たちがExcelに意味づけしてきたものとは何だったのか。

This demo was created as an experiment asking: *where is the boundary of what looks like Excel?*
If cells, value input, and formula references are enough to look like Excel — what exactly have we been attributing meaning to all along?

---

*Generated via Claude (Anthropic) — claude.ai*
*License: MIT*
