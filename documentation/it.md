<!-- ELUCENIA technical documentation · imc · it · no clinical/professional/rights approval -->

# IMC (indice di massa corporea)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/imc)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Peso

`peso`

kg · intervallo: 20–350

### Altezza

`altura`

cm · intervallo: 100–230

### Popolazione

`pop`

- `g` — Generale
- `a` — Asiatica

## Edizione del metodo

OMS/TRS 894/2000: kg/m², adulti; punti d’azione asiatici 23/27,5, OMS 2004

## Formula documentata

IMC = peso (kg) ÷ altezza² (m²).

Per le popolazioni asiatiche, l’OMS (2004) ha aggiunto punti d’azione di sanità pubblica: 23 kg/m² (rischio aumentato) e 27,5 kg/m² (alto rischio).

## Limiti e popolazione

L’IMC mette in relazione peso e altezza, ma non misura direttamente il grasso corporeo e non distingue grasso, muscolo e osso. L’interpretazione pediatrica dipende da età, sesso e curve di riferimento; applicare la classificazione adulta a un valore calcolato in un bambino non ne dimostra l’applicabilità. Il CDC distingue bambini e adolescenti di 2–19 anni dagli adulti a partire da 20 anni; tale confine appartiene alle indicazioni del CDC e non sostituisce automaticamente l’edizione della classificazione qui presentata. Il risultato deve essere interpretato insieme ad altri dati clinici.

## Riferimenti

- [World Health Organization. Obesity: preventing and managing the global epidemic. Report of a WHO consultation. WHO Technical Report Series 894, 2000.](https://pubmed.ncbi.nlm.nih.gov/11234459/)

- [WHO Expert Consultation. Appropriate body-mass index for Asian populations and its implications for policy and intervention strategies. Lancet, 2004.](https://doi.org/10.1016/S0140-6736(03)15268-3)

- [https://www.cdc.gov/bmi/faq/](https://www.cdc.gov/bmi/faq/)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
