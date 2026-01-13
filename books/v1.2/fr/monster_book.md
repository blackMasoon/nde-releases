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
generated_at: "2026-01-13T06:26:42.251Z"
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
# Manuel des Monstres

Automatic translation placeholder for fr

---



---

### 1. Introduction

- Nous utilisons les mêmes concepts que dans les règles de base et le livre MG.
- **Seuls les joueurs lancent.** Les adversaires exercent une pression par le biais de la <span class="rpg-token token-tn">TN</span> et des mouvements ; les dégâts résultent généralement de "représailles" ou de tests imposés aux joueurs.



---

### 1. Introduction

> Nom — Classe, <span class="rpg-token token-tn">TN</span>, Blessures, Rôle, Mouvement, Spécial

- **Classe :** Pion | Élite | Boss
- **<span class="rpg-token token-tn">TN</span> :** nombre 4/6/8/12 déterminant la difficulté de toucher/contourner l'adversaire.
- **Blessures :** uniquement pour l'Élite et le Boss (Élite : 2, Boss : 3 par défaut). Le Pion n'a pas de Blessures (il tombe après avoir été touché).
- **Rôle :** Brute (corps à corps), Escarmoucheur (mobile), Artillerie (distance), Contrôleur (contrôle de zone), Soutien (support).
- **Mouvement :** par défaut 5 cases. Changez si la mobilité est unique (ex. 6 Rapide, Vol, Saut 3).
- **Spécial :** 1–2 courtes capacités descriptives (voir les sections « Caractéristiques » et « Mouvements »).

Exemple d'écriture : « Gardien Élitaire — Élite, <span class="rpg-token token-tn">TN</span> 8, Blessures 2, Brute, Mouvement 5, Spécial : Protection Lourde ; Charge ».



---

### Pachołek (minion)

- **Pachołek (minion) :** <span class="rpg-token token-tn">TN</span> 6, schodzi po 1 trafieniu. En quantité, ils créent de la pression. Revanche en cas d'échec : −1 Cœur.
- **Elita :** <span class="rpg-token token-tn">TN</span> 8, 2 Blessures. A généralement 1 caractéristique défensive ou de mobilité. Revanche en cas d'échec : −1 Cœur ; parfois un effet situationnel supplémentaire.
- **Boss :** <span class="rpg-token token-tn">TN</span> 12, 3 Blessures. A 2–3 mouvements spéciaux et influence le terrain/rythme. Peut provoquer des tests chez les joueurs (par exemple, esquive, stabilisation).



---

### Brute (combat rapproché)

- **Brute (corps à corps):** exerce une pression en mêlée, pousse hors de la couverture.
- **Skirmisher (mobile):** entre/sort du contact, punit la solitude.
- **Artillery (distance):** tire depuis la couverture, force au mouvement.
- **Controller (contrôle):** crée des zones de danger, des fumées, des zones de repoussement.
- **Support (soutien):** renforce les alliés, abaisse la <span class="rpg-token token-tn">TN</span> des alliés ou augmente la <span class="rpg-token token-tn">TN</span> des héros d'un degré selon la situation.



---

### 1. Introduction

Ajoutez 1 à 2 au statblock. Ils agissent toujours de manière descriptive ; ils modifient la <span class="rpg-token token-tn">TN</span> d'un degré seulement si cela a du sens.
- **Bouclier Naturel :** à portée de distance, l'adversaire a généralement une couverture partielle (attaque contre lui → <span class="rpg-token token-tn">TN</span> +1 degré).
- **Armure Légère :** la première perte de 1 Cœur due à une riposte contre cette unité dans la scène est ignorée.
- **Dur :** le premier succès contre cette unité ne cause pas de Blessure (il ne fait que repousser/positionner) — bon pour les boss.
- **Rapide (Mouvement 6) :** ignore 1 case de terrain difficile par tour.
- **Grimpeur/Sauter :** se déplace verticalement/sur des obstacles comme sur du plat, saut de 3 cases.
- **Vol :** ignore les obstacles de terrain (le MJ veille à des couvertures sensées).
- **Éclaireur :** plus difficile à surprendre ; la première tentative de furtivité contre lui a une <span class="rpg-token token-tn">TN</span> +1.
- **Résistance [type] :** le premier effet de ce type dans la scène est réduit (le MJ explique : portée plus faible, durée plus courte).
- **Vulnérabilité [type] :** contre ce type d'attaques, la <span class="rpg-token token-tn">TN</span> est réduite d'un degré.
- **Essaims :** lorsqu'il se tient à côté de la cible, la riposte sur un échec peut toucher deux héros dans un rayon de 1.



---

### 1. Introduction

Choisissez 1 à 2 caractéristiques. Les mouvements décrivent l'effet ; s'ils menacent les héros, le MJ peut leur demander de faire un test approprié (D ou M) contre le <span class="rpg-token token-tn">TN</span> de l'adversaire.
- **Pression (Brute) :** après avoir touché un héros, déplacez-le de 1 à 2 cases supplémentaires.
- **Rupture de Protection :** lorsque cette unité touche, la protection de la cible cesse de fonctionner jusqu'à la fin du prochain tour.
- **Tirage (Skirmisher) :** entrer/sortir du corps à corps ne provoque pas de contre-attaque.
- **Salve (Artillery) :** zone 3×3 ; tous dans la zone font un test D contre <span class="rpg-token token-tn">TN</span> ; échec : −1 Cœur et poussée de 1 case.
- **Ancre (Controller) :** le champ 3×3 devient un « terrain collant » (entrer coûte toute l'Action) jusqu'à la fin du prochain tour.
- **Renforcement (Support) :** un allié a un avantage de 1 degré jusqu'à la fin du tour (les attaquants contre lui ont <span class="rpg-token token-tn">TN</span> +1).
- **Invocation (Boss) :** une fois au début, invoque 2 pions dans des cases libres.
- **Barrière (Boss) :** jusqu'à la fin du tour de la partie divine, les héros effectuent des attaques à distance avec <span class="rpg-token token-tn">TN</span> +1.
- **Choc (Boss) :** tous dans un rayon de 2 cases font un test S contre <span class="rpg-token token-tn">TN</span> ; échec : −1 Cœur ou renversement (vous perdez votre Mouvement ce tour-ci).



---

### 1. Introduction

1) **Choisissez une classe :** Panneau / Élite (2 Blessures) / Boss (3 Blessures).
2) **Définissez le <span class="rpg-token token-tn">TN</span> :** 6 / 8 / 12 (exceptionnellement 4 pour des très faibles ou 10 pour des élites coriaces).
3) **Attribuez un rôle :** Brute, Éclaireur, Artillerie, Contrôleur, Support.
4) **Ajoutez 1 à 2 caractéristiques** et **1 mouvement spécial** (Boss : 2 à 3 mouvements).
5) **Mouvement :** généralement 5 ; changez uniquement si c'est crucial.

C'est prêt. Ce squelette fonctionne dans tous les univers.



---

### 1. Introduction

7.2 Remplacez les entrées ci-dessous par des noms/couleurs du monde.

### 7.1 Pions
- **Gardien Pion — Pion, <span class="rpg-token token-tn">TN</span> 6, —, Brut, Mouvement 5, Spécial : Protection Naturelle.**
- **Éclaireur Pion — Pion, <span class="rpg-token token-tn">TN</span> 6, —, Éclaireur, Mouvement 6, Spécial : Éclaireur.**
- **Tireur Pion — Pion, <span class="rpg-token token-tn">TN</span> 6, —, Artillerie, Mouvement 5, Spécial : Salve (petite zone 2×2, avertit seulement : en cas d'échec -1 Cœur).**
- **Contrôleur Pion — Pion, <span class="rpg-token token-tn">TN</span> 6, —, Contrôleur, Mouvement 5, Spécial : Ancre (pour 1 tour, une seule fois).**
- **Soutien Pion — Pion, <span class="rpg-token token-tn">TN</span> 6, —, Soutien, Mouvement 5, Spécial : Renforcement (une fois par scène).**

### 7.2 Élites
- **Garde Élite — Élite, <span class="rpg-token token-tn">TN</span> 8, Blessures 2, Brute, Mouvement 5, Spécial : Armure Légère ; Poussée.**
- **Assassin Élite — Élite, <span class="rpg-token token-tn">TN</span> 8, Blessures 2, Éclaireur, Mouvement 6, Spécial : Tirage ; Vulnérabilité [observation] (plus facile à détecter).**
- **Tireur Élite — Élite, <span class="rpg-token token-tn">TN</span> 8, Blessures 2, Artillerie, Mouvement 5, Spécial : Couverture Naturelle ; Salve (3×3 après préparation).**
- **Contrôleur Élite — Élite, <span class="rpg-token token-tn">TN</span> 8, Blessures 2, Contrôleur, Mouvement 5, Spécial : Ancre ; Poussée de 1 case en cas de succès exceptionnel.**
- **Médecin Élite — Élite, <span class="rpg-token token-tn">TN</span> 8, Blessures 2, Soutien, Mouvement 5, Spécial : Renforcement ; en cas de touche, annule 1 complication d'un allié (de manière descriptive).**

### 7.3 Bosses
- **Leader — Boss, <span class="rpg-token token-tn">TN</span> 12, Blessures 3, Support, Mouvement 5, Spécial : Invocation ; Renforcement ; Barrière.**
- **Colosse — Boss, <span class="rpg-token token-tn">TN</span> 12, Blessures 3, Brute, Mouvement 5, Spécial : Poussée (jusqu'à 2 cases) ; Résistant ; Secousse.**
- **Chasseur — Boss, <span class="rpg-token token-tn">TN</span> 12, Blessures 3, Éclaireur, Mouvement 6, Spécial : Tirage ; Éclaireur ; Salve (saut — après le mouvement).**
- **Tacticien — Boss, <span class="rpg-token token-tn">TN</span> 12, Blessures 3, Contrôleur, Mouvement 5, Spécial : Ancre (maintien pour 1 Mana/ressource par tour) ; Barrière ; Invocation (1 pion/tour jusqu'à un maximum de 3).**



---

### 1. Introduction

Hazard est un « adversaire inconscient » ou un effet environnemental. Il fonctionne par tours ou sur déclencheur.  
Format : **Nom — <span class="rpg-token token-tn">TN</span>, Effet, Comment désactiver**  
- **Tourelle — <span class="rpg-token token-tn">TN</span> 8, Effet : à chaque tour des adversaires, chaque cible dans la ligne de tir fait un test Z contre <span class="rpg-token token-tn">TN</span>, échec : −1 Cœur ; Désactivation : test M ou Z <span class="rpg-token token-tn">TN</span> 8 près du panneau.**  
- **Piège — <span class="rpg-token token-tn">TN</span> 6, Effet : entrer dans le champ impose un test Z ; échec : immobilisation ou −1 Cœur ; Désactivation : Z <span class="rpg-token token-tn">TN</span> 6 avec des outils.**  
- **Champ Répulsif — <span class="rpg-token token-tn">TN</span> 8, Effet : au début du tour, déplace de 2 cases vers le bord ; Désactivation : M <span class="rpg-token token-tn">TN</span> 8 (dispersion) ou couper l'alimentation (S <span class="rpg-token token-tn">TN</span> 6).**  
- **Gaz/Fumée — <span class="rpg-token token-tn">TN</span> 6, Effet : dans une zone de 3×3, test M ou Z ; échec : zone aveugle/−1 Cœur ; Désactivation : aération (S) ou étanchéité (Z).**



---

### 1. Introduction

Choisissez 1 de chaque ligne (ou lancez un <span class="rpg-token token-d6">d6</span>) :
1. Objectif de la scène : passage / récupération / désactivation / escorte / vol / défense
2. Terrain principal : ouvert / couloirs étroits / multi-niveaux / protections modulaires / bords dangereux / brouillard-fumée
3. Opposants : 6× pion / 4× pion + élite / 2× élite / boss / boss + 2× pion / élite + hasard
4. Avantage des opposants : couverture / hauteur / mobilité / compte à rebours / goulots d'étranglement / soutien à distance
5. Avantage des joueurs : surprise / niveau supérieur / outils / barrière courte / raccourci / allié neutre



---

### 1. Introduction

Au lieu des <span class="rpg-token token-tn">TN</span> numériques, utilisez des degrés :
- **Panneau :** « Normal » (équivalent <span class="rpg-token token-tn">TN</span> 6)
- **Élite :** « Difficile » (+1 degré)
- **Boss :** « Héroïque » (+2 degrés) et 3 Blessures
Les caractéristiques et mouvements fonctionnent de la même manière ; lorsque « <span class="rpg-token token-tn">TN</span> +1 » est mentionné dans la description, augmentez le degré.



---

### 7.2 Si le combat dure trop peu de temps

- Si le combat dure trop peu de temps : ajoutez des pions par vagues (2 par tour) ou augmentez la <span class="rpg-token token-tn">TN</span> d'un niveau pour les adversaires ayant un avantage de position.
- Si le combat s'éternise : permettez un succès exceptionnel plus souvent en créant des opportunités (meilleure position), ou abaissez la <span class="rpg-token token-tn">TN</span> pour les ennemis affaiblis.
- Deux élites ≈ petit boss ; boss + 4 pions ≈ affrontement final pour une session de 2 heures.



---

### 7.2 Garde de défense — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Artillerie, Mouvement 5, Spécial : Protection naturelle.

- **Garde Défensive — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Artillerie, Mouvement 5, Spécial : Protection Naturelle.**
- **Patrouille Mobile — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Éclaireur, Mouvement 6, Spécial : Scout.**
- **Assaut Lourd — Élite, <span class="rpg-token token-tn">TN</span> 8, Blessures 2, Brut, Mouvement 5, Spécial : Armure Légère ; Charge.**
- **Tacticien de Champ — Élite, <span class="rpg-token token-tn">TN</span> 8, Blessures 2, Contrôleur, Mouvement 5, Spécial : Ancre ; Renforcement.**
- **Leader de Champ — Boss, <span class="rpg-token token-tn">TN</span> 12, Blessures 3, Soutien, Mouvement 5, Spécial : Invocation ; Barrière ; Renforcement.**
- **Colosse Terrien — Boss, <span class="rpg-token token-tn">TN</span> 12, Blessures 3, Brut, Mouvement 5, Spécial : Dur ; Choc ; Charge.**

---
Ceci est un ensemble d'outils pour créer rapidement des ennemis. Définissez le <span class="rpg-token token-tn">TN</span>, choisissez une classe et un rôle, ajoutez 1 à 2 caractéristiques ainsi que le mouvement — et vous avez un ennemi jouable prêt pour le plateau.

