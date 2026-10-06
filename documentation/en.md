<!-- ELUCENIA technical documentation · imc · en · no clinical/professional/rights approval -->

# BMI (Body Mass Index)

[conditions, sources and permissions](https://elucenia.org/en/tools/imc)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Weight

`peso`

kg · range: 20–350

### Height

`altura`

cm · range: 100–230

### Population

`pop`

- `g` — General
- `a` — Asian

## Method edition

WHO/TRS 894/2000: kg/m², adults; Asian action points 23/27.5, WHO 2004

## Documented formula

BMI = weight (kg) ÷ height² (m²).

For Asian populations, WHO (2004) added public-health action points: 23 kg/m² (increased risk) and 27.5 kg/m² (high risk).

## Limits and population

BMI relates weight and height but does not directly measure body fat or distinguish fat, muscle and bone. Pediatric interpretation depends on age, sex and reference curves; applying the adult classification to a value calculated in a child does not demonstrate its applicability. CDC distinguishes children and adolescents aged 2–19 years from adults aged 20 years and older; that boundary belongs to CDC guidance and does not automatically replace the classification edition presented here. The result must be interpreted with other clinical data.

## References

- [World Health Organization. Obesity: preventing and managing the global epidemic. Report of a WHO consultation. WHO Technical Report Series 894, 2000.](https://pubmed.ncbi.nlm.nih.gov/11234459/)

- [WHO Expert Consultation. Appropriate body-mass index for Asian populations and its implications for policy and intervention strategies. Lancet, 2004.](https://doi.org/10.1016/S0140-6736(03)15268-3)

- [https://www.cdc.gov/bmi/faq/](https://www.cdc.gov/bmi/faq/)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

Eutrophy (adequate weight) (WHO)

| Result details | |
| --- | --- |
| Weight range with BMI from 18.5 to 24.9 | 56.7 to 76.3 kg |


### 2

Overweight (pre-obesity) (WHO)

| Result details | |
| --- | --- |
| Weight range with BMI from 18.5 to 24.9 | 74.0 to 99.6 kg |


### 3

Class I obesity (WHO)

| Result details | |
| --- | --- |
| Weight range with BMI from 18.5 to 24.9 | 53.5 to 72.0 kg |


### 4

Normal weight (adequate weight) (WHO); in Asians, increased risk

| Result details | |
| --- | --- |
| Weight range with BMI from 18.5 to 24.9 | 53.5 to 72.0 kg |
| Asian action points (WHO 2004) | increased risk |

