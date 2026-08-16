# ÉLAN — Système de Marque

> La maison d'édition de développement personnel dont la **marque de fabrique** est
> de coupler un **ebook** + une **app IA d'accompagnement** : un coaching de
> transformation réel, accessible à toutes les bourses.

## Maison d'édition : « Les Éditions ÉLAN »

ÉLAN publie ses contenus sous le label **« Les Éditions ÉLAN »**. C'est la signature
éditoriale qui donne son **sérieux** et sa **ligne éditoriale** au catalogue.

### Hiérarchie de marque

```
                ÉLAN                ← la maison (marque mère)
      ┌────────────┴────────────┐
  LES ÉDITIONS ÉLAN              les produits numériques
      │                         (apps : KETO 360°, coach IA)
  ┌───┴────────────┐
  publications     / collections
  (ebooks, guides) / (les apps)
```

- **ÉLAN** : la marque mère (valeurs, promesse).
- **Les Éditions ÉLAN** : le label éditorial qui signe chaque **publication**
  (ebook, guide, livre). = la ligne éditoriale, la sélection, le catalogue.
- **Produits numériques** (apps) : compléments IA des publications, co-signés
  par ÉLAN (ex. « KETO 360° — une app des Éditions ÉLAN »).

### Bloc de signature éditoriale (à apposer sur chaque publication)

Composition recommandée, sous le logo :

```
                🦌  (logo officiel)
               ÉLAN
         LES ÉDITIONS ÉLAN
   ───  Titre de la publication  ───
```

Règles :
- Toujours associer le **titre** de la publication à la signature.
- Si le produit a une app, mentionner « + app IA » en sous-ligne.
- Le label s'écrit **« Les Éditions ÉLAN »** (majuscules de tête sur Éditions).

### Nomenclature de catalogue (numérotation)

Chaque publication reçoit une référence pour renforcer le sérieux éditorial :

| Réf | Publication | Produit lié |
|-----|-------------|-------------|
| ED-001 | Guide de la réussite | App Guide de la réussite |
| ED-002 | KETO 360° — Guide cétogène | App KETO 360° |

_Règle : ED-XXX incrémental par ordre de publication. La référence apparaît discrètement
en bas de couverture._

## Positionnement

- **Promesse** : la transformation, accompagnée. Pas seulement un livre qu'on lit
  une fois, pas seulement une app qu'on ouvre par hasard — mais **les deux**,
  reliés par une intelligence qui vous suit.
- **Différenciateur** : une **maison** (Les Éditions ÉLAN) qui publie le couple
  ebook + app IA = un catalogue cohérent, édité, digne de confiance. C'est ce que
  personne d'autre ne fait, et c'est le cœur de toute communication ÉLAN.
- **Public** : personnes qui veulent changer, de tous budgets. Ton accessible,
  chaleureux, jamais élitiste ni intimidant.
- **Valeurs** : mouvement (avancer), accessibilité (à la portée de tous),
  accompagnement (pas seul face au changement).

## Principes de marque

1. **Toujours présenter le couple** ebook + app IA (jamais l'un sans l'autre dans
   la communication de marque).
2. **Ton chaleureux et moteur** : encourager, donner de l'élan, pas sermonner.
3. **Simple et accessible** : langage clair, pas de jargon.
4. **Cohérence multi-produits** : un socle commun (ce document) + un thème couleur
   par produit.

## Socle commun (identique pour TOUS les produits)

Ce qui fait qu'un visiteur reconnaît « c'est de la maison ÉLAN » :

- **Typographie titres** : Playfair Display (serif, premium, chaleureux)
- **Typographie texte** : Inter (lisible, moderne, accessible) — Lato en variante
- **Arrondis** : `rounded-xl` / `rounded-2xl` (prononcés mais pas cartoon)
- **Ombres** : douces, `shadow-xl` maximum, jamais trop dures
- **Micro-interactions** : `hover:scale-105 transition-all duration-300` sur tout
  élément cliquable
- **Espacements** : généreux (`py-20`, `px-8`, `gap-8`)
- **Grammaire de composants** : cartes à fond translucide, badges de section,
  boutons CTA pleins, logo « bloc chiffre » (le chiffre du produit dans un carré)
- **Logo-family** : icône emblème + nom ÉLAN + déclinaison produit

## Thèmes couleur par produit

Le socle est partagé ; seule la **palette** change par produit.

| Produit | Fond | Accent 1 | Accent 2 | Typo |
|---------|------|----------|----------|------|
| **Guide de la réussite** (livre) | slate `#0f172a` | ambre `#FBBF24` | émeraude `#10B981` | Playfair + Lato |
| **Cétogène / KETO 360°** (app) | vert sombre `#111816` | vert sauge `#8FBC8F` | or `#D4AF37` | Playfair + Inter |

### Règle des 3 couleurs
Chaque produit respecte la **discipline 3 couleurs** : 1 fond + 1 accent principal
+ 1 accent secondaire. Jamais plus de 3 couleurs dominantes.

## Règle d'or : récupérer la vraie palette

Avant d'inventer une palette pour tout nouveau projet, **récupérer la palette
réelle** depuis les assets existants :
- Sources SVG / covers (extraction des hex `#RRGGBB`)
- `styles.css`, `tailwind.config`, `public/index.html`
- Assets print/web déjà produits

La palette doit refléter la réalité du produit, pas une valeur par défaut.

## Livrables de marque (par produit)

Chaque produit ÉLAN expose, idéalement :
- Logo produit (emblème + nom)
- Palette (tokens couleur) — `tokens/`
- Typographie — incluse au socle
- Modèles de rendus : landing, visuel pub, email — dans `templates/`
- Assets source/web/print — `assets/{source,print,web}`

## Structure recommandée

```
ELAN/
  brand-guide.md          # ce document
  tokens/                 # palettes par produit (CSS/JSON)
  templates/              # landing, visuel pub, email par produit
  assets/                 # logos, assets source/web/print
```
