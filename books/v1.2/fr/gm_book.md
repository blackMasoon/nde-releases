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
generated_at: "2026-01-12T20:14:08.494Z"
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
# Guide du Maître de Jeu

Automatic translation placeholder for fr

---



---

### 7.2 Communiquez clairement le tarif.

- **Communique clairement la difficulté.** Avant de lancer le dé, dis : caractéristique, <span class="rpg-token token-tn">TN</span>, conséquence d'un échec, possibilité d'aide.
- **Description → mécanique → résultat.** Commence toujours par la fiction, puis passe au lancer.
- **Scènes rapides.** Maintiens le rythme : un test = un effet sensé.
- **L'échec fait avancer l'action.** Une complication change la situation, elle ne "réinitialise" pas la scène.
- **Cohérence.** Les mêmes circonstances → les mêmes <span class="rpg-token token-tn">TN</span> et conséquences.



---

### 1. Introduction

1) Le joueur dit ce qu'il fait et ce qu'il veut accomplir.
2) Choisissez une caractéristique : **S** (force), **Z** (précision/rapidité), **M** (effets spéciaux).
3) Déterminez le **<span class="rpg-token token-tn">TN</span>** : 4 facile, 6 normal, 8 difficile, 12 héroïque.
4) Indiquez ce qui est en jeu en cas d'échec et si quelqu'un peut **aider** (augmenter le dé d'une taille).
5) Le joueur lance le dé de la caractéristique et compare au <span class="rpg-token token-tn">TN</span>.
6) Résolvez le résultat et mettez à jour la situation.

Abréviation pour la table : « Caractéristiques/<span class="rpg-token token-tn">TN</span>/Lancer/Conséquence ».



---

### 4 (facile) :

- **4 (facile) :** les conditions sont favorables, l'objectif ne résiste pas.
- **6 (normal) :** standard dans l'aventure sans avantage.
- **8 (difficile) :** pression du temps, mauvaise position, couverture, outils complexes.
- **12 (héroïque) :** défi exceptionnel ; nécessite généralement une préparation ou un dé élevé.

Modification situationnelle : déplacez la <span class="rpg-token token-tn">TN</span> **d'1 niveau** (maximum de 2 dans les extrêmes).
- Pire : sombre, glissant, couverture, alarme → <span class="rpg-token token-tn">TN</span> +1.
- Mieux : temps, outils, avantage de position, surprise → <span class="rpg-token token-tn">TN</span> -1.

Intuitions rapides sur l'efficacité (approximations) :
- <span class="rpg-token token-d6">d6</span> vs TN6 ≈ 17 % ; <span class="rpg-token token-d8">d8</span> vs 6 ≈ 38 % ; <span class="rpg-token token-d10">d10</span> vs 6 ≈ 50 % ; <span class="rpg-token token-d12">d12</span> vs 6 ≈ 58 %.
- <span class="rpg-token token-d10">d10</span> vs TN8 ≈ 30 % ; <span class="rpg-token token-d12">d12</span> vs 8 ≈ 42 % ; <span class="rpg-token token-d20">d20</span> vs 12 ≈ 45 %.
Utilisez ces chiffres à titre indicatif, ne comptez pas en temps réel.

Quand ne pas lancer :
- Lorsque le résultat est évident et qu'il n'y a pas d'enjeu.
- Lorsque le lancer ne changera rien (mieux vaut passer au défi suivant).



---

### 1 sur les os

- **1 sur les dés** : échec + complication. Exemples : bruit, perte de temps, fausse piste, petite blessure (−1 Cœur), ressource perdue, position moins favorable.
- **Échec (résultat < <span class="rpg-token token-tn">TN</span>)** : absence d'effet et éventuelle « riposte » (en combat) ou progression de la menace (hors combat).
- **Succès exceptionnel (max sur les dés)** : succès + avantage supplémentaire : plus rapidement/plus silencieusement/sans coût/effet plus important.

Checklist pour créer des complications :
1) Frappez une ressource (temps, position, cœurs, mana, équipement).
2) Modifiez la disposition sur le plateau (nouveaux obstacles, chemins coupés, protections renforcées).
3) Augmentez la pression (compteur, alarme, renforcement des adversaires).



---

### Ruch:

- **Mouvement :** jusqu'à 5 cases par tour ; déplacement en diagonale autorisé.
- **Couverture :** partielle → attaques à distance <span class="rpg-token token-tn">TN</span> +1 ; totale → pas de ligne de vue.
- **Terrain difficile (optionnel) :** entrer dans une case coûte 2 des 5 points de mouvement.
- **Pousser/déplacer :** test S contre <span class="rpg-token token-tn">TN</span> 6 (modifier selon la situation). Succès : déplacez la cible de 1 à 2 cases ; exceptionnel : +1 case.
- **Portées :** considérez jusqu'à 10 cases comme « sans pénalité » ; au-delà → <span class="rpg-token token-tn">TN</span> +1. La vitesse est plus importante que le comptage minutieux — gardez les règles légères.



---

### Kolejność:

- **Ordre:** joueurs → ennemis → répéter.
- **Attaque:** corps à corps = S, à distance = Z; <span class="rpg-token token-tn">TN</span> de l'ennemi : pion 6, élite 8, boss 12.
- **Toucher:** le pion est éliminé ; élite/boss reçoit 1 Blessure (le boss en a 3). Succès exceptionnel = généralement 2 Blessures.
- **Raté:** si l'ennemi pouvait atteindre → le héros perd 1 Cœur (revanche). En couverture/loin — généralement pas de revanche.

Échelonnement de la pression :
- Plusieurs pions "au corps à corps" → <span class="rpg-token token-tn">TN</span> +1 ou complication supplémentaire en cas de raté.
- Changez le terrain à chaque tour : des obstacles apparaissent, des goulots d'étranglement, des occasions de prendre l'avantage.



---

### 1. Introduction

Construisez des scènes en 5 étapes :
1) **Objectif** : pourquoi la scène (par exemple, transition, acquisition d'un objet, désactivation d'une menace).
2) **Obstacles** : 2-3 types différents (gardes, château, alarme, terrain dangereux).
3) **Menace** : sbires/élite/boss, dangers, pièges.
4) **Compteur (optionnel)** : 3-5 étapes ; les échecs le déplacent ; à la fin, une mauvaise conséquence.
5) **Récompense/conséquence** : ce que le succès apporte, ce que l'échec change.

Seuils de taille de combat (pour 3-5 héros) :
- **Facile :** 3-5 sbires ou élite sans soutien.
- **Standard :** 6-8 sbires ou élite + 2-4 sbires.
- **Difficile :** boss + 2-4 sbires ou 2 élites + 3-5 sbires.
- **Héroïque :** boss + 4-6 sbires et/ou élite.
Adaptez à la table : le terrain et les couvertures ont un impact important.



---

### 1. Introduction

Format (exemple, sans ambiance) :
> **Nom — <span class="rpg-token token-tn">TN</span>, Blessures, Tactique, Spécial**
- **Pion:** <span class="rpg-token token-tn">TN</span> 6, sans Blessures ; tactique simple.
- **Elite:** <span class="rpg-token token-tn">TN</span> 8, 2 Blessures ; a un avantage clair (par exemple, mobilité, couverture, contrôle du terrain).
- **Boss:** <span class="rpg-token token-tn">TN</span> 12, 3 Blessures ; 1–2 mouvements uniques (par exemple, repoussement, appel de renforts).

Réaction et moral (système léger) :
- Lorsque le premier pion tombe ou que l'élite reçoit une Blessure, lancez **<span class="rpg-token token-d6">d6</span>** :
  - 1–2 : retraite/camouflage ; 3–4 : tiennent la position ; 5–6 : attaquent.
- Modifiez ±1 pour avantage/peur/boss à proximité.



---

### 1. Introduction

La magie est des « effets spéciaux ». Attribuez le <span class="rpg-token token-tn">TN</span> et le coût de Mana selon l'échelle :
- **Tour de magie :** <span class="rpg-token token-tn">TN</span> 4, coût 0–1 (effet court, petit).
- **Standard :** <span class="rpg-token token-tn">TN</span> 6, coût 1 (cible unique, saut court, barrière).
- **Fort :** <span class="rpg-token token-tn">TN</span> 8, coût 2 (zone, contrôle, guérison +2 Cœurs).
- **Grande puissance :** <span class="rpg-token token-tn">TN</span> 12, coût 3 (effet scénique).

Règles auxiliaires :
- **Plusieurs cibles :** soit +1 coût de Mana, soit <span class="rpg-token token-tn">TN</span> +1 degré.
- **Maintien de l'effet :** payez 1 Mana par tour ou cela prend une Action.
- **Contre-attaque/esquive de sort :** permettez au héros d'effectuer un test approprié (Z ou M) contre le même <span class="rpg-token token-tn">TN</span> pour réduire ou éviter l'effet (selon la fiction).



---

### Skrytobójstwo/przemykanie : **réglez le « niveau d'alerte » sur **compteur 3–5

- **Assassinat/Discrétion :** règle le « niveau d'alerte » sur **compteur 3–5** ; les échecs l'augmentent ; une fois le maximum atteint, un patrouille apparaît, la serrure se verrouille, etc.
- **Poursuite :** détermine la distance en « pas de poursuite » (par exemple, 3). À chaque tour : les deux parties testent ; le succès du poursuivant réduit la distance, celui du fuyard l'augmente. Lorsque la distance atteint 0 → rattrapage ; à 5 → évasion.
- **Obstacles environnementaux :** communique clairement le coût du risque (par exemple, chute = −1 Cœur et position moins favorable), <span class="rpg-token token-tn">TN</span> dépendant des descriptions.



---

### Développement :

- **Développement :** après l'aventure, chacun choisit une option : augmenter la taille des dés de caractéristique, +1 Cœur (max 7) ou +1 Mana (max 5).
- **Récompenses matérielles :** offrent des « permissions » (nouvelles actions) ou des avantages ponctuels (« une fois par scène, réduire la <span class="rpg-token token-tn">TN</span> de 1 »). Évitez les modificateurs permanents.
- **Économie (optionnelle) :** seuils simples : bon marché/standard/cher — résolvez par un test de ressources au lieu de compter la monnaie.



---

### 1. Introduction

- Établissez avec les joueurs la portée du contenu (ce qui est acceptable, ce qu'il faut éviter).
- Convenez d'un signal simple "stop"/"rewind" pour les situations inconfortables.
- Résolvez les conflits dans la fiction, pas à la table.



---

### 1. Introduction

1) **Hak :** problème en une phrase.
2) **3 lieux** avec des caractéristiques tactiques (couvertures, hauteurs, passages étroits).
3) **3 obstacles :** château, garde, menace environnementale.
4) **Ressources en jeu :** temps, bruit, attention de l'adversaire.
5) **Liste de complications** (5 éléments) et **compteur** pour la scène.
6) **Adversaires :** entrées en 1 ligne (pions/élite/boss) + tactique simple.



---

## Komplikacje — <span class="rpg-token token-d6">d6</span> (universelles) :
1. Perte de temps / avantage de l'adversaire.
2. Révélation de la position / augmentation de l'alerte.
3. Dommages mineurs : −1 Cœur ou ressource.
4. Mauvaise position : poussée/coincement.
5. Perte/coincement d'équipement.
6. Une nouvelle menace apparaît dans la scène.

## Avantages en cas de succès exceptionnel — <span class="rpg-token token-d6">d6</span> :
1. Plus rapidement.
2. Plus silencieusement.
3. Sans coût (par exemple, sans Mana/sans représailles).
4. Effet plus important (zone/portée).
5. Meilleure position des alliés.
6. Indice/information supplémentaire.



---

### Cel des joueurs

- Objectif des joueurs : passer par le passage sécurisé.
- MJ : serrure (<span class="rpg-token token-tn">TN</span> 6), patrouille (compteur 3), passage étroit (couvert).
1) Joueur A : « J'ouvre la serrure » (D, <span class="rpg-token token-tn">TN</span> 6). Échec = +1 au compteur. Lancer 5 → échec, compteur 1/3.
2) Joueur B aide (augmente le dé). A : à nouveau (nouveaux outils, meilleure position), lancer <span class="rpg-token token-d12">d12</span>=9 → succès.
3) La patrouille s'approche (compteur 2/3). Joueur C couvre la sortie (S, <span class="rpg-token token-tn">TN</span> 6). Succès exceptionnel → avantage de position pour l'équipe.
Scène résolue rapidement, avec des enjeux clairs.

---
C'est tout ce dont vous avez besoin pour diriger. Le reste (monde, monstres, trésors) est modulaire et doit être adapté à l'univers choisi.

