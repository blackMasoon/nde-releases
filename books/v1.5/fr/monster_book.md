---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.5
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
generated_at: "2026-01-16T08:50:46.532Z"
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
    .token-luck { background-color: #fef08a; color: #854d0e; border: 1px solid #eab308; }
    .token-power { background-color: #e9d5ff; color: #6b21a8; border: 1px solid #c084fc; }
    .token-heart { background-color: #fecaca; color: #991b1b; border: 1px solid #ef4444; }
    .token-stat { background-color: #451a03; color: #ea580c; border: 1px solid #9a3412; }
    .token-math { background-color: #1e293b; color: #38bdf8; border: 1px solid #0f172a; }
    
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

### À quoi sert ce livre

Ce livre est un ensemble d'**outils** pour créer des adversaires et des menaces dans NDE :
- rapidement (en 2 à 5 minutes),
- sans calculer de coefficients,
- d'une manière cohérente avec les règles des **Règles de base** et du **Livre du MJ**.

**La prémisse la plus importante de NDE :** *seuls les joueurs lancent les dés.*
Les adversaires ne « attaquent pas avec un jet » — ils attaquent avec **la pression dans la fiction** : ils posent des obstacles, forcent des tests, créent des menaces et des conséquences.



---

### 0. Lexique (termes dans ce livre)

- **Défense** : seuil de toucher/contourner l'adversaire lors d'un combat. Le joueur lance et compare le résultat à la Défense.
- **Difficulté (D)** : seuil d'un test contre l'environnement, un phénomène, un mouvement spécial ou un "truc" de l'ennemi.
- **Cœurs** : combien de dégâts peut encaisser une créature dans cette scène.
- **Sbire / Élite / Boss** : trois niveaux d'importance de l'adversaire dans la scène.
- **Facilitation / Complication** : changement de taille de dé du joueur d'un degré (**<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>** / vers le bas).
- **Mouvement spécial** : capacité active de l'ennemi qui change la situation (souvent oblige un test F/A/<span class="rpg-token token-stat">M</span> pour le joueur).
- **Caractéristique (passive)** : propriété constante de l'ennemi (armure, vol, résistance, zone de danger), qui donne généralement une facilitation/complication ou change l'enjeu.



---

### 1. Comment fonctionne l'adversaire dans NDE (en bref)

Dans NDE, l'adversaire est simple, mais "vivant" grâce à son comportement.

1) **Le joueur agit → le joueur lance les dés.**  
   - Attaque au corps à corps : Force (F) contre la **Défense** de la cible.  
   - Attaque à distance : Dextérité (D) contre la **Défense** de la cible.  
   - Pouvoirs : Puissance (<span class="rpg-token token-stat">P</span>) contre la **Difficulté (D)** ou contre la Défense (si c'est une attaque/incapacitation).

2) **Si le joueur rate/perd le test**, la scène continue : un coût ou une complication apparaît.  
   En combat, le coût peut signifier :  
   - perte de position,  
   - perte de temps,  
   - entrer dans une zone dangereuse,  
   - ou **cœur perdu**, si cela a du sens (par exemple, combat au corps à corps, tir croisé, zone d'impact).

3) **L'adversaire "agit" sans lancer de dés :**  
   Le MJ décrit ce que fait l'ennemi et, si cela menace réellement les héros, cela :  
   - impose un test (F/D/<span class="rpg-token token-stat">P</span>) contre la **Difficulté (D)**,  
   - ou pose une condition (« tant que… », « quand tu entres dans… », « qui est à Proximité… »),  
   - ou modifie les dés des joueurs (facilitation/difficulté).

4) **Le combat est compréhensible lorsque l'ennemi a une tactique résumée en une phrase.**  
   Chaque fiche de personnage devrait inclure : « ce que cet ennemi fait au premier tour » et « ce qu'il fait quand il prend un coup dans la figure ».  




---

### 2. Bloc de statistiques — format et champs

Un bloc de statistiques minimal contient uniquement ce qui est nécessaire dans la scène.

> **Nom — Classe, Défense, Cœurs, Rôle, Mobilité, Capacités, Mouvements, Tactique**

### 2.1 Champs obligatoires

- **Classe :** Pion | Élites | Boss  
- **Défense :** nombre qui doit être dépassé pour frapper/contourner l'ennemi.  
- **Cœurs :** combien de coups il peut encaisser (dans NDE, un « coup » équivaut par défaut à 1 Cœur).  
- **Rôle :** quelle pression il crée lors du combat (voir chapitre 4).  
- **Mobilité :** comment il se déplace (décrit en zones ; la grille est une option).  
- **Capacités (passives) :** 1 à 2 caractéristiques courtes.  
- **Mouvements (actifs) :** 1 mouvement (Élite) ou 2 à 3 mouvements (Boss).  
- **Tactique :** 1 à 3 phrases pour que le MJ dirige l'ennemi de manière cohérente.

### 2.2 Champs optionnels (à avoir si pertinent)

- **Portée :** si l'ennemi est à distance (par exemple « Loin », « Très loin »).
- **Zone :** si l'ennemi crée une zone dangereuse (fumée, feu, champ de force).
- **Faiblesse :** un « levier » clair pour les joueurs (eau, lumière UV, perturbation de signal).
- **Récompense / Indice :** ce qui reste après la défaite (butin, piste, information).
- **Variantes :** 1-2 substitutions rapides (par exemple « au lieu de vol, il a un saut » ; « au lieu de feu, il a de l'acide »).

### 2.3 Exemple de statblock (universel)

**Garde — Sbire, Défense 5, Cœurs 1, Brute, Mobilité : Près→Proche, Capacités : Bouclier, Mouvements : Poussée, Tactique : bloque le passage et pousse hors des abris.**

- **Bouclier (passif) :** tant qu'il se tient **Proche** de l'abri ou d'un porteur de bouclier, l'attaquant a un **désavantage** (dé action abaissé d'un cran).
- **Poussée (mouvement) :** si le Garde touche au corps à corps (ou si le joueur rate une attaque au corps à corps contre lui), le MJ peut pousser le héros d'une zone (Proche→Près) ou de 1-2 cases dans la variante de grille.
- **Tactique :** engage le combat avec l'adversaire le plus faible, défend le couloir, ne fuit pas.



---

### 3. Classes d'adversaires : Sbire, Élite, Boss

Dans NDE, la « difficulté » d'un adversaire se compose de deux éléments :
- **à quel point il est difficile à toucher** (Défense),
- **combien il peut encaisser** (Cœurs),
- et **quelle pression il exerce** (rôle + mouvements).

### 3.1 Sbire (minion)

- **Défense :** généralement **5** (plus facile : 4, plus difficile : 6).  
- **Cœurs :** **1** (va à terre après un coup).  
- **Mouvements :** généralement 0-1 (simple, prévisible).  
- **À quoi sert-il :** apporte du rythme, du contexte et une sensation de « combat de groupe ».  
- **Comment les diriger :** entrent en groupes de 3 à 8, meurent rapidement mais font du bruit et occupent l'espace.

> Bonne règle : un sbire a avant tout une *position* (couverture, supériorité numérique, terrain élevé), et non une « mécanique complexe ». 

### 3.2 L'Élite

- **Défense :** généralement **6** (élite plus facile : 5, "élite dure" : 8).
- **Cœurs :** **2**.
- **Actions :** 1 action caractéristique + 1 trait passif.
- **Rôle :** il est "mini-boss" dans la scène, oblige à s'adapter.

>L'élite doit faire *une chose distinctement* : « brise les défenses », "crée des zones", "saute sur les murs", "soigne les sbires".

### 3.3 Boss

- **Défense :** habituellement **8** (légendaire : 12).
- **Cœurs :** **3** (final : 5).
- **Mouvements :** 2–3 mouvements + 1–2 caractéristiques passives.
- **Pour quoi faire :** c'est une scène en soi – elle influence le terrain et le rythme.

**Un boss sans astuces est ennuyeux.** Pour qu'un boss soit « jouable », donnez-lui au moins l'un des éléments suivants :
- un mouvement qui impose un test à plusieurs héros,
- une zone (un terrain à gérer),
- ou une mécanique de « phase » (après la perte de 1 Cœur, il change de comportement).

### 3.4 « Légendaire » (niveau optionnel)

Si vous avez besoin d'un adversaire de campagne :
- **Défense 12**, **Cœurs 5**, 3-4 mouvements, zones et phases.
C'est le « boss de fin d'acte » — ne le placez pas par hasard.



---

### 4. Rôles des adversaires (pression lisible)

Les rôles existent pour que le MJ sache immédiatement « comment l'incarner ».
Le rôle n'est pas une statistique — c'est un **style de menace**.

- **Brute (coup au corps à corps) :** il s'approche de près, pousse, renverse, brise le front.
  *Question aux joueurs :* « Qui est à l'avant et quels sont les risques ? »

- **Éclaireur (mobile) :** il entre, accomplit sa tâche et s'enfuit ; il punit la solitude.
  *Question :* « Qui est séparé de l'équipe ? »

- **Artillerie (distance) :** il tire depuis des couvertures ; force les mouvements et les changements de position.
  *Question :* « Où est l'endroit sûr et où se trouve la ligne de tir ? »

- **Contrôleur (contrôle) :** zones, fumée, terrain collant, pièges, pression sur des cibles.
  *Question :* « Comment contourner la zone au lieu de se battre dedans ? »

- **Soutien (support) :** renforce, soigne, déplace, offre des protections.
  *Question :* « Qui neutraliser en premier pour simplifier le combat ? »




---

### 5. Facilités/Contraintes chez les monstres — principe de conduite

Dans NDE, **nous ne compliquons pas les chiffres**. 
Au lieu de : « +2 à la touche, -1 aux dégâts, bonus à la CA » — nous faisons :

- **facilité :** augmentez le dé du joueur d'un cran, 
- **contrainte :** abaissez le dé du joueur d'un cran, 
- **changement de mise :** le succès fonctionne, mais nécessite une autre approche (par exemple, retirer un bouclier en premier).

### 5.1 Quand changer la Défense et quand changer le dé

- **Changez le dé du joueur le plus souvent** (facilitation/difficulté).
- **Changez rarement la Défense**, principalement lorsque :
  - l'ennemi possède une « armure / invisibilité / champ de force » qui le rend *réellement* plus difficile à toucher,
  - ou lorsque c'est une mécanique de phase de boss.

### 5.2 Exemples de "désavantages" purs

- "L'ennemi est partiellement à couvert" → l'attaquant a un **désavantage**.
- "L'ennemi est étourdi / entravé" → l'attaquant a un **avantage**.
- "L'ennemi est rapide et saute sur les murs" → l'attaquant a un **désavantage** tant qu'il n'est pas bloqué.



---

### 6. Capacités passives (traits) — catalogue à assembler

Vous trouverez ci-dessous des traits que vous pouvez ajouter à une fiche technique. Choisissez-en **1–2** (boss : 2–3). Décrivez-les toujours dans le contexte du jeu.

### 6.1 Protection et robustesse

- **Armure Légère :** le premier coup dans cette scène inflige 1 Cœur de moins (donc 0) *ou* nécessite une "précision" (le succès inflige un Cœur seulement lorsque l'attaque contourne l'armure). 
  *Version la plus simple :* "le premier coup n'inflige pas de Cœur".

- **Armure Lourde :** tant que l'armure n'est pas contournée (flank, explosion, crochet, magie), les attaques ont un **handicap**. 
  *Remarque :* donnez aux joueurs un moyen clair de contourner.

- **Robuste :** après la perte de 1 Cœur, l'ennemi ne change pas de position (il ne peut pas être facilement repoussé/renversé). 
  Utile pour les colosses et les boss.

### 6.2 Mobilité

- **Rapide :** une fois par tour, peut changer de distance d'une zone supplémentaire (par exemple, Loin → Près). Dans une grille : +1–2 cases.

- **Sauteur / Grimpeur :** considère les obstacles verticaux comme normaux. Offre des "entrées raccourcies" sensées vers l'arrière.

- **Vol :** ignore les obstacles du terrain, mais nécessite des couvertures "par le haut" ou impose des tests de réaction (par exemple, Agilité, pour éviter une attaque aérienne).

### 6.3 Perception et furtivité

- **Éclaireur :** la première tentative de l'approcher par surprise a un **désavantage**.
- **Sentinelles :** si quelqu'un effectue une action bruyante dans la scène, l'ennemi change immédiatement de position pour une meilleure (se met à couvert / appelle du renfort).

### 6.4 Résistances et faiblesses (simple)

- **Résistance [type] :** la première fois dans une scène où un ennemi devrait subir un certain effet (feu, glace, psyché, électricité), l'effet est **réduit** (zone plus petite / durée plus courte / pas de perte de Cœur). 
- **Vulnérabilité [type] :** contre ce type d'attaques, le joueur a un **avantage**.

> Principe de transparence : résistance et vulnérabilité n'ont de sens que si les joueurs peuvent les découvrir et les exploiter.

### 6.5 « Nuée » et la pression du nombre

- **Nuée :** si au moins deux de ces créatures sont Proches d'un héros, le héros a un **désavantage** sur les tests de mouvement/fuite tant qu'il ne change pas de zone.



---

### 7. Mouvements actifs — comment écrire et comment conduire

Un mouvement actif doit répondre à 3 questions :
1) **Que fait-il dans la fiction ?** (description)
2) **À qui s'adresse-t-il et quand ?** (déclencheur)
3) **Comment se résout-il mécaniquement ?** (test / effet / coût)

### 7.1 Format simple de mouvement

- **Nom du mouvement :** une phrase de description.
- **Déclencheur :** quand cela se produit (par exemple, « lorsque le héros est Près », « lorsque quelqu'un tire depuis un abri »).
- **Test :** quelle caractéristique et quelle difficulté.
- **Conséquence de l'échec :** ce que vous perdez, ce qui change.
- **Conséquence du succès :** vous évitez généralement la conséquence, ou gagnez un avantage.

### 7.2 Comment déterminer la Difficulté des mouvements ennemis (sans tableaux)

Si le mouvement est « attaquant » et concerne une cible unique :
- définissez **D mouvement = Défense de l'ennemi** (c'est cohérent et facile à retenir).

Si le mouvement est de zone ou « grand » :
- définissez D un degré au-dessus de la norme de la scène (généralement **D 6** ou **D 8**).

### 7.3 Mouvements d'exemple (modules)

**Charge (Brute)**
- **Description :** l'ennemi engage et pousse.
- **Déclencheur :** lorsque l'ennemi est Proche du héros.
- **Test :** le héros effectue un test **F ou D** contre **D = Défense de l'ennemi**.
- **Échec :** le héros perd 1 Cœur *ou* est poussé d'une zone (MJ choisit ce qui est logique).
- **Succès :** évite les dégâts et maintient sa position.

**Rafale (Artillery)**
- **Description :** une série de tirs/fragments dans une zone.
- **Déclencheur :** lorsque au moins 2 héros sont dans la même zone et à découvert.
- **Test :** chaque cible effectue un test **D** contre **D 6** (ou D = Défense de l'ennemi, si l'ennemi est une élite).
- **Échec :** −1 Cœur et « tu dois te déplacer » (Proche→Éloigné).
- **Succès :** tu te caches/ne reçois rien.

**Ancrage (Controller)**
- **Description :** terrain collant, champ de force, toile, glace.
- **Déclencheur :** l'ennemi a un moment pour préparer la zone.
- **Test :** lorsque tu entres dans la zone, teste **D ou I** contre **D 5–6**.
- **Échec :** tu perds le mouvement ce tour et tu es en « mauvaise position » (désavantage pour les attaques).
- **Succès :** tu traverses ou neutralises la zone.

**Renforcement (Support)**
- **Description :** l'ennemi protège un allié/soigne/donne un avantage.
- **Déclencheur :** une fois par tour, quand un allié est menacé.
- **Effet :** l'allié choisi reçoit un « bouclier » — les attaquants ont **désavantage** jusqu'à la fin du tour, ou l'allié récupère 1 Cœur (boss/élite).
- **Riposte des joueurs :** éliminer le soutien ou le forcer à choisir (qui sauver).



---

### 8.1 Par Défaut: Zones de Distance

Dans les combats descriptifs, utilisez : **Proche / Pas loin / Loin / Très loin**. 

Dans le statblock, notez la mobilité comme suit :
- "**Mobilité :** change de zone de 1 (standard)"
- ou "**Mobilité :** Rapide (change de zone de 2)"
- ou "**Mobilité :** Vole (ignore les obstacles, mais oblige à des tests lors des attaques aériennes)".

### 8.2 Option : la grille (si votre table aime la tactique)

Si vous jouez sur une carte : - mouvement standard = **5 cases**, - Rapide = **6–7**, - Saut = 3 cases "en hauteur" ou par-dessus les obstacles. **Toutes les capacités descriptives fonctionnent de la même manière** — la grille ne fait que "donner un mètre ruban".



---

### 9. Créer un adversaire en 2 minutes (procédure)

1) **Choisir la classe** : Sbire / Élite / Boss. 
2) **Définir la Défense** : 5 / 6 / 8 (légendaire : 12). 
3) **Définir les Cœurs** : 1 / 2 / 3 (final : 5). 
4) **Choisir le rôle** : Brutal / Éclaireur / Artillerie / Contrôleur / Support. 
5) **Ajouter 1–2 traits passifs** (boss : 2–3). 
6) **Ajouter des mouvements** : Élite 1, Boss 2–3. 
7) **Écrire la tactique en 2 phrases** (premier round + réaction à une menace). 
8) (Optionnel) Ajouter une **faiblesse** et une **récompense**. 

> Test pratique : si vous pouvez diriger l’ennemi sans regarder le tableau — la fiche technique est bonne.



---

### 10. Modèles prêts à l'emploi (pour re-skinner dans chaque univers)

Les entrées suivantes sont intentionnellement « sans couleur ». Vous changez le nom et la description — la mécanique reste.

### 10.1 Subalternes

- **Gardien — Subalterne, Défense 5, Cœurs 1, Brute, Mobilité : standard, Capacités : Bouclier, Mouvements : Poussée, Tactique : bloque et repousse.**
- **Éclaireur — Subalterne, Défense 5, Cœurs 1, Skirmisher, Mobilité : Rapide, Capacités : Éclaireur, Mouvements : Évasion, Tactique : approche, marque des cibles et disparaît.**
- **Tireur — Subalterne, Défense 5, Cœurs 1, Artillerie, Mobilité : standard, Capacités : Couverture, Mouvements : Tir de couverture, Tactique : maintient à distance et force à fuir.**
- **Contrôleur — Subalterne, Défense 5, Cœurs 1, Contrôleur, Mobilité : standard, Capacités : Zone, Mouvements : Ancrage, Tactique : divise l'équipe.**
- **Soutien — Subalterne, Défense 5, Cœurs 1, Support, Mobilité : standard, Capacités : <span class="rpg-token token-stat">M</span>édecin, Mouvements : Renforcement, Tactique : protège l'élite.**

**Mouvements rapides pour les subalternes :**
- **Évasion :** lorsqu'il est touché (mais n'est pas encore "hors-jeu" dans la fiction, par exemple l'armure), il se retire d'une zone.
- **Tir de couverture :** si quelqu'un se tient à découvert, il lui donne un désavantage pour la prochaine action ("balles, éclats, peur").
- **Zone :** une fois par scène, il crée une petite zone de désavantage (fumée, huile, boue).

### 10.2 Élites

- **Costaud — Élite, Défense 6, Cœurs 2, Brute, Mobilité : standard, Capacités : Armure légère, Mouvements : Foncée, Tactique : s'approche et maintient la ligne.**
- **Assassin — Élite, Défense 6, Cœurs 2, Skirmisher, Mobilité : Rapide + Sautillant, Capacités : Éclaireur, Mouvements : Coupe de flanc, Tactique : frappe à l'arrière et se retire.**
- **Sniper — Élite, Défense 6, Cœurs 2, Artillerie, Mobilité : Lointaine, Capacités : Couverture, Mouvements : Tir sélectif, Tactique : force à bouger et punit l'absence de couverture.**
- **Manipulateur de terrain — Élite, Défense 6, Cœurs 2, Contrôleur, Mobilité : standard, Capacités : Zone (2×), Mouvements : Ancrage, Tactique : coupe la voie de fuite.**
- **Commandant — Élite, Défense 6, Cœurs 2, Support, Mobilité : standard, Capacités : Sentinelles, Mouvements : Renforcement, Tactique : renforce les alliés et les place sous couverture.**

### 10.3 Les Boss

- **Chef — Boss, Défense 8, Cœurs 3, Support, Mobilité : standard, Capacités : Sentinelles + Bouclier, Actions : Renforcement + Invocation + Barrière, Tactique : maintient le support et contrôle le rythme.**
- **Colosse — Boss, Défense 8, Cœurs 3, Brute, Mobilité : standard, Capacités : Dur + Armure Lourde, Actions : Choc + Poussée, Tactique : brise l'alignement et impose des tests.**
- **Chasseur — Boss, Défense 8, Cœurs 3, Escarmoucheur, Mobilité : Rapide + Sautillant, Capacités : Éclaireur, Actions : Embuscade + Taillade + Fuite, Tactique : isole et élimine.**
- **Architecte des Zones — Boss, Défense 8, Cœurs 3, Contrôleur, Mobilité : standard, Capacités : Zone (2×) + Résistance [type], Actions : Ancrage + Salve + Déplacement, Tactique : divise l'équipe et force à la décision.**



---

### 11. Menaces environnementales (Aléas)

Un aléa est un « adversaire sans volonté » ou un mécanisme de scène : tourelle, feu, avalanche, alarme.

**Format : Nom — Difficulté (D), Quand il agit, Effet, Comment le désactiver / contourner**

### 11.1 Exemples de dangers (universels)

**Tourelle / Drone défensif — D 6**
- **Quand ça fonctionne :** à la fin du tour, si quelqu'un est dans la ligne de tir.
- **Effet :** test **D vs D 6**; échec : -1 Cœur et vous devez vous mettre à l'abri.
- **Désactivation :** test **I ou D vs D 6** sur le panneau / brouillage / coupure d'alimentation.

**Piège / Mine / Collet — D 5**
- **Quand ça fonctionne :** lorsque vous entrez dans la zone.
- **Effet :** test **D vs D 5**; échec : -1 Cœur ou immobilisation (vous perdez votre mouvement).
- **Désactivation :** outils + test **D vs D 4–5**.

**Gaz / Fumée / Contamination — D 5**
- **Quand ça fonctionne :** au début du tour, si vous êtes dans la zone.
- **Effet :** test **<span class="rpg-token token-stat">P</span> ou I vs D 5**; échec : -1 Cœur ou pénalité aux tests pour sortie.
- **Désactivation :** ventilation, masques, étanchéité.

**Alarme / Compte à rebours — D (dépend de la scène)**
- **Quand ça fonctionne :** lorsqu'une complication survient ou que quelqu'un fait du bruit.
- **Effet :** une pression temporelle apparaît (nouvelle vague, fermeture des portes, renforts).
- **Désactivation :** test **I** (piratage/rituel) ou "physiquement" test **<span class="rpg-token token-stat">P</span>/D**.



---

### 12. Générateur de scène de combat (rapide, lisible)

Choisissez une option dans chaque ligne (ou lancez <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span>):

1) **Objectif de la scène :** passage / récupération / désactivation / escorte / vol / défense  
2) **Terrain :** ouvert / goulots d'étranglement / multi-niveau / nombreuses couvertures / bords / brouillard-fumée  
3) **Adversaires :** 6× sbire / 4× sbire + élite / 2× élite / boss / boss + 2× sbire / élite + hasard  
4) **Avantage ennemi :** couverture / hauteur / mobilité / chronomètre / embuscade / soutien à distance  
5) **Avantage des joueurs :** surprise / outils / raccourci / allié neutre / le terrain offre une couverture / information (ils savent de quel ennemi il s'agit)



---

### 13. L'équilibre en pratique (sans mathématiques)

Dans le NDE, l'équilibre est obtenu par le *rythme* et la *pression*, et non par le « CR ». 

### 13.1 Règles rapides pour définir la difficulté d'une scène

- **Scène facile :** 4–6 sbires ou 1 élite.
- **Scène standard :** 4 sbires + 1 élite, ou 2 élites.
- **Scène difficile :** boss + 2–4 sbires, ou boss + danger.
- **Finale :** boss (Cœurs 5) + élite + pression du temps.

### 13.2 Si le combat est trop court

- Envoyez une **vague de sbires** (2-3 par tour pendant 2 tours). 
- Augmentez la pression environnementale : zone de fumée, alarme, absence de couvert. 
- Changez de tactique : l'ennemi cesse de se battre "honnêtement" (se retire, prend un otage, bloque la sortie).

### 13.3 Si le combat traîne en longueur

- Donnez aux joueurs un "levier" : réservoir exposé, panneau, rituel, faiblesse.
- Accordez des **bénéfices pour un succès exceptionnel** : briser une couverture, désarmer, disperser les renforts.
- Réduisez les Cœurs du boss de 5 à 3, si ce n'est pas la finale.



---

### 14. Reskin : comment adapter un ennemi pour chaque univers

Vous avez la fiche de statistiques "Éclaireur". Maintenant, changez seulement la description :

- **Fantasy :** archer gobelin éclaireur (Éclaireur + Tir).  
- **Science-fiction :** drone de reconnaissance (Éclaireur + Capteurs).  
- **Cyberpunk :** éclaireur de gang en skateboard (Rapide + Fuite).  
- **Slave :** démon traqueur de traces (Vulnérabilité : fer; Résistance : peur).

La mécanique reste la même. Cela permet à la communauté d'ajouter des centaines d'entrées sans perturber la cohérence du noyau.

