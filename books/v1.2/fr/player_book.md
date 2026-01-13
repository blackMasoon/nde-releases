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
generated_at: "2026-01-13T06:26:48.878Z"
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
# Manuel du Joueur

Automatic translation placeholder for fr

---



---

### MG décrit la situation et dit ce qui est possible.
- Tu dis, **ce que tu fais** et **quel effet tu souhaites**.
- Si le résultat est incertain, MG dit.

- MG décrit la situation et dit ce qui est possible.
- Tu dis, **ce que tu fais** et **quel effet tu souhaites**.
- Si le résultat est incertain, le MG dit :
  1) quelle caractéristique tu utilises (S/Z/M),
  2) quelle est la difficulté (<span class="rpg-token token-tn">TN</span>),
  3) ce qui peut se passer en cas d'échec.
- Tu lances **un dé** de ta caractéristique et regardes si le résultat ≥ <span class="rpg-token token-tn">TN</span>.

### La règle la plus courte



---

### 1. Introduction

Votre personnage a :
- **Rôle** (Guerrier / Voleur / Mage),
- 3 **caractéristiques** : Force (F), Dextérité (D), Magie (M),
- **Vie** (Cœurs) et **Mana**,
- 2 **Talents** (facultatif, mais recommandé),
- un équipement.

### 2.1 Caractéristiques (S/Z/M) — à quoi elles servent
- **Force (S)** : combat rapproché, forçage, levage, endurance.
- **Agilité (Z)** : tirs, précision, furtivité, esquive, acrobatie.
- **Magie (M)** : effets « spéciaux » (sorts/psychique/technologie — selon le jeu).

### 2.2 Dés des caractéristiques
Chaque caractéristique a son propre dé (par exemple, <span class="rpg-token token-d6">d6</span>, <span class="rpg-token token-d8">d8</span>, <span class="rpg-token token-d10">d10</span>, <span class="rpg-token token-d12">d12</span>, <span class="rpg-token token-d20">d20</span>). Vous lancez toujours **un** dé.
- Un dé plus grand = plus de chances d'obtenir des résultats élevés.

### 2.3 Vie et Mana
- **Vie :** 5 Cœurs (début).
- **Mana :** 3 (début). Tu la dépenses lorsque tu utilises de la Magie.



---

### Étape 1 : Choisissez un rôle
Choisissez un rôle. Cela définit les dés de caractéristiques de départ :
- **Guerrier :** Force <span class="rpg-token token-d10">d10</span>, Agilité <span class="rpg-token token-d6">d6</span>, Magie <span class="rpg-token token-d6">d6</span>
- **Voleur :** Force <span class="rpg-token token-d6">d6</span>, Agilité <span class="rpg-token token-d10">d10</span>, Magie <span class="rpg-token token-d6">d6</span>
- **Magicien :** Force <span class="rpg-token token-d6">d6</span>, Agilité <span class="rpg-token token-d6">d6</span>, Magie <span class="rpg-token token-d10">d10</span>

### Étape 2 : Enregistrer les ressources

### Étape 3 : Choisissez 2 Talents (facultatif)
Les Talents sont de courtes phrases décrivant dans quoi vous êtes bon.
- Exemples neutres : « Négociateur », « Éclaireur », « Mécanicien », « Médecin », « Athlète », « Analyste », « Hacker ».

**Comment fonctionnent les Talents :** si un Talent aide réellement dans le test, le MJ peut **réduire la difficulté (<span class="rpg-token token-tn">TN</span>) d'un niveau**.
- En général, 1 Talent par test.
- Le Talent ne remplace pas la description de l'action — il aide lorsque cela a réellement du sens.

### Étape 4 : Équipement
Liste :
- 1 outil de combat (de près ou à distance),
- protection (si cela convient),
- 3 objets utilitaires.

L'équipement dans ce jeu fonctionne le plus souvent comme un **« permis »** : tu as quelque chose, donc tu peux essayer certaines actions.

### Exemple de personnage
- Rôle : Voleur
- S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
- Vie 5, Mana 3
- Talents : « Éclaireur », « Négociateur »
- Équipement : outil à distance, crochets, corde, lampe torche



---

### 4.1 Quand tu lances
Tu lances quand :
- quelque chose est **risqué** ou incertain,
- et l'échec a des conséquences.

Si quelque chose est évident et sans pression, le MJ peut dire « ça réussit » sans lancer.

### 4.2 Difficultés (<span class="rpg-token token-tn">TN</span>)
Quatre niveaux sont utilisés :
- **<span class="rpg-token token-tn">TN</span> 4 — Facile**
- **<span class="rpg-token token-tn">TN</span> 6 — Normal**
- **<span class="rpg-token token-tn">TN</span> 8 — Difficile**
- **<span class="rpg-token token-tn">TN</span> 12 — Héroïque**

Le MJ choisit la <span class="rpg-token token-tn">TN</span>. Vous n'avez pas besoin de "deviner" — le MJ indique simplement quelle est la difficulté.

### Wyniki Testu

> **Niveau de Difficulté (<span class="rpg-token token-tn">TN</span>)** : 4 (Facile), 6 (Normal), 8 (Difficile).
> 
> **Résultat du Lancer :**
> - **1** : Échec + Complication.
> - **< <span class="rpg-token token-tn">TN</span>** : Échec.
> - **≥ <span class="rpg-token token-tn">TN</span>** : Succès.
> - **Max (10/20)** : Succès + Avantage.

---

### 4.3 Résultats du jet
- **Résultat ≥ <span class="rpg-token token-tn">TN</span> :** succès.
- **Résultat < <span class="rpg-token token-tn">TN</span> :** échec.
- **Jet de 1 :** échec avec complication.
- **Max sur les dés** (par exemple, 10 sur <span class="rpg-token token-d10">d10</span>) : succès exceptionnel + avantage supplémentaire.

**Avantage supplémentaire** (exemples) : plus rapide, plus silencieux, plus sûr, plus grand effet, meilleure position.

### 4.4 Changements de difficulté « d'un degré »
Au lieu de compter les bonus, le MJ change parfois la <span class="rpg-token token-tn">TN</span> d'un degré :
- conditions moins favorables → <span class="rpg-token token-tn">TN</span> plus élevée (par exemple, 6 → 8),
- conditions plus favorables → <span class="rpg-token token-tn">TN</span> plus basse (par exemple, 8 → 6).

Votre rôle en tant que joueur : **créez de meilleures conditions** par la description et les décisions (couverture, préparation, outils, plan).

### 4.5 Aide d'un allié
Un allié peut utiliser son Action pour t'aider. Dans ce cas, pour ce seul jet, tu peux :
- augmenter le dé d'une taille : **<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>**.

L'aide doit avoir un sens dans la description (par exemple, couvrir, distraire, fournir des outils).

### Exemple de test
Tu veux rapidement ouvrir un passage bloqué.
- MG : « C'est de l'Agilité, <span class="rpg-token token-tn">TN</span> 6. »
- Tu lances un <span class="rpg-token token-d10">d10</span> et tu obtiens 7 → succès : passage ouvert.



---

### 1. Kratka

- **1 case** est l'unité de base de distance.
- Dans un tour, vous avez **un mouvement de 5 cases**.
- Vous pouvez vous déplacer en diagonale (une diagonale compte comme 1 case).
- La couverture est importante : si quelque chose vous protège d'une attaque à distance, il est généralement plus difficile de toucher.



---

### 6.1 À quoi ressemble un tour
Dans votre tour, vous avez :
- **Mouvement** (jusqu'à 5 cases),
- **1 Action**.

Une action peut être : attaque, utilisation d'équipement, test de caractéristique, aide, utilisation de la Magie.

### Atak

> 1) Choisissez une cible (dans la portée et en ligne de vue).
> 2) Choisissez une arme/sort.
> 3) Vérifiez quelle Caractéristique est utilisée (par exemple, Force au corps à corps, Dextérité à distance, Magie pour le sort).
> 4) **Lancez.** Comparez avec la **<span class="rpg-token token-tn">TN</span>** de l'adversaire.

---

### 6.2 Attaque
- **Corps à corps :** jet de **Force (F)**.
- **À distance :** jet de **Agilité (A)**.
- Le MJ indique la <span class="rpg-token token-tn">TN</span> de l'adversaire.

<span class="rpg-token token-tn">TN</span> par défaut des adversaires :
- **Péon :** <span class="rpg-token token-tn">TN</span> 6
- **Élite :** <span class="rpg-token token-tn">TN</span> 8
- **Boss :** <span class="rpg-token token-tn">TN</span> 12

### Trafienie

> - **Pachołek** : Meurt (ou est éliminé du combat).
> - **Élite/Boss** : Perd **1 Cœur**.
> - **Joueur** : Perd **1 Cœur** (sauf s'il a une Armure — dans ce cas, l'Armure absorbe le coup, mais s'use).

---

### 6.3 Que signifie un coup
- Tu touches un cône → il sort du combat.
- Tu touches une élite/un boss → il reçoit une Blessure (le boss a généralement 3 Blessures).
- Succès exceptionnel contre une élite/un boss → tu infliges généralement +1 Blessure (au total 2), ou tu gagnes un avantage situationnel (par exemple, le repousser de sa couverture).

### Pudło i Odwet

> Walka ma ryzyko. Jeśli **tu ne touches pas** (wynik < <span class="rpg-token token-tn">TN</span>) ou que tu obtiens **1** :
> - L'adversaire contre-attaque : tu perds **1 Cœur**.
> - Ou une autre complication logique se produit (par exemple, tu perds une arme, tu es renversé).
> 
> *Ce n'est pas le tour de l'adversaire — c'est l'effet de ton attaque ratée.*

---

### 6.4 Pudło et « revanche »
Si tu **pudles** (résultat < <span class="rpg-token token-tn">TN</span>) et que l'adversaire pouvait réellement t'atteindre, tu perds **1 Cœur**.
- C'est fréquent en combat rapproché.
- Pour les attaques à distance, beaucoup dépend de la couverture et de la situation.

Ta leçon tactique : **positionne-toi de manière à ne pas subir de revanche en cas de raté** (couverture, distance, plan, aide).

### 0 Serc

> Si tu tombes à 0 Cœurs :
> - Tu es **À terre**.
> - Tu ne peux pas effectuer d'actions (seulement ramper et parler avec tes dernières forces).
> - Un allié peut te "relever" (action Aide), en te redonnant 1 Cœur.
> - Si tu reçois des dégâts en étant À terre — **Tu meurs**.

---

### 6.5 0 Serc
Lorsque tu tombes à 0 Serc :
- tu es renversé et tu ne peux pas effectuer d'actions,
- un allié peut utiliser une Action pour te remettre sur pied avec **1 Serc**.

### Exemple de courte action
- Mouvement : tu cours de 3 cases vers la couverture.
- Action : tu tires (Z). MJ : « <span class="rpg-token token-tn">TN</span> 6, mais la cible est derrière la couverture → <span class="rpg-token token-tn">TN</span> 8 ». Tu lances <span class="rpg-token token-d10">d10</span>=9 → touche.



---

### 1. Introduction

Magie à mécanique des « effets spéciaux ». Vous décrivez l'effet, le MJ fixe la difficulté et le coût en mana.

### 7.1 Coûts et niveaux
- **Astuce :** <span class="rpg-token token-tn">TN</span> 4, coût 0–1
- **Standard :** <span class="rpg-token token-tn">TN</span> 6, coût 1
- **Effet puissant :** <span class="rpg-token token-tn">TN</span> 8, coût 2
- **Grande puissance :** <span class="rpg-token token-tn">TN</span> 12, coût 3

### 7.2 Échec en Magie
Lorsque la Magie échoue :
- tu perds la Mana dépensée,
- une conséquence apparaît (par exemple, −1 Cœur, perte de position, menace supplémentaire).

### 7.3 Succès exceptionnel
Le maximum sur les dés de Magie donne un avantage supplémentaire :
- portée/zone plus grande,
- durée plus longue,
- efficacité accrue,
- ou coût réduit (le MJ peut rendre 1 Mana).

### Exemple de Magie
Tu veux effectuer un court « saut » de 5 cases.
- MJ : « C'est Standard : <span class="rpg-token token-tn">TN</span> 6, coût 1. »
- Tu paies 1 Mana, tu lances M <span class="rpg-token token-d10">d10</span>=7 → succès : tu sautes derrière la couverture.



---

### 1. Introduction

Après le conflit, si vous avez un moment de sécurité et des conditions de repos minimales :
- La Vie et le Mana reviennent à plein.



---

### 1. Introduction

Po przygodzie wybierasz **un** :
- augmente S/Z/M d'1 taille de dé : <span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>,
- ou +1 Cœur (max 7),
- ou +1 Mana (max 5).

Cela signifie un développement sans ajouter d'autres dés aux lancers.



---

### 1. Introduction

Si sur la table il n'y a qu'un <span class="rpg-token token-d6">d6</span>, au lieu de la taille du dé, tu as le seuil de succès :
- Maître 3+, Formé 4+, Novice 5+, Sans compétence 6.

Le MJ peut augmenter/diminuer le seuil de 1 niveau en fonction de la situation ou de l'aide.



---

### Toujours dire

- Toujours dis : **ce que tu fais** + **pourquoi**. « Je veux appuyer sur le levier » c'est bien, mais « je veux appuyer sur le levier pour fermer le passage » c'est encore mieux.
- Si le <span class="rpg-token token-tn">TN</span> est élevé : ne dis pas « fatigue du jet » — change la situation (couverture, outils, aide, autre chemin).
- Établissez la coopération : une personne aide, l'autre effectue le test.
- En combat, respecte la couverture et la position — elles sont souvent plus importantes que le jet lui-même.

---
Fin du livre du joueur.

