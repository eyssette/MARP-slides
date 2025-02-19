---
marp: true
theme: teaching
paginate: true
size: 4:3
---

<!-- _class: titre -->
<style scoped>
span {font-size:0.7em}
</style>

# Utiliser <br>le Markdown<br>pour tout faire<!-- fit -->

Cédric Eyssette (2022-2023)
https://eyssette.github.io/

---
<!-- _class: partie -->
# I - <br>Pourquoi ? <!-- fit -->
Première partie


---
<!-- _class: souspartie -->
<style scoped>
p {margin:20px 60px; font-size:1.5em}
</style>

## A. Objectif principal

<span data-marpit-fragment="1">→ Travailler seulement avec des fichiers textes</span>

---
<!-- _class: etape fp -->
<style scoped>
h3 {padding-bottom:0.8em; font-size:1.2em}
</style>

### 1/ Un format léger
* **Édition** plus rapide
  * Pas besoin d'un logiciel lourd
  * Pas besoin d'un ordinateur hyper-performant 
  * Logiciels plus adaptés pour l'édition de textes
  * Focalisation sur le fond et pas sur la forme
* **Sauvegarde** plus économe et plus rapide
  * synchronisation facilitée
  * versionnage facilité
* **Recherche** plus rapide dans ses fichiers

<!-- 
VSCodium : évoquer (en parler plus tard)
git, forge pour synchronisation et versionnage
évoquer système de nommage des fichiers -->


---
<!-- _class: etape fpppppp -->
<style scoped>
h3 {padding-bottom:0.8em; font-size:1.2em}
</style>

### 2/ Un format ouvert

* On peut utiliser n'importe quelle **machine** et n'importe quel **logiciel** d'édition de texte
* On peut **collaborer** facilement sur un même fichier
* La **pérennité** du fichier est assurée


<!-- Pas prisonnier d'un logiciel qui doit être installé, on peut travailler de partout même avec un éditeur en ligne
(VS Code : édition en ligne possible) -->


---
<!-- _class: souspartie -->
<style scoped>
p {margin:0px 60px; font-size:1.2em}
</style>

## B. Le Markdown : un bon compromis

<span data-marpit-fragment="1">→ Une syntaxe qui reste simple</span>
<span data-marpit-fragment="2">→ Mais qui permet de créer<br>des documents complexes</span>


---
<!-- _class: etape fppp -->
<style scoped>
h3 {padding-bottom:0.8em; font-size:1.2em}
p {text-align:left;}
</style>

### 1/ Une syntaxe simple

* Titres : `# Titre 1` / `## Titre 2`
* Gras / italiques : `**gras**` / `_italiques_`
* Citations, code : `> citation` / ``` `code` ``` 
* Listes : `- texte` / `1. texte`
* Liens : `[texte](URL)`
* Images : `![description](URL)`


---
<!-- _class:  -->

### Deux avantages

1) Un balisage léger : compréhensible par un être humain et facile à apprendre.
2) Un document structuré : facile à exploiter par un programme informatique.

---
<!-- _class: etape fpp -->
<style scoped>
h3 {padding-bottom:0.5em; font-size:1.2em}
</style>

### 2/ Une syntaxe qui permet de <br>créer des documents complexes

* Possibilité d'intégrer du HTML, du $\LaTeX$
* Des extensions possibles du Markdown
* Possibilité d'avoir un en-tête en YAML
* Des outils pour transformer le markdown en un autre format : <span data-marpit-fragment="1">un pdf</span><span data-marpit-fragment="2">, un diaporama</span><span data-marpit-fragment="3">, un site web</span><span data-marpit-fragment="4">, une carte mentale, …</span>
* Export HTML : intégration possible de styles CSS

<!-- 
Extensions du markdown :
notes de bas de page
tableaux
texte souligné / surligné / supprimé / exposant / indices

https://github.com/CriticMarkup/CriticMarkup-toolkit


Ajouter ?
Des outils pour intégrer dans du markdown d'autres fichiers ?
fichier bibtex pour les 
-->

---
<!-- _class: partie -->
# II - <br>Comment ? <!-- fit -->
Deuxième partie


---
<!-- _class: i1t0 pp -->
<style scoped>
</style>

![](https://raw.githubusercontent.com/eyssette/mindmap/main/utiliser-le-markdown-pour-tout-faire-comment.svg)


---
<!-- _class: souspartie -->
## A. Pour éditer <br>son texte


---
<!-- _class:  -->
<style scoped>
ol {font-size:1.15em}
</style>
1) Une solution en ligne dans Apps Edu : [CodiMD](https://codimd.apps.education.fr/)
2) Un logiciel dédié à l'édition en Markdown
3) Un éditeur de texte brut avec des plugins pour le markdown


---
<!-- _class:  -->
### Logiciel proposé : [VS Codium](https://vscodium.com/)

1) Une interface générale et un système de plugins très pratiques
2) Des raccourcis claviers très efficaces
3) Des snippets configurables

<!-- Faire démonstration :
correction de copies / création d'un diaporama
-->

---
<!-- _class: souspartie -->
<style scoped>
h2 {font-size:1.7em}
p {font-size:1.4em; margin: 0 60px}
</style>
## B. Pour sauvegarder et gérer l'historique

<span data-marpit-fragment="1">→ utiliser _git_ et une forge</span>
<span data-marpit-fragment="2">→ utiliser _diff_</span>

---
<!-- _class: souspartie -->
## C. Pour transformer son fichier dans <br>un autre format


---
<!-- _class: etape fppppppp -->
<style scoped>
span {font-size:0.7em}
</style>
### 1) Document texte au format académique <span>(thèse, article, poster …)</span>

* Fichier Bibtex pour les citations et [plugin pour autocompléter ses citations](https://marketplace.visualstudio.com/items?itemName=notZaki.pandocciter)
* Fichier de style CSL pour les citations
* [Pandoc](https://pandoc.org/) pour la transformation du markdown en PDF (ou un autre format) [:link:](https://programminghistorian.org/fr/lecons/redaction-durable-avec-pandoc-et-markdown) [:link:](https://www.arthurperret.fr/cours/pandoc.html)


<!-- 
https://ineed.coffee/post/how-to-write-an-acm-styled-conference-paper-using-markdownpandoc

http://programminghistorian.org/en/lessons/sustainable-authorship-in-plain-text-using-pandoc-and-markdown
 -->

---
<!-- _class: etape -->
### 2) Diaporama

* Plusieurs solutions possibles : [reveal.js](https://revealjs.com/), [Remark](https://remarkjs.com/#1), [Marp](https://marp.app/) …
* Solution la plus simple : [reveal.js sur CodiMD](https://codimd.apps.education.fr/dj4bCWxPTVeoWWFnZ3uFiA?both)
* Solution plus complète : [Marp](https://marp.app/).
* Exemple de thème : [teaching](https://eyssette.github.io/teaching-theme-for-marp/)

<!-- Montrer comment Marp fonctionne -->


---
<!-- _class: etape -->
### 3) Sites webs

* Plusieurs générateurs de sites statiques : [jekyll](https://jekyllrb.com/), [mkdocs](https://www.mkdocs.org/), [mdbook](https://rust-lang.github.io/mdBook/), [Hugo](https://gohugo.io/) …
* Un même principe : des fichiers en markdown, des propriétés YAML exploitées par le thème, une syntaxe pour créer des modèles de page


---
<!-- _class: etape -->
### 4) Cartes mentales

* Intégration de [Mermaid](https://mermaid.js.org/). Possibilité de créer des [modèles](https://codimd.apps.education.fr/o1E9rMaMTg2rik93decJUg?both).
* Un logiciel en ligne : [myMarkmap](https://mymarkmap.netlify.app/)

<!-- Montrer comment myMarkmap fonctionne -->

---
<!-- _class: etape fppppppp -->
### 5) Des modèles spécifiques

* Idée : créer des modèles dédiés à un usage pédagogique précis
* Des modèles utilisables soit par les collègues soit par les élèves dans le cadre d'une activité qu'on leur fait faire
* Des modèles utilisables sur [CodiMD](https://codimd.apps.education.fr/) et sur [la forge](https://forge.apps.education.fr/)


---
<!-- _class: fppp -->
<style scoped>
h4 {text-align:center}
</style>
#### Exemples

* Un [dialogue](https://codimd.apps.education.fr/KsjwIfUJT8S8X0gs3lsMIA?both) sous la forme de SMS échangés
* Un [cahier de textes](https://codimd.apps.education.fr/vLFQu2JITKey43EMqYi1FA?both)
* Des [flashcards](https://codimd.apps.education.fr/aHGYCpIiRtmiP7ewkoWOYQ?both)
* Un [commentaire d'un texte](https://codimd.apps.education.fr/a8oECv4nSeu6LMsGUfxqVQ?both)
* Un [mur d'images](https://codimd.apps.education.fr/rceCV-QSTIC-f1RJ7pHxIA?both)
* Un [pad](https://codimd.apps.education.fr/lClEnAoTSMenFPVDtmc92g?both)
* Un [dictionnaire](https://eyssette.github.io/dataview/?url=https://codimd.apps.education.fr/aYv4xF8ZQKCWg75h_UOaDQ) [:link:](https://codimd.apps.education.fr/aYv4xF8ZQKCWg75h_UOaDQ)
* Une [frise chronologique](https://codimd.apps.education.fr/pWrVyaN7SMubB1k65zeJzA?both)
* Des [cartes à jouer](https://codimd.apps.education.fr/zuKmY75LR6KmC79V-R5wKg?both)
