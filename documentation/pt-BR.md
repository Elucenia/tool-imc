<!-- ELUCENIA technical documentation · imc · pt-BR · no clinical/professional/rights approval -->

# IMC (Índice de Massa Corporal)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/imc)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Peso

`peso`

kg · intervalo: 20–350

### Altura

`altura`

cm · intervalo: 100–230

### População

`pop`

- `g` — Geral
- `a` — Asiática

## Edição do método

OMS/TRS 894/2000:kg/m², adultos; pontosaçãoasiáticos 23/27,5 WHO 2004

## Fórmula documentada

IMC = peso (kg) ÷ altura² (m²).

Em populações asiáticas, a OMS (2004) acrescentou pontos de ação em saúde pública: 23 kg/m² (risco aumentado) e 27,5 kg/m² (alto risco).

## Limites e população

O IMC relaciona peso e altura, mas não mede diretamente a gordura corporal nem distingue gordura, músculo e osso. A interpretação pediátrica depende de idade, sexo e curvas de referência; aplicar a classificação adulta a um valor calculado em criança não demonstra sua aplicabilidade. O CDC distingue crianças e adolescentes de 2–19 anos e adultos a partir de 20 anos; essa fronteira pertence à orientação do CDC, sem substituir automaticamente a edição da classificação apresentada aqui. O resultado deve ser interpretado com outros dados clínicos.

## Referências

- [World Health Organization. Obesity: preventing and managing the global epidemic. Report of a WHO consultation. WHO Technical Report Series 894, 2000.](https://pubmed.ncbi.nlm.nih.gov/11234459/)

- [WHO Expert Consultation. Appropriate body-mass index for Asian populations and its implications for policy and intervention strategies. Lancet, 2004.](https://doi.org/10.1016/S0140-6736(03)15268-3)

- [https://www.cdc.gov/bmi/faq/](https://www.cdc.gov/bmi/faq/)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
