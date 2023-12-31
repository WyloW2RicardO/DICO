# Markdown
Commencé le 2023-10-12
## Abstract
Ce document servira à referancé les fonction des ficher Markdown (.md).
Vous pouver toujour suivre la methode pas a pas [ici](https://github.com/skills/communicate-using-markdown).
## Style
### Parametre
police de largeur fixe ; Profil > Settings > Apparence > Préférence de police de l’éditeur Markdown > sélectionnez
### Ecriture
|Style           |Syntaxe          |Raccourci|
|-:              |-                |:-:      |
|Italique        |`*txt*`          |Ctrl+I   |
|Gras            |`**txt**`        |Ctrl+B   |
|Gras et Italique|`***txt***`      |None     |
|Barré           |`~~txt~~`        |None     |
|Indice          |`<sub>txt</sub>` |None     |
|Exposant        |`<sup>txt</sup>` |None     |
|Citation        |`>txt`           |None     |
|Code            |``` `txt` ```    |Crtl+E   |
|Comantaire      |`<!--txt-->`     |None     |
### Alertes
`>[!Type]` et en citation les informations
|Style             |Type       |Couleur|
|-:                |-          |:-:    |
|Met en evidance   |`NOTE`     |Bleu   |
|Facultatives      |`TIP`      |Vert   |
|Necessary         |`IMPORTANT`|Violet |
|Risques potentiels|`WARNING`  |Ocre   |
|Negative          |`CAUTION`  |Rouge  |
## Liste
- ***Table*** ; `|` pour séparent chaque colonne et `-` pour créer l'en-tête de chaque colonne, Il doit y avoir au moins trois traits d’union dans chaque colonne de la ligne d’en-tête. Plus [ici](https://docs.github.com/fr/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-tables)
- ***Tiré*** ; précéder une ou plusieurs lignes de texte de `1.`
- ***Non-tiré*** ; précéder une ou plusieurs lignes de texte de `-`
- ***Imbiqué*** ; `-` se trouve directement sous le premier caractère du texte dans l'élément au-dessus de lui, Tab ou Maj+Tab
- ***Taches*** ; ` - []` et `- [x]` pour une tache terminer et `\(optional)`. Plus [ici](https://docs.github.com/fr/get-started/writing-on-github/working-with-advanced-formatting/about-task-lists)
## Lien
- ***Mention*** ; `@` affiche une liste de personnes ou d'équipes sur un projet
- ***Inline*** ; `[txt]` texte du lien et `(url)` pour l'URL
- ***Section*** ;
- ***Relatif*** ; `/NOM.md` pur l'URL de l'Inline et utiliser operande `./` ou `../`
- ***Image*** ; `!` est ajouter en amontd'un lien Inline
- ***Note*** ; `[^Nm]` apres le mot puis `[^NUM]:` pour ecrire la note
