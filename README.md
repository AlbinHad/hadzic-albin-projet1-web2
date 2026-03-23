# DOCUMENTATION

## 1. Nomenclature CSS

J’ai utilisé la méthode BEM (Block, Element, Modifier) pour nommer mes classes.
Je trouve que c’est plus clair et ça aide à ne pas mélanger les styles.

Par exemple :

* `.nav` pour le bloc
* `.nav__menu` pour un élément
* `.card--service` pour une variante

---

## 2. Variables CSS

J’ai utilisé des variables dans `:root` pour les couleurs et les espacements.

Exemples :

* `--color-primary-green1`
* `--space-4`

Ça permet de modifier facilement le design sans toucher à tout le code.

---

## 3. Composants réutilisables

J’ai créé des composants que je réutilise :

* `.card`
* `.btn`
* `.section`
* `.nav`

Ça rend le projet plus organisé et évite de répéter du code.

---

## 4. Flexbox

J’ai utilisé Flexbox pour organiser les éléments :

* les boutons
* la navbar
* le hero
* les cartes

Par contre j’ai eu **de la difficulté avec flexbox**, surtout avec la navbar.
Même après plusieurs tests, je n’ai pas réussi à avoir un comportement parfaitement stable.

Par exemple :

* les éléments changeaient de position
* le menu ne restait pas toujours aligné comme voulu
* certaines valeurs donnaient des résultats inattendus

J’ai quand même réussi à faire fonctionner les autres sections correctement en contrôlant mieux les éléments individuellement.

---

## 5. Fonctions CSS

Je n’ai pas utilisé `clamp()` ou `calc()`.
J’ai préféré rester simple avec des valeurs fixes.

---

## 6. Problèmes rencontrés

J’ai rencontré plusieurs problèmes :

* flexbox difficile à maîtriser
* la navbar qui ne se comportait pas comme prévu
* une classe globale `.cards` qui affectait tout
* l’image du hero qui causait des problèmes de layout

Solutions :

* séparation des sections (`about__cards`, `services__cards`)
* ajustement de `flex-shrink` et `flex-wrap`
* simplification du layout

Même si tout n’est pas parfait, j’ai réussi à stabiliser la majorité du site.

---

## 7. Utilisation de l’IA

J’ai utilisé ChatGPT pour m’aider.

Outil : ChatGPT
Version : GPT-5.3
Date : 2026

L’IA m’a aidé à :

* comprendre certains concepts de flexbox
* corriger des erreurs


J’ai testé et validé plusieurs fois les solutions moi-même.

## 8. Problème avec l’image du hero

J’ai aussi eu un problème avec l’image dans le hero.
Même après plusieurs changements avec flexbox, l’image continuait de “shrink” au lieu de se déplacer comme je voulais.

J’ai essayé plusieurs propriétés comme `flex-shrink`, `width` et `max-width`, mais le comportement changeait souvent selon les autres éléments.

Finalement, j’ai réussi à améliorer un peu le rendu en ajustant le flex seulement sur l’image, mais ça a été un des points les plus difficiles à gérer dans mon projet.

