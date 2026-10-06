<!-- ELUCENIA technical documentation · imc · zh · no clinical/professional/rights approval -->

# 体重指数（BMI）

[条件、来源与许可](https://elucenia.org/zh/tools/imc)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 体重

`peso`

kg · 范围: 20–350

### 身高

`altura`

cm · 范围: 100–230

### 适用人群

`pop`

- `g` — 一般
- `a` — 亚洲

## 方法版本

WHO/TRS 894/2000：kg/m²，成人；亚洲行动界值23/27.5，WHO 2004

## 已记录的公式

BMI=体重（kg）÷身高²（m²）。

WHO（2004）为亚洲人群增加公共卫生行动界值：23 kg/m²（风险增加）和27.5 kg/m²（高风险）。

## 限制与适用人群

体质指数（BMI）关联体重与身高，但不直接测量体脂，也不区分脂肪、肌肉和骨骼。儿科解释取决于年龄、性别及参考曲线；将成人分类应用于儿童的计算值不能证明适用性。CDC区分2–19岁儿童及青少年与20岁及以上成人；该界限属于CDC指导，不自动替代此处呈现的分类版本。结果须结合其他临床数据解释。

## 参考文献

- [World Health Organization. Obesity: preventing and managing the global epidemic. Report of a WHO consultation. WHO Technical Report Series 894, 2000.](https://pubmed.ncbi.nlm.nih.gov/11234459/)

- [WHO Expert Consultation. Appropriate body-mass index for Asian populations and its implications for policy and intervention strategies. Lancet, 2004.](https://doi.org/10.1016/S0140-6736(03)15268-3)

- [https://www.cdc.gov/bmi/faq/](https://www.cdc.gov/bmi/faq/)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

正常体重（体重适宜）（WHO）

| 结果详情 | |
| --- | --- |
| BMI为18.5至24.9的体重范围 | 56.7 至 76.3 kg |


### 2

超重（前期肥胖）（WHO）

| 结果详情 | |
| --- | --- |
| BMI为18.5至24.9的体重范围 | 74.0 至 99.6 kg |


### 3

I 级肥胖（WHO）

| 结果详情 | |
| --- | --- |
| BMI为18.5至24.9的体重范围 | 53.5 至 72.0 kg |


### 4

正常体重（适当体重）（WHO）；亚洲人风险增加

| 结果详情 | |
| --- | --- |
| BMI为18.5至24.9的体重范围 | 53.5 至 72.0 kg |
| 亚洲人行动点（WHO 2004） | 风险增加 |

