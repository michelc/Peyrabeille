# L'Auberge de Peyrabeille

Version électronique du livre que Paul d'Albigny a consacré à l'histoire de la
célèbre auberge "rouge".

Cet ebook est basé sur la 1° édition parue en 1886, disponible sur le site
Gallica de la BNF (http://gallica.bnf.fr/ark:/12148/bpt6k5802450t).


## Numérotation des pages

A l'écran, je fais apparaitre les numéros de pages qui correspondent à la
première édition de 1886. Cela facilite la relecture et la comparaison avec le
texte d'origine.

Ces numéros de page sont masqués à l'impression, car ils ne sont pas
synchronisés avec la pagination obtenue lors d'une impression au format A4
portrait.

Malgré tout, la table des matières indique les numéros de pages de l'édition
originale aussi bien à l'écran qu'à l'imprimante.


## Pages blanches

Dans l'édition d'origine, on trouve des pages blanches avant certains chapitres,
pour que ceux-ci démarrent sur une page de droite. Ces pages blanches sont ici
définies sous la forme : `<div class="blank"></div>` :

* A l'écran, ces pages blanches sont matérialisées par une dizaine de lignes
vides.
* A l'impression, ces pages blanches ne sont pas rendues.

A l'impression, les chapitres ne commençent donc pas toujours sur une "belle"
page (page de droite, impaire), mais ce n'était pas non plus le cas de tous les
chapitres dans l'édition originale du livre.

Pour avoir au minimum une page blanche au dos de la couverture (et au dos de la
page à propos qui n'existe pas dans l'édition d'origine), une balise
`<div class="verso"></div>` a été utilisée.

A l'écran, cette classe est matérialisée par une dizaine de lignes vides. A
l'impression, elle est rendue sous forme d'une page vide grâce à la propriété
CSS `page-break-before: always`.
