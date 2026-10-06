<!-- ELUCENIA technical documentation · imc · es · no clinical/professional/rights approval -->

# IMC (índice de masa corporal)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/imc)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Peso

`peso`

kg · intervalo: 20–350

### Estatura

`altura`

cm · intervalo: 100–230

### Población

`pop`

- `g` — General
- `a` — Asiática

## Edición del método

OMS/TRS 894/2000: kg/m², adultos; puntos de acción asiáticos 23/27,5, OMS 2004

## Fórmula documentada

IMC = peso (kg) ÷ altura² (m²).

En poblaciones asiáticas, la OMS (2004) añadió puntos de acción en salud pública: 23 kg/m² (riesgo aumentado) y 27,5 kg/m² (alto riesgo).

## Límites y población

El IMC relaciona peso y altura, pero no mide directamente la grasa corporal ni distingue grasa, músculo y hueso. La interpretación pediátrica depende de edad, sexo y curvas de referencia; aplicar la clasificación adulta a un valor calculado en un niño no demuestra su aplicabilidad. El CDC distingue niños y adolescentes de 2–19 años y adultos a partir de 20 años; ese límite pertenece a la orientación del CDC y no sustituye automáticamente la edición de la clasificación presentada aquí. El resultado debe interpretarse junto con otros datos clínicos.

## Referencias

- [World Health Organization. Obesity: preventing and managing the global epidemic. Report of a WHO consultation. WHO Technical Report Series 894, 2000.](https://pubmed.ncbi.nlm.nih.gov/11234459/)

- [WHO Expert Consultation. Appropriate body-mass index for Asian populations and its implications for policy and intervention strategies. Lancet, 2004.](https://doi.org/10.1016/S0140-6736(03)15268-3)

- [https://www.cdc.gov/bmi/faq/](https://www.cdc.gov/bmi/faq/)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

Eutrofia (peso adecuado) (OMS)

| Detalles del resultado | |
| --- | --- |
| Rango de peso con IMC de 18,5 a 24,9 | 56,7 a 76,3 kg |


### 2

Sobrepeso (preobesidad) (OMS)

| Detalles del resultado | |
| --- | --- |
| Rango de peso con IMC de 18,5 a 24,9 | 74,0 a 99,6 kg |


### 3

Obesidad grado I (OMS)

| Detalles del resultado | |
| --- | --- |
| Rango de peso con IMC de 18,5 a 24,9 | 53,5 a 72,0 kg |


### 4

Eutrofia (peso adecuado) (OMS); en asiáticos, riesgo aumentado

| Detalles del resultado | |
| --- | --- |
| Rango de peso con IMC de 18,5 a 24,9 | 53,5 a 72,0 kg |
| Puntos de acción para asiáticos (OMS 2004) | riesgo aumentado |

