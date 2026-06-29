# ⚡ APEX

**Transforme ton entraînement réel en jeu de rôle.** Tu logges tes vraies séances de muscu, l'app calcule ta performance, te donne de l'XP honnête, te fait monter des niveaux et des rangs.

Mélange de deux inspirations :
- **Liftoff** → rang par exercice + progression chiffrée du 1RM.
- **Habitica** → avatar, niveau, points de vie, streak, quêtes et récompenses.

## ▶️ Lancer l'app

Aucune installation, aucune dépendance. **Double-clique sur [`index.html`](index.html)** — ça s'ouvre dans ton navigateur et fonctionne hors-ligne. La progression est sauvegardée en local dans le navigateur.

Pour repartir du profil de démo propre : ouvre la console du navigateur et tape `APEX.reset()`.

## 📱 Écrans

- **Accueil** — avatar + barre d'XP, Indice de Force, flamme de streak, points de vie, quêtes du jour/semaine.
- **Logger** — choix d'exercice (ou crée le tien), poids/reps/séries, 1RM estimé en direct, animation de record/montée de rang.
- **Progression** — rang métallique par exercice, courbe du 1RM dans le temps, vue du corps (groupes musculaires travaillés).
- **Quêtes** — 4 étages : journalier, hebdo, mensuel, annuel. Les petites quêtes ouvrent la grosse mission du mois.
- **Cercle** — mini-classement entre potes (niveau, rang, streak).
- **Récompenses** — les tiennes, débloquées sur un record ou une montée de niveau.

## 🔧 Le moteur d'XP

- **1RM estimé (Epley)** : `poids × (1 + reps / 30)`.
- Comparé au meilleur passé du même exercice : record **+30 XP**, solide (≥ −5 %) **+15**, léger **+5**, première fois **+15**.
- Présence par séance : **+20 XP**.
- **Streak** : +10 % d'XP par séance enchaînée, plafond +50 %.
- **Niveaux** : le 1ᵉʳ coûte 100 XP, chaque suivant ×1,15 (la montée ralentit).
- **Points de vie** : 100 au départ, −10 par séance prévue et sautée.
- **XP d'une séance** = (présence + somme des XP des exercices) × multiplicateur de streak.
- **Rangs par exercice** (Bronze → Argent → Or → Platine → Titan) basés sur le ratio **1RM / poids de corps**, pas le poids brut.

> Règle d'or : l'XP colle à l'effort réel. Jamais gonflée.

## 🗂️ Stack

Un seul fichier `index.html` — HTML, CSS et JavaScript vanilla, zéro dépendance. Graphes et silhouettes en SVG inline.
