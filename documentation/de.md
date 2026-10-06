<!-- ELUCENIA technical documentation · imc · de · no clinical/professional/rights approval -->

# BMI (Body-Mass-Index)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/imc)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Gewicht

`peso`

kg · Bereich: 20–350

### Körpergröße

`altura`

cm · Bereich: 100–230

### Population

`pop`

- `g` — Allgemein
- `a` — Asiatisch

## Fassung der Methode

WHO/TRS 894/2000: kg/m², Erwachsene; asiatische Aktionsschwellen 23/27,5, WHO 2004

## Dokumentierte Formel

BMI = Gewicht (kg) ÷ Körpergröße² (m²).

Für asiatische Populationen ergänzte die WHO (2004) gesundheitspolitische Aktionsschwellen: 23 kg/m² (erhöhtes Risiko) und 27,5 kg/m² (hohes Risiko).

## Grenzen und Population

Der BMI setzt Gewicht und Größe in Beziehung, misst Körperfett aber nicht direkt und unterscheidet nicht zwischen Fett, Muskel und Knochen. Die pädiatrische Interpretation hängt von Alter, Geschlecht und Referenzkurven ab; die Erwachsenenklassifikation auf einen berechneten Kinderwert anzuwenden belegt keine Eignung. CDC unterscheidet Kinder und Jugendliche von 2–19 Jahren und Erwachsene ab 20 Jahren; diese Grenze gehört zur CDC-Empfehlung und ersetzt nicht automatisch die hier dargestellte Klassifikationsausgabe. Das Ergebnis muss mit weiteren klinischen Daten interpretiert werden.

## Referenzen

- [World Health Organization. Obesity: preventing and managing the global epidemic. Report of a WHO consultation. WHO Technical Report Series 894, 2000.](https://pubmed.ncbi.nlm.nih.gov/11234459/)

- [WHO Expert Consultation. Appropriate body-mass index for Asian populations and its implications for policy and intervention strategies. Lancet, 2004.](https://doi.org/10.1016/S0140-6736(03)15268-3)

- [https://www.cdc.gov/bmi/faq/](https://www.cdc.gov/bmi/faq/)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Eutrophie (angemessenes Gewicht) (WHO)

| Ergebnisdetails | |
| --- | --- |
| Gewichtsbereich mit einem BMI von 18,5 bis 24,9 | 56,7 bis 76,3 kg |


### 2

Übergewicht (Präadipositas) (WHO)

| Ergebnisdetails | |
| --- | --- |
| Gewichtsbereich mit einem BMI von 18,5 bis 24,9 | 74,0 bis 99,6 kg |


### 3

Adipositas Grad I (WHO)

| Ergebnisdetails | |
| --- | --- |
| Gewichtsbereich mit einem BMI von 18,5 bis 24,9 | 53,5 bis 72,0 kg |


### 4

Normalgewicht (angemessenes Gewicht) (WHO); bei Asiaten erhöhtes Risiko

| Ergebnisdetails | |
| --- | --- |
| Gewichtsbereich mit einem BMI von 18,5 bis 24,9 | 53,5 bis 72,0 kg |
| Handlungsgrenzen für Asiaten (WHO 2004) | erhöhtes Risiko |

