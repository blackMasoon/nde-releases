---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.2
    </div>
  footerTemplate: |-
    <div style="font-size: 8px; width: 100%; display: flex; justify-content: space-between; padding: 0 20px; color: #78716c; font-family: 'Cinzel', serif;">
      <span>Nano Dungeon Engine</span>
      <span>Page <span class="pageNumber"></span> of <span class="totalPages"></span></span>
    </div>
  margin:
    top: "20mm"
    bottom: "20mm"
    left: "20mm"
    right: "20mm"
generated_at: "2026-01-12T20:13:48.803Z"
---


<style>
    body > h1:first-of-type, .markdown-body > h1:first-of-type { 
        text-align: center; 
        font-size: 2.5em; 
        border-bottom: 2px solid #b91c1c; 
        padding-bottom: 0.5em;
        margin-bottom: 2em;
    }
</style>

<style>
    h1 { color: #1c1917; }
    
    /* Dice & Tokens */
    .rpg-token {
        display: inline-block;
        padding: 0 0.3em;
        border-radius: 0.25em;
        font-weight: bold;
        font-family: 'Courier New', Courier, monospace;
        white-space: nowrap;
        font-size: 0.9em;
    }
    .token-d4 { background-color: #fef08a; color: #854d0e; border: 1px solid #eab308; }
    .token-d6 { background-color: #e2e8f0; color: #1e293b; border: 1px solid #94a3b8; }
    .token-d8 { background-color: #bfdbfe; color: #1e40af; border: 1px solid #60a5fa; }
    .token-d10 { background-color: #d8b4fe; color: #6b21a8; border: 1px solid #c084fc; }
    .token-d12 { background-color: #fbcfe8; color: #9d174d; border: 1px solid #f472b6; }
    .token-d20 { background-color: #bbf7d0; color: #166534; border: 1px solid #4ade80; }
    .token-tn { background-color: #451a03; color: #ea580c; border: 1px solid #9a3412; }
    
    /* Footer Styling */
    .pdf-footer {
        font-family: 'System-ui', sans-serif;
        font-size: 9px;
        color: #78716c;
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0 20px;
        border-top: 1px solid #e7e5e4;
        padding-top: 8px;
    }
    .footer-logo { height: 16px; vertical-align: middle; opacity: 0.6; margin-left: 10px; }
    
    /* Density Adjustments */
    h1, h2, h3, h4 { margin-top: 1em; margin-bottom: 0.5em; }
    p, ul, ol, blockquote { margin-bottom: 0.6em; }
    hr { margin: 1.5em 0; border: 0; border-top: 1px solid #e7e5e4; }
</style>
# Règles en bref

Automatic translation placeholder for fr

---



---

### 1) Héros en 1 minute

- Rôle (choisissez-en un) :
  - Guerrier — maître de la force et du combat rapproché
  - Voleur — maître de la vitesse, de la furtivité et des tirs
  - Mage — maître des sorts et du savoir
- Caractéristiques et dés : Force (F), Dextérité (D), Magie (M).
  - Guerrier : F <span class="rpg-token token-d10">d10</span>, D <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d6">d6</span>
  - Voleur : F <span class="rpg-token token-d6">d6</span>, D <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
  - Mage : F <span class="rpg-token token-d6">d6</span>, D <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d10">d10</span>
- Vie : 5 Cœurs. Mana : 3 (utilisé pour les sorts).
- Équipement : arme, armure légère, 3 objets correspondant au rôle.
Exemple : Le Voleur a Dextérité <span class="rpg-token token-d10">d10</span>, donc pour les tirs, il utilise <span class="rpg-token token-d10">d10</span>.



---

### 2) Comment exécuter des actions

1. Choisissez la caractéristique appropriée (S/Z/M) et lancez le dé de cette caractéristique.
2. Comparez au niveau de difficulté (<span class="rpg-token token-tn">TN</span>) :
   - Facile 4, Normal 6, Difficile 8, Héroïque 12.
3. Résultat :
   - 1 sur le dé — échec avec complication (bruit, perte de temps, petite blessure, etc.).
   - Résultat < <span class="rpg-token token-tn">TN</span> — échec.
   - Résultat ≥ <span class="rpg-token token-tn">TN</span> — succès.
   - Maximum sur le dé (par exemple 10 sur <span class="rpg-token token-d10">d10</span>, 20 sur <span class="rpg-token token-d20">d20</span>) — succès exceptionnel avec un avantage supplémentaire.
Améliorations sans comptage :
- Meilleure/ pire situation : abaissez/ augmentez le <span class="rpg-token token-tn">TN</span> d'un niveau (par exemple, 6 → 8 grâce à une couverture).
- Aide d'un allié (avec son action) : pour ce lancer, "augmentez" le dé d'une taille (<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>).
Exemple : Le guerrier défonce la porte (Normal 6). Il lance un <span class="rpg-token token-d10">d10</span> et obtient 10 — succès exceptionnel : la porte vole en éclats, et le garde derrière elle tombe.



---

### 3) Mouvement et combat sur le plateau

- Mouvement : jusqu'à 5 cases (diagonales autorisées).
- Ton tour : Mouvement + 1 Action (par exemple, attaque, sort, fouille, lever un levier).
- Attaque :
  - Corps à corps (C) : jet contre la <span class="rpg-token token-tn">TN</span> de l'adversaire.
  - Distance (D) : la couverture de la cible augmente la <span class="rpg-token token-tn">TN</span> de 1 niveau.
- <span class="rpg-token token-tn">TN</span> des adversaires : Soldat 6, Élite 8, Boss 12.
- Effets d'un coup : Soldat — tombe après un coup ; Élite — le MJ peut exiger des conditions favorables ; Boss — a 3 Blessures (un coup = 1 Blessure). Succès exceptionnel contre le Boss = 2 Blessures.
- Riposte : si tu manques en corps à corps ou dans la portée de riposte, tu perds 1 Cœur (sauf si tu as une couverture totale).
Exemple : Mage (D <span class="rpg-token token-d6">d6</span>) tire avec une fronde sur un soldat derrière un coffre : <span class="rpg-token token-tn">TN</span> 6 + couverture → 8. Le Mage demande de l'aide au Voleur (augmente le dé à <span class="rpg-token token-d8">d8</span>) et change de position pour une meilleure couverture (<span class="rpg-token token-tn">TN</span> descend à 6). <span class="rpg-token token-d8">d8</span>=7 — touché.



---

### 4) Magie (prosto)

- Lancer un sort : décrivez l'effet, dépensez du Mana, lancez Magie (M).
  - Astuce (flamme, bruit, brouillard) — <span class="rpg-token token-tn">TN</span> 4, coût 0–1 Mana.
  - Projectile/Protection/Saut de 5 cases — <span class="rpg-token token-tn">TN</span> 6, coût 1 Mana.
  - Zone/Soin +2 Cœurs/Paralysie — <span class="rpg-token token-tn">TN</span> 8, coût 2 Mana.
  - Grande puissance (pont de glace, tempête de feu) — <span class="rpg-token token-tn">TN</span> 12, coût 3 Mana.
- Échec : La Mana est perdue ; une petite conséquence survient (essoufflement −1 Cœur ou attention non désirée des ennemis).
- Repos après le combat : vous récupérez toute votre Mana ; un repos en sécurité restaure également des Cœurs.
Exemple : « Éclair » (téléportation courte de 5 cases) : <span class="rpg-token token-tn">TN</span> 6, coût 1 Mana. Le mage <span class="rpg-token token-d10">d10</span> lance 7 — saut réussi derrière la protection.



---

### 5) Chute et guérison

- 0 Cœur : renversé (tu ne fonctionnes pas). Un allié peut utiliser une action pour te relever à 1 Cœur.
- Après un affrontement, après un court repos et un repas, vous revenez à plein de Cœurs et de Mana.
Exemple : Le Voleur tombe à 0. Le Guerrier l'aide à se relever — le Voleur revient à 1 Cœur.



---

### 6) Développement des PERSONNAGES

Po l'aventure, choisis une option :
- Augmente un attribut d'une taille de dé : <span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>,
- ou +1 Cœur (max 7),
- ou +1 Mana (max 5).
Exemple : Le Guerrier augmente sa Force de <span class="rpg-token token-d10">d10</span> à <span class="rpg-token token-d12">d12</span> — il est plus facile d'atteindre la <span class="rpg-token token-tn">TN</span> 12.



---

### 7) Variante seulement-<span class="rpg-token token-d6">d6</span>

Lorsque vous n'avez qu'un seul dé <span class="rpg-token token-d6">d6</span> :
- Au lieu des tailles de dés, chaque caractéristique a un seuil de réussite :
  - Maître 3+, Formé 4+, Novice 5+, Sans compétence 6.
- La <span class="rpg-token token-tn">TN</span> modifie toujours la situation d'un degré (plus facile/difficile).
- Aide : abaissez le seuil de 1 (par exemple, de 4+ à 3+ pour ce lancer).
- Développement : augmentez le niveau d'une caractéristique (par exemple, Formé 4+ → Maître 3+) ou +1 Cœur/Mana.
Exemple : Tir de Voleur (Formé 4+) sur une cible en légère couverture (d'un degré plus difficile) nécessite 5+. Lancer <span class="rpg-token token-d6">d6</span>=5 — touche.

