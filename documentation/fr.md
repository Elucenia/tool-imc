<!-- ELUCENIA technical documentation · imc · fr · no clinical/professional/rights approval -->

# IMC (indice de masse corporelle)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/imc)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Poids

`peso`

kg · intervalle: 20–350

### Taille

`altura`

cm · intervalle: 100–230

### Population

`pop`

- `g` — Général
- `a` — Asiatique

## Édition de la méthode

OMS/TRS 894/2000 : kg/m², adultes ; points d’action asiatiques 23/27,5, OMS 2004

## Formule documentée

IMC = poids (kg) ÷ taille² (m²).

Pour les populations asiatiques, l’OMS (2004) a ajouté des points d’action en santé publique : 23 kg/m² (risque accru) et 27,5 kg/m² (risque élevé).

## Limites et population

L’IMC relie le poids à la taille, mais ne mesure pas directement la graisse corporelle et ne distingue pas graisse, muscle et os. L’interprétation pédiatrique dépend de l’âge, du sexe et des courbes de référence ; appliquer la classification adulte à une valeur calculée chez un enfant ne démontre pas son applicabilité. Le CDC distingue les enfants et adolescents de 2–19 ans des adultes à partir de 20 ans ; cette frontière appartient à ses recommandations et ne remplace pas automatiquement l’édition de la classification présentée ici. Le résultat doit être interprété avec d’autres données cliniques.

## Références

- [World Health Organization. Obesity: preventing and managing the global epidemic. Report of a WHO consultation. WHO Technical Report Series 894, 2000.](https://pubmed.ncbi.nlm.nih.gov/11234459/)

- [WHO Expert Consultation. Appropriate body-mass index for Asian populations and its implications for policy and intervention strategies. Lancet, 2004.](https://doi.org/10.1016/S0140-6736(03)15268-3)

- [https://www.cdc.gov/bmi/faq/](https://www.cdc.gov/bmi/faq/)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Eutrophie (poids adéquat) (OMS)

| Détails du résultat | |
| --- | --- |
| Plage de poids avec IMC de 18,5 à 24,9 | 56,7 à 76,3 kg |


### 2

Surpoids (pré-obésité) (OMS)

| Détails du résultat | |
| --- | --- |
| Plage de poids avec IMC de 18,5 à 24,9 | 74,0 à 99,6 kg |


### 3

Obésité de classe I (OMS)

| Détails du résultat | |
| --- | --- |
| Plage de poids avec IMC de 18,5 à 24,9 | 53,5 à 72,0 kg |


### 4

Normopondéral (poids adéquat) (OMS) ; chez les Asiatiques, risque accru

| Détails du résultat | |
| --- | --- |
| Plage de poids avec IMC de 18,5 à 24,9 | 53,5 à 72,0 kg |
| Seuils d’action pour les Asiatiques (OMS 2004) | risque accru |

