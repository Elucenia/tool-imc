<!-- ELUCENIA technical documentation · imc · ja · no clinical/professional/rights approval -->

# 体格指数（BMI）

[条件・出典・許諾](https://elucenia.org/ja/tools/imc)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 体重

`peso`

kg · 範囲: 20–350

### 身長

`altura`

cm · 範囲: 100–230

### 対象集団

`pop`

- `g` — 一般
- `a` — アジア

## 方法の版

WHO/TRS 894/2000：kg/m²、成人；アジア人介入基準23/27.5、WHO 2004

## 記載された計算式

BMI=体重（kg）÷身長²（m²）。

WHO（2004）はアジア人集団に公衆衛生上の介入基準値を追加：23 kg/m²（リスク増加）、27.5 kg/m²（高リスク）。

## 限界・対象集団

BMIは体重と身長を関連付けますが、体脂肪を直接測定せず、脂肪、筋肉、骨を区別しません。小児での解釈は年齢、性別、基準曲線に依存します。小児で計算した値に成人の分類を適用しても、その適用可能性が示されるわけではありません。CDCは2–19歳の小児・青少年と20歳以上の成人を区別します。この境界はCDCの指針に属し、ここで示す分類の版を自動的に置き換えるものではありません。結果は他の臨床データと合わせて解釈する必要があります。

## 参考文献

- [World Health Organization. Obesity: preventing and managing the global epidemic. Report of a WHO consultation. WHO Technical Report Series 894, 2000.](https://pubmed.ncbi.nlm.nih.gov/11234459/)

- [WHO Expert Consultation. Appropriate body-mass index for Asian populations and its implications for policy and intervention strategies. Lancet, 2004.](https://doi.org/10.1016/S0140-6736(03)15268-3)

- [https://www.cdc.gov/bmi/faq/](https://www.cdc.gov/bmi/faq/)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

正常体重（適正体重）（WHO）

| 結果の詳細 | |
| --- | --- |
| BMIが18.5～24.9の体重範囲 | 56.7～76.3 kg |


### 2

過体重（前肥満）（WHO）

| 結果の詳細 | |
| --- | --- |
| BMIが18.5～24.9の体重範囲 | 74.0～99.6 kg |


### 3

肥満 1度（WHO）

| 結果の詳細 | |
| --- | --- |
| BMIが18.5～24.9の体重範囲 | 53.5～72.0 kg |


### 4

正常体重（適正体重）（WHO）；アジア人ではリスク増加

| 結果の詳細 | |
| --- | --- |
| BMIが18.5～24.9の体重範囲 | 53.5～72.0 kg |
| アジア人の行動基準値（WHO 2004） | リスク増加 |

