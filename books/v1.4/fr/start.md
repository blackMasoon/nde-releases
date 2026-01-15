---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.4
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
generated_at: "2026-01-15T07:57:22.409Z"
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
# Règles en bref

Automatic translation placeholder for fr

---



---

### 1) Héros en 1 minute


* **Concept :** qui es-tu et dans quel genre joues-tu (1 phrase).
* **Rôle (choisis-en un) :**

  * **Assaut** – pression, combat, franchissement d'obstacles
  * **Spécialiste** – discrétion, précision, technique, observation
  * **Adepte** – pouvoirs, connaissance, influence, improvisation
* **Caractéristiques (3) :**

  * **Force (F)** – force physique, endurance, combat rapproché
  * **Agilité (A)** – réflexes, discrétion, tir, pilotage
  * **Pouvoir (<span class="rpg-token token-stat">P</span>)** – magie/psychokinésie/technologie/bluff/intuition (selon le monde)
* **Dés de caractéristiques :** une caractéristique **<span class="rpg-token token-d12">k12</span>**, une **<span class="rpg-token token-d8">k8</span>**, une **<span class="rpg-token token-d6">k6</span>** (choisis selon le rôle).
* **Cœurs :** 5. **Points de Pouvoir :** 3 (tu les dépenses pour des pouvoirs et des « actions spéciales »).
Voici un extrait prêt à être collé (variante A), dans le style des règles courtes « 1-page ».

**Jet de Chance (comment ça fonctionne) :** dépense **1 JP**, pour choisir une des options suivantes :

* **Relance** de ton test (tu gardes le meilleur résultat), ou
* **Augmentation du dé d'un niveau** pour ce jet unique (**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>**), ou
* **Transformation d'un échec en « succès avec coût »** — l'action réussit, mais le MJ impose immédiatement un prix (par exemple, tu perds du temps, fais du bruit, utilises une ressource, finis dans une position moins favorable, attires l'attention, abîmes du matériel).

**Récupération de JP :** au début de la prochaine session, tu reviens à la limite. Le MJ peut accorder **+1 JP** pour un risque audacieux, une excellente décision narrative ou le jeu des conséquences.

* **Équipement :** 1 outil « clé » (par exemple, épée, fusil, kit de hacking), 1 protection (armure, bouclier énergétique, camouflage), 3 bricoles correspondant au concept.

**Exemple :** Spécialiste : F <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">P</span> <span class="rpg-token token-d8">k8</span>, A <span class="rpg-token token-d6">k6</span>. Dans un univers cyberpunk, <span class="rpg-token token-stat">P</span> est « Hacking/Influence » ; dans un univers fantastique, <span class="rpg-token token-stat">P</span> est « Magie/Volonté ».



---

### 2) Comment résoudre les actions

1. Le joueur dit **ce qu'il fait** et **comment** (description dans le monde du jeu).
2. Le meneur de jeu détermine la **Difficulté** et l'enjeu ("que se passera-t-il en cas d'échec").
3. Lance le dé de caractéristique (D/I/C) et compare avec la Difficulté.

**Difficulté (D) :**

* **3** facile, **4** standard, **5** difficile, **6** très difficile, **8** héroïque, **12** légendaire.

**Résultat du lancer :**

* **1** – échec avec conséquence (la complication se produit à coup sûr).
* **< D** – échec (mais la scène continue : perte de temps, bruit, position moins favorable, perte de ressource).
* **≥ D** – succès.
* **Max sur le dé** (par exemple, 12 sur <span class="rpg-token token-d12">k12</span>, 20 sur <span class="rpg-token token-d20">k20</span>) – succès exceptionnel : vous obtenez un avantage supplémentaire.

**Modificateurs sans compter :**

* **Meilleure situation** : augmentez le dé d'un niveau (<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>).
* **Pire situation** : réduisez le dé d'un niveau (<span class="rpg-token token-d20">k20</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d4">k4</span>).
* **Aide d'un allié** (coûte son action) : augmentez le dé d'un niveau.

**Exemple :** L'adepte essaie de fermer le portail (D <span class="rpg-token token-d8">k8</span>) sous alarme et stress → pire situation, passe à <span class="rpg-token token-d6">k6</span>. D = 5. Lancer 6 : succès, mais "l'alarme" reste en arrière-plan comme pression narrative.



---

### 3) Mouvement et combat – par défaut sans grille, grille en option

**Par défaut : théâtre de l'esprit (recommandé)**

* Décrivez les distances comme : **Proche** (à portée de main), **Pas loin** (quelques pas), **Loin** (de l'autre côté de la scène), **Très loin** (sniper/véhicule).
* À votre tour, vous avez : **Déplacement + 1 Action**.

  * Le déplacement change généralement la distance d'1 « degré » (Pas loin → Proche, etc.).
* **Attaque** : jet **<span class="rpg-token token-stat">M</span>** (corps à corps) ou **D** (distance) contre **Défense** de la cible.

**Défense des adversaires (indicatif) :**

* **Faible** 4, **Typique** 5, **Elite** 6, **Boss** 8 (boss légendaire 12).

**Effets d'un coup (combat rapide) :**

* Un coup inflige **1 Cœur**.
* Un succès exceptionnel inflige **2 Cœurs** ou donne un effet fort (désarmement, renversement, dispersion).

**Couverture et avantage positionnel :**

* Couverture légère / mauvais angle : abaissez le dé de l'attaquant d'1 degré.
* Bonne position / surprise : augmentez le dé d'1 degré.

**Option : jeu sur grille**

* 1 case = 1–2 m. Mouvement par tour : **jusqu'à 5 cases**. Le reste des règles reste inchangé.

**Exemple :** Un spécialiste tire depuis une couverture (D sur un <span class="rpg-token token-d12">d12</span>) sur une élite (Défense 6). La cible est en légère couverture → D tombe à un <span class="rpg-token token-d8">d8</span>. Jet 7 : succès, 1 Cœur de dégâts.



---

### 4) Pouvoirs, « sorts » et actions spéciales (universels)


Cela inclut la magie, la psionique, la cybernétique, les gadgets, les tours de magie – selon le monde.

* Lorsque vous faites quelque chose **au-delà de la norme** : dépensez **un Point de Pouvoir** et lancez **<span class="rpg-token token-stat">M</span>**.
* Déterminez le niveau de l'effet :

**Niveaux de puissance (T / coût) :**

* **Tour** (effet court, astuce, « flash ») : **T 4 / 0–1 PP**
* **Standard** (attaque, bouclier, impulsion, contrôle mineur) : **T 5 / 1 PP**
* **Fort** (zone, guérison, paralysie, hack « en direct ») : **T 6 / 2 PP**
* **Grand** (changement de scène, intervention puissante) : **T 8–12 / 3 PP**

**Échec :** Les PP sont perdus, et la conséquence est immédiate (surcharge, trace numérique, fissure dans le rituel, attention indésirable).

**Récupération :** après la scène de conflit, vous récupérez **1 PP**, après un repos en sécurité – jusqu'à plein.

**Exemple :** Dans une opération spatiale, l'Adept essaie de « plier le capteur » d'un drone : Standard, T 5, coût 1 PP. Lancer <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span> = 8 : succès exceptionnel – le drone perd le signal et se trompe de piste.



---

### 5) Chute, risque et guérison

* Lorsque vous tombez à **0 Cœurs**, vous êtes **hors de l'action** (blessé, étourdi, en état de choc – selon la convention).
* Un allié peut utiliser une action pour vous remettre à **1 Cœur** (premiers secours, adrénaline, redémarrage du système).
* Après la scène, si vous avez un moment de répit : vous revenez à **Cœurs pleins**, tant que vous avez les conditions nécessaires (abri, bandage, service, repas).
* Si la scène a été particulièrement brutale ou si les ennemis ont l'avantage, le Maître de Jeu peut exiger qu'un « réinitialisation complète » nécessite un arrêt en toute sécurité.

**Exemple :** L'assaut tombe à 0. Le spécialiste le tire derrière une couverture et utilise une action : l'assaut revient à 1 Cœur et peut agir au tour suivant.



---

### 6) Développement du personnage (campagne sans tableaux ni comptabilité)


Après l'aventure, choisis **une** option :

* **Augmente** une caractéristique de 1 niveau (max. jusqu'à <span class="rpg-token token-d20">k20</span>), ou
* **+1 Cœur** (max. 7), ou
* **+1 Point de Pouvoir** (max. 5), ou
* **Nouvel Avantage** (règle courte, en une phrase convenue avec le Maître de Jeu).

**Exemples d'avantages (universels) :**

* **Pression :** une fois par scène, lorsque tu touches au corps à corps, tu infliges +1 Cœur de dégâts.
* **Ombre :** lorsque tu agis dans l'ombre, tu as un bonus de dés de 1 niveau.
* **Étincelle :** une fois par scène, tu peux dépenser 1 <span class="rpg-token token-power">PM</span> pour obtenir automatiquement un « succès avec coût » sans lancer de dé.

**Exemple :** L'Adepte augmente <span class="rpg-token token-stat">M</span> de <span class="rpg-token token-d8">k8</span> à <span class="rpg-token token-d12">k12</span> – maintenant ses pouvoirs se stabilisent mieux avec T 5–6.



---

### 7) Variante « uniquement <span class="rpg-token token-d6">k6</span> » en mode **2k6** (rapide et très jouable)


Si vous n'avez pas de jeu de dés ou si vous souhaitez des degrés de résultat plus « narratifs » :

* Chaque test est : **lancez 2k6 + modificateur de caractéristique**.
* **Modificateurs de caractéristiques** à choisir au départ : une caractéristique **+2**, une **+1**, une **+0**.
* Résultat :

  * **6 ou moins** – échec avec conséquence
  * **7–9** – succès avec coût (compromis, perte de ressource, position défavorable)
  * **10+** – succès complet
  * **12** – succès exceptionnel (avantage supplémentaire)

**Difficulté de la situation :** au lieu de changer les seuils, ajoutez **+1 / -1** au lancer (facilite / complique) ou un coût en cas de 7–9.

**Mapping vers la version dés-caractéristiques (si vous souhaitez la compatibilité) :**

* <span class="rpg-token token-d6">k6</span> ≈ +0, <span class="rpg-token token-d8">k8</span> ≈ +1, <span class="rpg-token token-d12">k12</span> ≈ +2, <span class="rpg-token token-d20">k20</span> ≈ +3 (pour des personnages très expérimentés).

**Exemple :** Un spécialiste tire en courant : <span class="rpg-token token-stat">Z</span> = +2, situation difficile (-1). Lancer 2k6 = 8, somme 9 : succès avec coût – il touche, mais finit en position exposée.

