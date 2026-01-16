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
generated_at: "2026-01-16T08:33:24.443Z"
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
# Guide du Maître de Jeu

Automatic translation placeholder for fr

---



---

### 0) Directives de maîtrise en 30 secondes

- **Commencez par la fiction.** D'abord, décrivez la situation et les actions des joueurs, puis réalisez le test.
- **Établissez l'enjeu avant le lancer.** Dites : *ce qui est en jeu* et *ce qui se passera en cas d'échec*.
- **Une décision → un lancer → un effet pertinent.** Ne divisez pas une intention en 3 tests.
- **L'échec fait avancer le jeu.** Ne « réinitialisez » pas une scène – modifiez-la par une complication, un coût ou une pression.
- **Maintenez la cohérence.** Les mêmes conditions → une Difficulté similaire, des conséquences similaires.
- **La grille est une option.** Par défaut, le jeu fonctionne sans carte : « Proche / Éloigné / Loin / Très loin ».



---

### 1.1. Quand faire un jet de dés ?

Le jet n'a de sens que lorsque simultanément :
- le résultat **n'est pas évident**,
- il existe **un enjeu réel** (quelque chose va changer),
- les deux parties acceptent que **la mécanique a le droit de décider**.

**Ne faites pas de jet**, lorsque :
- l'action est routinière et sans pression,
- un échec n'apportera rien d'intéressant,
- le succès est certain et le prix déjà payé (par exemple, les joueurs ont le temps, les outils et la sécurité).

**Exemple (sans jet) :** Un spécialiste a un accès administratif et des conditions sereines – l'ouverture de portes standard dans la base ne nécessite pas de test.  
**Exemple (avec jet) :** Les mêmes portes, mais l'alarme est active et une patrouille s'approche dans 30 secondes – c'est un test, car l'enjeu est le temps et la révélation.

### 1.2. Liste de vérification de résolution (procédure de table)

1) Le joueur dit : **ce qu'il fait** et **ce qu'il veut accomplir**. 
2) Vous répondez : **ce qui se met en travers** et **quel est l'enjeu**. 
3) Vous choisissez une caractéristique : **Force (F)** / **Habileté (H)** / **Puissance (<span class="rpg-token token-stat">P</span>)**. 
4) Vous définissez la **Difficulté (D)** ou la **Défense** (en combat). 
5) Vous déterminez le modificateur de situation : **augmentation/diminution du dé** ainsi que **l'aide** éventuelle. 
6) Jet → résultat → conséquence → mise à jour de la scène.

Résumé : **Description → Enjeu → Caractéristique → D/Defense → Jet → Conséquence**.

### 1.3. Difficulté (D) : échelle et règles pratiques

Utilisez une seule échelle tout au long du jeu. Cela renforce la confiance des joueurs envers les décisions du MJ.

- **D 3 – facile :** conditions favorables, pas de pression, résistance minimale.  
- **D 4 – standard :** travail "normal" lors d'une aventure.  
- **D 5 – difficile :** pression temporelle, risque, adversaire, fenêtre étroite.  
- **D 6 – très difficile :** net avantage de l'ennemi, risque élevé, action complexe sous stress.  
- **D 8 – héroïque :** exploit au-dessus de la moyenne; nécessite généralement un avantage, un plan ou une ressource.  
- **D 12 – légendaire :** moment "wow"; rarement sans préparation et souvent à un prix élevé.

**Règle pratique :** si vous ne savez pas quoi choisir, commencez par **D 4** puis justifiez vers le "haut" ou le "bas".

### 1.4. Modificateurs sans calcul : augmenter/diminuer le dé

Au lieu d'ajouter des bonus et des pénalités, dans NDE vous changez **la taille du dé** pour un test.

- **Meilleure situation :** augmentez le dé d'un cran
  <span class="rpg-token token-<span class="rpg-token token-d4">d4</span>"><span class="rpg-token token-d4">d4</span></span>→<span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">d8</span>"><span class="rpg-token token-d8">d8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">d12</span>"><span class="rpg-token token-d12">d12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d20">d20</span>"><span class="rpg-token token-d20">d20</span></span>
- **Pire situation :** diminuez le dé d'un cran (dans l'autre sens).

**Assistance d'un allié :** coûte son action et donne **une augmentation du dé d'un cran** pour ce test.

**Exemple :** Un château en silence (D 4) vs un château sous la pluie et sous le feu (D 5 + diminution du dé, car les mains tremblent et la visibilité est faible).
Ceci fonctionne généralement mieux que « D 6 et +2 et -1 ». 

---

### 1.5. Résultats des tests : succès, échec et rythme de jeu

- **1 sur le dé :** échec + complication (la complication est inévitable).  
- **Résultat < T :** échec (mais la situation évolue).  
- **Résultat ≥ T :** succès.  
- **Résultat maximal sur le dé :** succès exceptionnel (avantage supplémentaire).

#### Comment concevoir un échec sans bloquer le jeu ?

Avant que le joueur ne lance les dés, déterminez 1 à 2 types de coûts :
- **temps** (quelqu'un aura le temps, quelque chose se refermera),
- **position** (moins bien placé, exposé),
- **ressource** (équipement, munitions, énergie, Point de Pouvoir),
- **attention** (alarme, soupçons, piste).

**Exemple (échouer en avançant) :**  
Un joueur veut forcer une porte. Un échec ne signifie pas "tu ne l'ouvres pas".  
Un échec signifie : "tu l'ouvres, mais tu fais du bruit – la patrouille est maintenant Proche, et le niveau d'alerte augmente".



---

### 2) Coup de Chance (CdC) : Comment soutenir la dramaturgie sans gâcher le jeu

Chaque héros commence la session avec **2 CdC**. C'est un outil pour les joueurs, mais le MJ est responsable de son « économie » à la table.

### 2.1. À quoi les joueurs dépensent-ils les Ł<span class="rpg-token token-stat">S</span> ?

Dépensez 1 Ł<span class="rpg-token token-stat">S</span> pour :
- effectuer un **relance** (conserver le meilleur résultat),
- **améliorer un dé d'un degré** pour un seul lancer,
- transformer un échec en **succès avec un coût** (le MJ impose un prix).

### 2.2. Quand attribuer un Point de Destin supplémentaire ?

Le MJ peut attribuer **+1 PD** pour : - une prise de risque consciente qui fait avancer la scène, - accepter les conséquences sans "négocier", - une solution créative conforme au thème, - un jeu très bon avec une relation, une motivation ou un enjeu.

**Principe de parcimonie :** attribuez-les avec parcimonie (1-2 par session et par personne dans un jeu extrêmement généreux). Le PD doit être une "étincelle", pas un carburant permanent.



---

### 3) Conflit et combat

L'EDN doit combattre rapidement. Si le combat dure 60 minutes, cela signifie presque toujours : trop d'ennemis « avec PV » ou trop de jets mineurs.

### 3.1. Par défaut sans carte: distances scéniques

Utilisez quatre distances: 
- **Près** – à portée de main (corps à corps),
- **Pas loin** – à quelques pas,
- **Loin** – de l'autre côté de la scène,
- **Très loin** – distance de sniper/véhicule.

Lors d'un tour, un personnage a : **Déplacement + 1 Action**.  
Le déplacement modifie généralement la distance de **1 degré** (Pas loin→Près).

**Exemple :** Un guerrier est Pas loin. Pendant le tour : il court (Près) et attaque.

### 3.2. Option : grille – quand vous avez besoin de précision

Si vous jouez sur une grille :
- mouvement par tour : **jusqu'à 5 cases**,
- diagonales autorisées,
- terrain difficile peut coûter « 2 cases pour 1 entrée » (optionnel).

Toutes les autres règles restent identiques.

### 3.3. Défense des adversaires et dégâts

En combat, au lieu de la Difficulté, vous utilisez la **Défense** (une sorte de "D pour le combat").

**Défense (indicatif) :**
- **Faible** 4
- **Typique** 5
- **Élite** 6
- **Boss** 8 (boss légendaire 12)

**Attaque :** lancer de **Force** (corps à corps) ou **Dextérité** (à distance) contre la Défense.

**Dégâts (allure) :**
- une touche inflige **1 Cœur**,
- un succès exceptionnel inflige **2 Cœurs** ou produit un effet puissant (désarmement, renversement, perturbation, dispersion).

**Sbires et élites (modèle recommandé) :**
- **Sbir** : 1 touche = disparaît du combat (battu, s'enfuit, neutralisé).
- **Élite** : possède **2 Cœurs** (ou "2 touches"), dispose souvent d'un avantage tactique.
- **Boss** : possède **3 Cœurs** + 1-2 "mouvements de boss" (voir 3.6).

Cela permet des affrontements rapides sans compter les points.

### 3.4. Couvert, avantage et « terrain lisible »

Au lieu de multiplier les règles, utilisez un seul langage : **montée de dé / descente de dé**.

- Couvert léger, fumée, mauvais angle : **diminuez le dé de l'attaquant** d'un niveau.  
- Bonne position, surprise, avantage de hauteur : **augmentez le dé** d'un niveau.  
- Couvert complet : l'attaque est impossible tant que la situation ne change pas.

**Exemple :** Un sniper à la fenêtre est considéré comme étant « Loin » et a un avantage de hauteur → l'attaquant subit une descente de dé.  
L'équipe change la scène : grenade fumigène, contournement, déviation – et l'avantage disparaît.

### 3.5. Ordre en combat sans calcul d'initiative

Schéma rapide recommandé :
1) **Les joueurs agissent** (dans n'importe quel ordre autour de la table).
2) **Les adversaires agissent**.
3) Répétez.

Cela permet aux joueurs de planifier de courtes combinaisons sans alourdir la table avec l'initiative.

### 3.6. Comment concevoir un boss intéressant (et pas seulement une « éponge à dégâts »)

Un boss dans le NDE devrait avoir :
- **Défense 8** (ou 12 dans la version « final de saison »),
- **3 Cœurs**,
- **1 à 2 mouvements uniques** qui changent la scène.

**Exemples de mouvements de boss (universels) :**
- **Repousser:** quelqu'un touché recule de 1 distance (Proche→Loin) et perd sa position.
- **Bris de couverture:** le boss détruit une couverture ou force à sortir de sa cachette.
- **Appel de renforts:** 2 sbires ou une élite rejoignent le combat (de préférence une fois par combat).
- **Zone de danger:** une zone devient dangereuse (feu, électricité, runes) - quiconque la traverse risque un test.

**Règle :** le mouvement du boss doit changer le plateau de jeu, et non seulement "infliger davantage de dégâts".

### 3.7. Moral et comportement des ennemis (procédure légère)

Quand :
- le premier sbire tombe, ou
- l'élite perd son premier Cœur, ou
- le boss perd son deuxième Cœur,

lancez <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span> et décidez :
- **1–2 :** ils se retirent / cherchent un abri / négocient,
- **3–4 :** ils tiennent leur position,
- **5–6 :** ils attaquent agressivement.

Modifiez de **+1** s'ils ont l'avantage, **-1** s'ils sont terrifiés ou isolés.



---

### 4) Pouvoirs (<span class="rpg-token token-stat">P</span>) côté MJ : comment les évaluer et comment ne pas briser le rythme

Dans NDE, le « Pouvoir » inclut la magie, la psionique, la cybernétique, le piratage informatique, le charisme « digne d'un film » – selon l'univers.

### 4.1. Échelle de puissance : Difficulté et coût en Points de Puissance

- **Truc :** D 4, coût 0–1 PP (petit effet, courte durée).
- **Standard :** D 5, coût 1 PP (cible unique, courte téléportation, bouclier).
- **Puissant :** D 6, coût 2 PP (zone, contrôle, guérison).
- **Grand :** D 8–12, coût 3 PP (effet modifiant la scène).

**Conseil :** si un effet doit « changer les règles de la scène » (pont de glace, panne de courant dans un quartier) – c'est un Grand pouvoir.

### 4.2. Conséquences de l'échec d'un pouvoir

L'échec doit être concret et immédiat : - perte de <span class="rpg-token token-power">PM</span> (toujours), - surcharge (baisse de position, exposition), - trace (numérique/astrale), - effet secondaire dans l'environnement (bruit, éclair, odeur, écho).  **Exemple :** Piratage « en direct » pendant un combat. Échec : <span class="rpg-token token-power">PM</span> perdu, et le système enregistre l'intrus – le compteur « contre-ICE » entre en jeu.

### 4.3. Défense contre le pouvoir

Si la fiction le justifie, autorisez un "contre-test" :
- **Dextérité** (esquive, réflexe) ou
- **Pouvoir** (résistance, contre-rituel, barrière).

Le contre-test ne doit pas multiplier les jets. Utilisez-le là où cela rend la scène plus intéressante (par exemple, paralysie, contrôle mental).



---

### 5.1. Construire des scènes en 5 étapes

1) **Objectif de la scène :** ce que le groupe doit accomplir (de manière concrète).  
2) **Obstacles :** 2 à 3 types différents (personnes, dispositifs, environnement).  
3) **Menace :** adversaires, dangers, pièges, pression temporelle.  
4) **Compteur (optionnel) :** 3 à 5 cases ; les échecs font avancer le compteur ; à la fin, une grande conséquence entre en jeu.  
5) **Récompense et conséquences :** ce que le succès change, ce que l'échec change.

C'est le « moteur de scène » minimal – il fonctionne dans le fantasy, la science-fiction et le genre criminel.

### 5.2. Compteurs (clocks) – version simplifiée

Un compteur possède 3 à 5 segments. Il se remplit lorsque :
- un test se termine par un échec,
- quelqu'un fait du bruit,
- les ennemis ont le temps de réagir.

Lorsque le compteur est plein, cela entraîne une conséquence :
- alarme,
- renforts,
- fermeture de la route,
- perte de ressource,
- escalade du conflit.

**Exemple :** « Alarme 0/4 ». Échec en furtivité = +1. Succès exceptionnel = -1 (optionnel).  
Lorsque vous atteignez 4/4 – une patrouille apparaît et les portes se verrouillent.

### 5.3. Comment évaluer la "difficulté d'une scène" sans tout compter

Pour une équipe de 3 à 5 héros :

- **Facile :** 3 à 5 sbires ou une élite sans avantages de terrain.
- **Standard :** 6 à 8 sbires ou une élite + 2 à 4 sbires, ou un danger environnemental.
- **Difficile :** un boss + 2 à 4 sbires, ou 2 élites + 3 à 5 sbires, ou un compte à rebours de 3.
- **Héroïque :** un boss + soutien + pression du terrain + compte à rebours de 3 à 5.

**Le plus important :** le terrain et les couvertures signifient souvent plus que le nombre d'ennemis.



---

### 6.1. Furtivité et infiltration : « Alerte »

1) Définissez le compteur **Alerte 0/3 à 0/5**. 
2) Chaque échec = +1 alerte. 
3) Les joueurs peuvent réduire l'alerte par des actions (par exemple, faux signal, sabotage) – ce sont des tests normaux. 
4) Au maximum, la conséquence intervient : patrouille, verrouillage, confinement.

**Exemple :** L'équipe progresse dans le couloir. Le spécialiste veut contourner les caméras (<span class="rpg-token token-stat">M</span>, D 5). Échec = +1 alerte. 
Avant de lancer, ils savent ce qu'ils risquent – et c'est crucial.

### 6.2. Poursuite : « Distance de poursuite »

Déterminez la **Distance** en pas, par exemple **3** (moyenne).  
À chaque « tour de poursuite » :  
- le fuyard effectue un test (<span class="rpg-token token-stat">Z</span> ou <span class="rpg-token token-stat">M</span> selon la méthode),  
- le poursuivant effectue un test,  
- un succès du fuyard augmente la distance, un succès du poursuivant la diminue,  
- lorsque la distance tombe à **0** – rattrapage,  
- lorsqu'elle atteint **5** – évasion.  
  
Ajoutez des obstacles (virage, foule, barricade) sous forme de description + modificateur de dé.

### 6.3. Enquête : « Indices au lieu de murs de tests »

Règle : **un indice clé ne peut pas rester bloqué sur un seul test**. 
Si la scène d'enquête doit progresser, l'indice clé est disponible :
- automatiquement (si les joueurs ont fait quelque chose de sensé),
- ou après un test, mais l'échec le fournit « avec un coût » (temps, fausse piste, alerte).

**Exemple :** Examen du corps. Succès : ils obtiennent la vérité. Échec : ils obtiennent la vérité, mais la garde arrive ou quelqu'un les remarque.

### 6.4. Conflit social : enjeu, pression, conséquence

Ne transformez pas la conversation en une "lutte de jets de dés". Déterminez :
- ce que veut le PNJ,
- ce que veulent les joueurs,
- quel est l'enjeu,
- combien il y a de "mouvements" avant le point critique (compteur de 3 à 5).

Les tests **<span class="rpg-token token-stat">M</span>** (influence, bluff, autorité) ou **<span class="rpg-token token-stat">Z</span>** (lecture des intentions) modifient la position de la conversation. 
Un échec entraîne un coût (mauvaise impression, perte de ressource, temps, hostilité).



---

### 7.1. Complications en cas d'échec (lancez un <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span>)

1. Perte de temps / quelqu'un a eu le temps de réagir. 
2. Position révélée / alerte accrue. 
3. Dommage mineur : -1 Cœur ou perte d'une ressource. 
4. Mauvaise position : poussée, chute, exposition. 
5. Perte ou détérioration d'équipement. 
6. Une nouvelle menace apparaît dans la scène.

### 7.2. Avantages en cas de succès exceptionnel (lancez <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span>)

1. Plus rapidement (vous économisez du temps ou un mouvement).  
2. Plus silencieusement (pas d'augmentation de l'alerte).  
3. Sans coût (par exemple, sans dépenser de <span class="rpg-token token-power">PM</span> / sans conséquences liées au terrain).  
4. Effet augmenté (plus grande portée, cible supplémentaire).  
5. Meilleure position pour un allié (quelqu'un gagne un bonus de dé lors de la prochaine action).  
6. Indice supplémentaire ou avantage narratif.

### 7.3. Entrée rapide d'un adversaire (format pour les notes)

> **Nom — Défense, Cœurs, Tactique, Astuce/Atout**

- **Sbire:** Défense 4–5, 1 coup = disparaît.  
- **Élite:** Défense 6, 2 Cœurs, un atout (mobilité/contre/couverture).  
- **Boss:** Défense 8 (ou 12), 3 Cœurs, 1–2 mouvements de boss.

**Exemple (universel) :**  
> **Garde — Défense 5, 1 coup, garde le couloir, grenade fumigène (une fois)**




---

### 8) <span class="rpg-token token-stat">S</span>écurité et accord à la table (minimum)

- Déterminez ce que vous ne jouez pas (sujets tabous) et ce que vous « avancez rapidement ».
- Convenez d'un signal simple pour interrompre une scène (par exemple, « stop » ou « pause »).
- Résolvez les conflits à la table par la discussion en dehors de la fiction, et non par des « décisions sous le coup de la colère ».

Cela améliore la qualité du jeu plus que n'importe quelle mécanique.



---

### 9) Modularité et développement par la communauté : comment garder le contrôle

Si vous construisez NDE en tant que "moteur", la communauté pourra le développer plus facilement à travers des packs :

- **Pack thématique** (fantasy/cyberpunk/horreur) : cartographie des Pouvoirs, liste des atouts, équipement, ennemis, 1 à 2 procédures (par exemple, peur, poursuite).
- **Pack d'adversaires :** 10 à 20 entrées pour le sbire/l'élite/le boss + tactiques.
- **Pack d'aventures :** scènes d'une page avec compteurs et enjeux.

**Exigence de qualité de la contribution :** chaque nouvelle règle devrait comporter:
- une phrase "pourquoi c'est nécessaire" (quel problème cela résout),
- une courte description de la règle,
- un exemple de 3 à 5 lignes.

Ainsi, les ajouts ne vont pas disloquer le noyau et resteront lisibles pour les nouveaux venus.

