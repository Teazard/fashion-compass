
# Fashion Compass

Un **fashion compass interactif**, inspiré des *political compasses*, pour positionner des styles, esthétiques ou silhouettes sur deux axes culturels.

Le placement se fait librement par clic ou glisser-déposer, comme une tier list en 2D.

---

## Concept

Le Fashion Compass repose sur deux axes :

- **Marginal → Dominant**  
  De la marge culturelle aux codes dominants / institutionnels

- **Sobre → Exubérant**  
  De l’esthétique minimaliste à l’expression visuelle maximale

### Quadrants

- **Avant-garde** — Exubérant & Marginal  
- **Bourge** — Exubérant & Dominant  
- **Prolo** — Sobre & Marginal  
- **Beige** — Sobre & Dominant  

---

## Fonctionnalités

- Placement de points par clic
- Déplacement par drag & drop
- Suppression par double-clic
- Fonds colorés par quadrant
- Export des points en JSON
- Import par collage de JSON (fusion automatique)
- Composant 100% front-end (aucun backend requis)

---

## Format des données

Les données sont stockées sous forme de tableau JSON :

```json
[
  {
    "id": "uuid-optionnel",
    "x": -0.4,
    "y": 0.7,
    "label": "Goth",
    "color": "hsl(290 70% 55%)"
  }
]
```

* `x` : Marginal (-1) → Dominant (+1)
* `y` : Sobre (-1) → Exubérant (+1)
* `id` est optionnel (généré automatiquement)
* Les imports fusionnent les points existants (pas de remplacement global)

---

## Installation

Aucune dépendance.

```bash
git clone https://github.com/TON-USER/fashion-compass.git
cd fashion-compass
```

Ouvre simplement `fashion-compass.html` dans un navigateur
ou héberge le dossier sur n’importe quel serveur statique.

---

## Personnalisation

Tout se fait dans le fichier HTML :

* Couleurs et noms des quadrants
* Labels des axes
* Taille du canvas
* Typographie
* Logique d’import/export

---

## Roadmap (ouvert aux suggestions)


* Partage par URL
* Tooltips explicatifs par quadrant
* Presets / templates de styles
* Edit des noms d'axes
* Mode collaboratif

