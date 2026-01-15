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
generated_at: "2026-01-15T08:02:46.318Z"
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
# Livre des Règles de Base



---



---

### Choses nécessaires pour jouer

- Crayon et fiche de personnage.
- (Optionnel) carte/grille à carreaux et marqueurs de personnage (papier à carreaux, tapis, VTT).
- Dés : **<span class="rpg-token token-d4">k4</span>, <span class="rpg-token token-d6">k6</span>, <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-d20">k20</span>**.
  - En pratique, il suffit d'**un de chaque** (on lance un dé à la fois).
  - (Optionnel) **k100** pour les tables aléatoires ou les générateurs.
- Si vous n'avez que **<span class="rpg-token token-d6">k6</span>**, utilisez la variante **2k6** (à la fin).

---



---

### Glossaire des termes


Ces mots apparaissent dans les règles — voici leur explication « en termes simples » :

- **MJ (Maître de Jeu)** : dirige le monde, décrit les situations, contrôle les adversaires, détermine la Difficulté et les conséquences.
- **Joueur** : décrit les actions de son personnage et effectue des jets.
- **Test** : un jet de dés qui détermine un résultat incertain.
- **Caractéristiques** : **Force (F)**, **Agilité (A)**, **Pouvoir (<span class="rpg-token token-stat">P</span>)**. Indiquent *quel dé vous lancez*.
- **Dé de caractéristique** : la taille du dé attribuée à une caractéristique (par exemple, A = <span class="rpg-token token-d12">d12</span>).
- **Difficulté (D)** : le nombre à atteindre ou à dépasser pour que l'action réussisse.
- **Succès** : résultat ≥ Difficulté.
- **Succès exceptionnel** : **résultat maximal** sur le dé (par exemple, 12 sur <span class="rpg-token token-d12">d12</span>, 20 sur <span class="rpg-token token-d20">d20</span>) — succès + avantage supplémentaire.
- **Complication** : problème supplémentaire après un échec (bruit, perte de temps, position défavorable, perte de ressource).
- **Succès à coût** : l'action réussit, mais vous payez le prix (compromis, perte de ressource, révélation, risque).
- **Coup de Chance (CC)** : ressource limitée qui permet de sauver des scènes (relance / augmentation de dé / transformation d'un échec en succès à coût).
- **Cœurs** : « vie » du personnage (endurance, blessures, condition — selon le monde).
- **Points de Pouvoir (PP)** : ressource pour des pouvoirs et des actions « au-delà de la norme » (magie, psionique, gadgets, actions « cinématographiques »).
- **Défense** : seuil pour toucher un adversaire en combat (au lieu de multiplier les règles sur l'armure, la classe d'armure, etc.).
- **Couverture** : obstacle entre vous et la cible. Généralement, cela complique les attaques à distance ou les actions d'observation.

---



---

### 1. Personnage


Tworzenie postaci jest krótkie. Postać to: **concept + rôle + caractéristiques + ressources + équipement**.

---

### 1.1 Concept

Jedno zdanie: kim jesteś i w jakim gatunku grasz.

> Przykład: „Była agentka korporacji, dziś łowczyni nagród, która działa po cichu i nie ufa nikomu.”

### 1.2 Rôle (choisissez-en un)


Rôles sont délibérément « neutres par rapport au monde ». Dans un univers fantastique, vous pouvez les appeler autrement, dans un univers cyberpunk autrement, mais ils fonctionnent de la même manière.

- **Assaut** — pression, combat, franchissement d'obstacles, percement de front.
- **Spécialiste** — furtivité, précision, technique, observation, plan.
- **Adepte** — pouvoirs, influence, connaissance, improvisation (magie/psychique/technologie selon le monde).

### 1.3 Caractéristiques et dés


Vous avez trois caractéristiques :

- **Force (F)** — force physique, endurance, combat rapproché, effort.
- **Agilité (A)** — réflexes, précision, discrétion, tir, conduite.
- **Pouvoir (<span class="rpg-token token-stat">P</span>)** — « ce qui est spécial » : magie, psionique, technologie avancée, bluff social, intuition — selon la convention.

**Au départ, répartissez les dés comme suit :**
- une caractéristique a **<span class="rpg-token token-d12">k12</span>**,
- une a **<span class="rpg-token token-d8">k8</span>**,
- une a **<span class="rpg-token token-d6">k6</span>**.

**Répartition suggérée selon le rôle (le plus simple) :**
- **Assaut :** F <span class="rpg-token token-d12">k12</span>, A <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-stat">P</span> <span class="rpg-token token-d6">k6</span>
- **Spécialiste :** A <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">P</span> <span class="rpg-token token-d8">k8</span>, F <span class="rpg-token token-d6">k6</span>
- **Adepte :** <span class="rpg-token token-stat">P</span> <span class="rpg-token token-d12">k12</span>, A <span class="rpg-token token-d8">k8</span>, F <span class="rpg-token token-d6">k6</span>

> Exemple : si vous avez A = <span class="rpg-token token-d12">k12</span>, alors lors d'un tir, d'une discrétion et d'esquives, vous lancez généralement <span class="rpg-token token-d12">k12</span>.

### 1.4 Ressources

- **Cœurs :** 5.
- **Points de Pouvoir (PP) :** 3.
- **Coup de Chance (CC) :** au début de chaque session, tu as **2 CC**.

**Coup de Chance (comment ça fonctionne) :** dépense **1 CC** pour choisir l'une des options suivantes :
- **Relance** de ton test (tu gardes le meilleur résultat), ou
- **Augmentation du dé d'un niveau** pour ce lancer unique (**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>**), ou
- **Transformation d'un échec en « succès avec coût »** — l'action réussit, mais le MJ impose immédiatement un coût (par exemple : bruit, perte de temps, perte de ressource, position défavorable, attirer l'attention, endommagement de l'équipement).

**Récupération de CC :** au début de la prochaine session, tu reviens à la limite. Le MJ peut accorder **+1 CC** pour un risque audacieux, une excellente décision narrative ou le jeu des conséquences.

### 1.5 Talents (optionnels, mais recommandés)

Les talents sont **2 courtes phrases** qui décrivent dans quoi votre personnage excelle (sans liste, sans tableau).

- Exemples : « <span class="rpg-token token-stat">M</span>écanicien », « Éclaireur », « Négociateur », « <span class="rpg-token token-stat">M</span>édecin », « Hacker », « Vétéran », « Explorateur ».

**Comment fonctionnent les Talents :** si un Talent aide réellement lors d'un test, le MJ peut **augmenter le dé d'1 niveau** (ou neutraliser une difficulté).
- Un Talent ne garantit pas de succès automatiques.
- En général, **maximum 1 Talent** influence un test.

### 1.6 Équipement

Énumérez :
- 1 outil « clé » (arme / ensemble / équipement sans lequel vous ne pouvez pas faire votre travail),
- 1 protection (armure, bouclier, camouflage — selon le monde),
- 3 bricoles utiles dans l'aventure.

L'équipement dans le cœur des règles est principalement **une autorisation** (permet des actions), et non un bonus numérique.

### 1.7 Exemple de personnage complet

- Concept : « Une voleuse d'informations qui dérobe des données des systèmes, et non des poches. »
- Rôle : Spécialiste
- Caractéristiques : <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">k6</span>, <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span>
- Ressources : 5 Cœurs, 3 <span class="rpg-token token-power">PM</span>, 2 LS
- Talents : « Hacker », « Ombre »
- Équipement : pistolet, armure légère, kit de cambriolage, corde, lampe torche

---



---

### 2. Noyau des règles : tests

Cette partie est la plus importante — si vous la comprenez, vous comprenez le système.

### 2.1 Quand tu fais un test

Tu fais un test lorsque les deux conditions suivantes sont remplies :
1) le résultat est incertain (cela peut réussir ou non), et
2) l'enjeu est réel (un échec change quelque chose / coûte quelque chose).

Si l'action est banale et sans pression — le MJ peut dire "réussi" sans lancer de dés.

### 2.2 Comment effectuer un test (étape par étape)

1) Le joueur dit **ce qu'il fait** et **pourquoi**.
2) Le MJ choisit une caractéristique : **<span class="rpg-token token-stat">S</span>** ou **<span class="rpg-token token-stat">Z</span>** ou **<span class="rpg-token token-stat">M</span>**.
3) Le MJ détermine la **Difficulté (D)** et explique ce que signifie un échec (mise).
4) Le joueur lance **le dé de caractéristique**.
5) Comparez le résultat avec D et déterminez les conséquences.

### 2.3 Difficultés (T)


Nous utilisons des seuils simples. Si vous avez un doute, choisissez un seuil inférieur, et la « difficulté » se montrera par les conséquences.

- **T 3** – facile (presque sûr, mais parfois il vaut mieux vérifier sous pression)
- **T 4** – standard (défi typique)
- **T 5** – difficile (nécessite des compétences ou un avantage)
- **T 6** – très difficile (sans avantage, c'est risqué)
- **T 8** – héroïque (pour les meilleurs ou après une bonne préparation)
- **T 12** – légendaire (rarement « à la propre » ; généralement comme objectif de campagne, plan, rituel, grandes conditions)

### 2.4 Résultats du test

- **Résultat ≥ T → Succès.** Vous atteignez l'effet désiré.
- **Résultat < T → Échec.** Vous n'atteignez pas l'effet, et la situation change (complication ou coût).
- **Lancer un 1 → Échec + complication.** La complication se produit à coup sûr.
- **Résultat maximal sur les dés → Succès exceptionnel.**
  - En plus du succès, vous obtenez un **avantage supplémentaire** (plus rapidement, plus silencieusement, plus fortement, plus sûrement, effet supplémentaire).

> Exemple de succès avec coût : « Vous parvenez à forcer la porte, mais vous faites du bruit et quelqu'un vient vérifier. »

### 2.5 Facilités et obstacles (sans comptage)


Au lieu d'ajouter +1/−1 aux jets, nous changeons la **taille des dés**.

- **Meilleure situation** → **augmente le dé d'un niveau**  
  <span class="rpg-token token-d6">k6</span> → <span class="rpg-token token-d8">k8</span> → <span class="rpg-token token-d12">k12</span> → <span class="rpg-token token-d20">k20</span>
- **Pire situation** → **diminue le dé d'un niveau**  
  <span class="rpg-token token-d20">k20</span> → <span class="rpg-token token-d12">k12</span> → <span class="rpg-token token-d8">k8</span> → <span class="rpg-token token-d6">k6</span> → <span class="rpg-token token-d4">k4</span>

**Exemples de facilités :** préparation, bons outils, avantage de position, surprise, soutien.  
**Exemples d'obstacles :** obscurité, glissant, pression du temps, bruit, distraction, couverture.

**Règle de l'ordre :** pour la rapidité, supposez qu'à un seul test vous appliquez généralement **au maximum 1 facilité et 1 obstacle** (ils peuvent s'annuler).

### 2.6 Aide d'un allié

Un allié peut consacrer son action (ou du temps dans une scène en dehors du combat) pour aider.

**Effet :** pour ce seul test, **augmente le dé d'un niveau**.

L'aide doit être décrite de manière sensée (protection, fourniture d'outils, diversion, stabilisation, conseils).

### 2.7 Répétition des tests


Si le test a échoué, ne le répétez pas « à l'infini » sans changer la situation.
- Soit vous faites quelque chose différemment (une autre caractéristique / d'autres outils / un autre chemin),
- soit vous acceptez le coût (temps, alarme, ressource),
- soit vous vous retirez.

### 2.8 Exemples de tests (hors combat)

**Exemple A — passage silencieux**
- Joueur : « Je vais traverser la cour avant que le projecteur ne revienne. »
- MJ : Agilité (A). C'est sous pression temporelle → Difficulté **D 5**.
- Le personnage a le Talent « Ombre » → avantage, le dé est augmenté d'un niveau.
- Lancer : <span class="rpg-token token-d12">D12</span> = 4 → échec. MJ : « Ils ne te remarquent pas tout de suite, mais quelqu'un entend un bruit et commence à vérifier la zone (complication : la pression augmente). »

**Exemple B — forçage à la force**
- Joueur : « Je vais forcer la porte en métal avant que la sécurité n'atteigne le coin. »
- MJ : Force (F), Difficulté **D 6** (très difficile sans outils).
- Quelqu'un aide en maintenant la serrure et en coinçant la porte → le dé est augmenté d'un niveau.
- Lancer : F <span class="rpg-token token-d12">D12</span> = 12 → succès exceptionnel : la porte s'ouvre immédiatement et tu le fais plus silencieusement que prévu.



---

### 3. Mouvement et distances (la grille est une option)

Par défaut, le NDE fonctionne sans carte : vous décrivez la scène et les positions des personnages.

### 3.1 Par défaut : distances descriptives


Utilisez quatre zones :
- **Près** — à portée de main, combat au corps à corps.
- **Pas loin** — quelques pas, approche facile.
- **Loin** — de l'autre côté de la scène, nécessite un déplacement clair.
- **Très loin** — de manière snipériste/avec véhicule/« à la limite de la scène ».

Lors d'un tour, vous pouvez généralement changer la distance de **une zone** (par exemple, Loin → Pas loin).


### 3.2 Option : jeu sur grille (pour la tactique)


Si vous préférez des détails concrets :
- 1 case = 1–2 m.
- Mouvement par tour : **jusqu'à 5 cases**.
- Les diagonales sont autorisées (comptent comme une case normale).


### 3.3 Couverture et ligne d'action

- **Couverture totale :** il est impossible d'interagir « en ligne » (tir, observation, plusieurs pouvoirs).
- **Couverture partielle :** complique — généralement **diminue le dé d'un niveau** pour l'attaquant/l'observateur.

---



---

### 4. Combat

Le combat est une scène ordinaire avec des tests, simplement organisée en tours.

### 4.1 Quand commence le combat

Le combat commence lorsque :
- au moins une des parties souhaite nuire à l'autre, et
- il est important de savoir qui agit et quand.

Si la situation est brève et évidente, le MJ peut la résoudre par un seul test.

### 4.2 Ordre des tours (version simple)


Le plus simple :
- D'abord, tous les joueurs agissent (dans n'importe quel ordre),
- ensuite, les ennemis agissent,
- et ainsi de suite en boucle.

### 4.3 Que fais-tu pendant ton tour


Dans ton tour, tu as :
- **Déplacement** (changement de zone / jusqu'à 5 cases dans la variante grille),
- **1 Action** (attaque, test, aide, utilisation de pouvoir, équipement, interaction avec la scène).


### 4.4 Attaque : comment ça fonctionne

1) Choisissez une cible et décrivez l'attaque.
2) Choisissez une caractéristique :
   - **corps à corps** → jet de **Force (F)**,
   - **distance** → jet de **Dextérité (D)**,
   - **pouvoirs** → généralement jet de **Pouvoir (<span class="rpg-token token-stat">P</span>)** (voir chapitre 5).
3) Déterminez la **Défense** de la cible.
4) Lancez le dé et comparez avec la Défense.

### 4.6 Dommages et « combien ils en supportent »

- Une touche inflige **1 Cœur**.
- **Succès exceptionnel** inflige **2 Cœurs** *ou* donne un effet puissant (désarmement, renversement, poussée hors de la couverture) — choisissez-en un.

Archétypes les plus simples d'ennemis :
- **<span class="rpg-token token-stat">P</span>éon :** tombe après 1 touche.
- **Élite :** a **2 Cœurs**.
- **Boss :** a **3 Cœurs** (ou 5 dans les scènes finales).

> Remarque : « tomber » ne doit pas nécessairement signifier la mort. Il peut être inconscient, avoir fui, s'être rendu, ou avoir été mis hors d'action.

### 4.5 Défense des adversaires (indicatif)

- **Faible :** Défense **4**
- **Typique :** Défense **5**
- **Élite :** Défense **6**
- **Boss :** Défense **8** (boss légendaire : **12**)

La couverture et les conditions modifient généralement la taille des dés de l'attaquant (facilités/difficultés), et non la Défense.

### 5.7 Portée des attaques (par défaut)
Pour ne pas multiplier les chiffres, utilisez des règles simples :
- À portée : cible sur la case adjacente.
- Distance : cible dans « le champ de vision » sur le plateau.
  - Si le MJ souhaite une restriction : considérez **jusqu'à 10 cases** sans malus ; au-delà de 10 cases, <span class="rpg-token token-<span class="rpg-token token-math">tn</span>"><span class="rpg-token token-math">TN</span></span> +1 degré.

### 5.8 Plusieurs adversaires à la fois
Si plusieurs pions sont « au contact » d'un personnage, le MJ peut :
- augmenter la <span class="rpg-token token-<span class="rpg-token token-math">tn</span>"><span class="rpg-token token-math">TN</span></span> d'un niveau (pression), ou
- considérer que l'échec entraîne une complication supplémentaire (par exemple, vous perdez votre position).

La règle doit être rapide : **une résolution → un effet**.

### 4.7 Exemples de combat

**Exemple A — combat rapproché avec un garde**
- L'assaut (D <span class="rpg-token token-d12">k12</span>) attaque le garde (Défense 5).
- Les conditions sont bonnes (surprise) → le dé est augmenté d'un niveau, mais c'est déjà un <span class="rpg-token token-d12">k12</span>, donc l'augmentation donne un <span class="rpg-token token-d20">k20</span>.
- Lancer <span class="rpg-token token-d20">k20</span> = 7 → touche, le garde tombe.

**Exemple B — tir sur l'élite depuis un abri**
- Le spécialiste (D <span class="rpg-token token-d12">k12</span>) tire sur l'élite (Défense 6).
- La cible est partiellement à couvert → difficulté, le dé passe à <span class="rpg-token token-d8">k8</span>.
- Lancer <span class="rpg-token token-d8">k8</span> = 6 → touche, l'élite perd 1 Cœur (il lui en reste 1).

**Exemple C — boss et Coup de Chance**
- L'adepte (<span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">k12</span>) essaie de neutraliser le boss (Défense 8) avec sa puissance.
- Lancer <span class="rpg-token token-d12">k12</span> = 4 → échec. Le joueur dépense 1 CC pour relancer.
- Relance = 10 → succès. Le boss perd 1 Cœur, mais le MJ ajoute un coût : « l'effet est bruyant, une alarme se déclenche. »



---

### 5. Pouvoirs (<span class="rpg-token token-stat">P</span>) et Points de Pouvoir (PP)

Dans le NDE, le "Pouvoir" est une catégorie d'effets spéciaux. Selon le monde, cela peut signifier :
- magie, psionique, rituels,
- technologie avancée, drones, hacking "en direct",
- actions cinématographiques des héros (par exemple, "concentration maîtrisée"),
- influence sociale dans les jeux où la conversation est "un pouvoir".

### 5.1 Quand tu dépenses des <span class="rpg-token token-power">PM</span>

Tu dépenses des <span class="rpg-token token-power">PM</span> lorsque tu essaies d'obtenir un effet **au-dessus de la norme**.

---

### 5.2 Comment utiliser les pouvoirs (étape par étape)

1) Décris l'effet que tu souhaites obtenir.
2) Le MJ détermine la Difficulté et le coût en <span class="rpg-token token-power">PM</span>.
3) Dépense des <span class="rpg-token token-power">PM</span>.
4) Lance **<span class="rpg-token token-stat">M</span>** et compare avec la Difficulté.

**Échec :** l'effet ne fonctionne pas ; les <span class="rpg-token token-power">PM</span> sont perdus ; une complication survient (surcharge, trace, révélation, effet secondaire).

### 5.3 Niveaux d'effets (Difficulté / coût)

- **Astuce** (truc court) : **D 4 / 0–1 <span class="rpg-token token-power">PM</span>**  
  lumière, son, petit rideau, distraction temporaire.
- **Standard** : **D 5 / 1 <span class="rpg-token token-power">PM</span>**  
  projectile, bouclier, impulsion, saut, renforcement.
- **Fort** : **D 6 / 2 <span class="rpg-token token-power">PM</span>**  
  zone, contrôle, guérison, paralysie, « hack en combat ».
- **Grand** : **D 8–12 / 3 <span class="rpg-token token-power">PM</span>**  
  effet qui change la scène ou a des conséquences sur la campagne.

### 5.4 Succès exceptionnel en puissance

Si vous obtenez un maximum sur le dé <span class="rpg-token token-stat">M</span> :
- augmentez l'échelle (plus grande zone / plus longtemps / plus fort), ou
- ajoutez un avantage supplémentaire (plus silencieusement, plus précisément, plus en sécurité), ou
- le MJ peut rendre **1 <span class="rpg-token token-power">PM</span>** (si cela correspond à la fiction).

### 5.5 Récupération de <span class="rpg-token token-power">PM</span>

- Après une scène de conflit, tu récupères **1 <span class="rpg-token token-power">PM</span>**.
- Après un repos en toute sécurité, tu retrouves tes pleines capacités.

### 5.6 Exemples de pouvoirs

**Exemple A — bouclier pour courir**
- Joueur : « Je place une courte protection pour courir vers une meilleure position. »
- MJ : Standard **D 5**, coût 1 <span class="rpg-token token-power">PM</span>.
- Lancer <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">d12</span> = 9 → succès : tu cours en toute sécurité.

**Exemple B — échec avec conséquence**
- Joueur : « J'immobilise l'élite sur place. »
- MJ : Fort **D 6**, coût 2 <span class="rpg-token token-power">PM</span>.
- Lancer = 1 → échec + complication : tu perds 2 <span class="rpg-token token-power">PM</span>, et l'effet rebondit et révèle ta position.



---

### 6.1 0 Coeurs

Si vous tombez à 0 Coeurs :
- vous êtes **hors de combat** (blessé, assommé, en état de choc — selon la convention),
- un allié peut consacrer une action pour vous remettre sur pied avec **1 Coeur**.

### 6.2 Repos

- Après une scène de conflit, si vous avez un moment de répit et des conditions de base, vous pouvez revenir à des Cœurs pleins.
- Dans des campagnes plus strictes, le MJ peut exiger un arrêt en sécurité pour revenir à la plénitude.

### 7.3 Repos
Après une scène de combat/conflit, si vous avez un moment de repos en toute sécurité (et des conditions de base), vous revenez à pleine capacité :
- de Cœur,
- de Mana.

Cela permet de garder le système rapide et ne nécessite pas de longues périodes de guérison.



---

### 7. Développement du personnage

**Quand tu grandis :** après une aventure, une mission ou un chapitre important de l'histoire (généralement tous les 1 à 3 sessions).

Choisis **une** option :
- **Augmente** une caractéristique de 1 niveau de dés (max. jusqu'à <span class="rpg-token token-d20">k20</span>), ou
- **+1 Coeur** (max. 7), ou
- **+1 <span class="rpg-token token-power">PM</span>** (max. 5), ou
- **Nouvel Avantage** (une capacité spécifique convenue avec le MJ).

> Exemple : Le spécialiste augmente <span class="rpg-token token-stat">Z</span> de <span class="rpg-token token-d12">k12</span> à <span class="rpg-token token-d20">k20</span>, car la campagne est entrée dans une phase de poursuites et de fusillades.

---



---

### 8. Variante uniquement <span class="rpg-token token-d6">k6</span> : 2k6

Si vous ne souhaitez pas utiliser différents dés, jouez avec **2k6**.

### 8.1 Caractéristiques en tant que modificateurs


Au lieu des tailles de dés, sépare les modificateurs :
- une caractéristique a **+2**
- une a **+1**
- une a **+0**


### 8.2 Test

**Lancez **2d6 + modificateur de caractéristique**.

**Résultat :**
- **6 ou moins** – échec avec conséquence
- **7–9** – succès avec coût
- **10+** – succès complet
- **12** – succès exceptionnel (avantage supplémentaire)

### 8.3 Difficulté de la situation

Au lieu de modifier les seuils, donne :
- **+1** pour l'avantage, la préparation, un bon plan,
- **−1** pour les obstacles, la pression, la couverture, le chaos.

### 8.4 Coup de Chance en 2d6

Dépenser 1 CC pour :
- relancer 2d6, ou
- ajouter **+1** au résultat du test, ou
- transformer un échec en succès avec un coût.

### 8.5 Cartographie rapide (optionnelle)

Si jamais vous souhaitez "recalculer" un personnage entre les variantes :
- <span class="rpg-token token-d6">k6</span> ≈ +0
- <span class="rpg-token token-d8">k8</span> ≈ +1
- <span class="rpg-token token-d12">k12</span> ≈ +2
- <span class="rpg-token token-d20">k20</span> ≈ +3 (pour les très expérimentés)

---



---

[FR] Contenu à venir...




---

### 1. Introduction

7.2 Ces ajouts ne sont pas obligatoires, mais ils facilitent parfois la gestion.

### 9.1 Protection (armour) as a simple resource


Si vous souhaitez que la « protection » ait un effet clair :
- le personnage avec protection a **1 jeton d'Armure par scène**, 
- lorsqu'il devrait perdre 1 Cœur, il peut plutôt utiliser un jeton d'Armure.

### 9.2 Pression du temps comme chronomètre


Si la scène a une limite de temps, le MJ établit un « compteur » (par exemple, 3 étapes). Chaque échec déplace le compteur de 1. Lorsque le compteur atteint la fin — une conséquence se produit (alarme, fuite de la cible, effondrement du passage).

---

### 9.3 Vengeance (variante de combat risqué)

Si vous souhaitez que le combat soit plus « intense » et rapide :
- lorsque vous **attaquez au corps à corps** et que vous **ratez**, vous perdez **1 Cœur**, à condition que l'adversaire ait pu vous atteindre réellement.
C'est une variante — dans le cœur du NDE, les conséquences des échecs en combat résultent principalement de la fiction et des décisions du MJ.

