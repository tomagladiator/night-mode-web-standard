# Night Mode in web, why not a standard yet ?
Propose a standard for including Night Mode in browsers

Currently, this note is in french, please, help me to translate it!

## Contexte
Pour nombre d'entre nous, notre quotidien et notre santé est altéré par la puissance lumineuse de certains sites populaires. Une lumière blanche à bleuté trompe notre cerveau pour lui donner l'illusion qu'il fait encore jour et celui-ci tente de rester éveillé ce qui cause des troubles du sommeil et des mals de tête, tout âge confondu.

## Problème
Les sites utilisant le texte noir sur fond blanc sont majoritaires, rien d'étonnant puisque depuis l'école nous écrivons à l'encre foncée sur du papier blanc. Le blanc est aussi, d'un point de vue marketing, associé à la pureté, au minimalisme, ce qui plait au web-designers.

## Solution
Les navigateurs devraient, si le site l'offre, afficher un bouton natif pour passer en mode nuit.

L'utilisation d'une simpte META faisant référence à un CSS devrait être suffisant.

`<link href="/styles/nightmode.css" rel="nightmode">`

1 - Par défaut, le navigateur ne téléchargerait pas ce CSS pour des raisons de performance, mais ferait une vérification si celui-ci ne retourne pas une 404.

2 - Par la présence de la META dans la balise HEAD, le navigateur verrait apparaitre dans sa barre de recherche une nouvelle icone

3 - Au clic sur celui-ci le CSS serait appliqué et l'icone changerait en mode actif

4 - Une option permettrait d'activer automatiquement le mode nuit pour tous les sites le supportant

## Recommandation
Ne pas utiliser un texte blanc #fff sur fond noir #000, privilégier un fond foncé #252525 et une couleur de texte gris clair de #dadada

Appliquer une transition CSS3 pour le changement de couleur

Éviter de placer des images dont la transparence est simulée par le fonds blanc de l'image sur le fond blanc du site.
