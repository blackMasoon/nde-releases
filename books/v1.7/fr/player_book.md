---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.7
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
generated_at: "2026-01-16T10:17:16.430Z"
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
# Manuel du Joueur

Automatic translation placeholder for fr

---



---

### 1) Comment se déroule le jeu à table

- **Le Meneur de Jeu (MJ)** décrit la situation et dit ce qui est possible dans cette scène.
- **Toi** tu dis : **ce que tu fais** et **quel effet tu souhaites**.
- Si le résultat est incertain ou risqué, le MJ dit :
  1) **Quelle caractéristique** tu utilises (<span class="rpg-token token-stat">S</span>/<span class="rpg-token token-stat">Z</span>/<span class="rpg-token token-stat">M</span>),
  2) **Quelle est la difficulté** <span class="rpg-token token-t">D</span> (ou la **défense** de la cible),
  3) **Quelles sont les menaces en cas d'échec** (conséquence).

Ensuite, tu jettes le dé de caractéristique et vous savez immédiatement ce qui se passe ensuite.

### La règle la plus courte

**Lancer le dé de caractéristique. Résultat ≥ <span class="rpg-token token-t">T</span> = succès.**



---

### 2) Ce que possède votre personnage

Votre personnage possède :
- **Concept** (1 phrase : qui vous êtes, dans quel monde vous évoluez),
- **Rôle** (Assaut / Spécialiste / Adepte),
- 3 **caractéristiques** : Force (F), Dextérité (D), Pouvoir (<span class="rpg-token token-stat">P</span>),
- **Cœurs** (endurance) et **Points de Pouvoir** (PP),
- **Coup de Chance** (CC),
- (optionnel) **Talents**,
- **équipement**.

### 2.1 Caractéristiques (F/A/<span class="rpg-token token-stat">P</span>) — à quoi servent-elles

- **Force (F)**: combat rapproché, force physique, portage, endurance. - **Adresse (A)**: tir, précision, furtivité, esquive, acrobatie, conduite de véhicules. - **Puissance (<span class="rpg-token token-stat">P</span>)**: « effets spéciaux » du monde du jeu : magie, psionisme, foi, supertechnologie, piratage, influence, intuition — selon la convention.

### 2.2 Dés de caractéristiques — comment fonctionnent-ils

Chaque caractéristique a un dé : <span class="rpg-token token-<span class="rpg-token token-d4">k4</span>"><span class="rpg-token token-d4">d4</span></span>, <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">d6</span></span>, <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span>, <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span> ou <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">d20</span></span>.  
Lorsque vous utilisez une caractéristique, vous lancez **un dé** de cette caractéristique.

- Plus le dé est grand = plus la chance de succès et de succès exceptionnel (maximum sur le dé) est élevée.

**Exemple :** Vous avez une Dextérité de <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span>. Lorsque vous tirez, grimpez ou vous faufilez, vous lancez généralement un <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span>.

### 2.3 Ressources : Cœurs, Points de Pouvoir et Coup de Chance

- **Cœurs :** 5 au début. Les coups et la pression retirent des Cœurs.
- **Points de Pouvoir (PD) :** 3 au début. Vous les dépensez pour des pouvoirs et des actions hors norme.
- **Coup de Chance (CC) :** 2 au début de chaque session. C'est votre « sauvetage de scènes » et l'augmentation du drame.



---

### Étape 1 : Concept et rôle

Choisissez un rôle – c'est le style général d'action (applicable à tout univers).

- **Assaut** : vous prenez des risques et poussez les scènes en avant.  
  (ex. : guerrier, marines, gardien, chasseur, barbare)
- **Spécialiste** : vous agissez avec précision, avec un plan et des outils.  
  (ex. : voleur, sniper, éclaireur, hacker, pilote, traqueur)
- **Adepte** : vous faites des choses "au-delà de la norme" – par le pouvoir, le savoir, l'influence.  
  (ex. : mage, psionique, prêtre, alchimiste, technomancien, diplomate)

### Étape 2 : Répartissez les dés de caractéristiques

Répartissez les dés : une caractéristique <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>, une <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>, une <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>.

Conseils rapides :
- **Assaut** a généralement <span class="rpg-token token-stat">S</span> au plus haut.
- **Spécialiste** a généralement <span class="rpg-token token-stat">Z</span> au plus haut.
- **Adepte** a généralement <span class="rpg-token token-stat">M</span> au plus haut.

### Étape 3 : Enregistrer les ressources

- **Cœurs :** 5 
- **Points de Puissance :** 3 
- **Coup de Chance :** 2 (renouvelé au début de la session)

### Étape 4 (facultatif) : Choisissez 2 Talents

Les talents sont des mots-clés courts décrivant dans quoi vous êtes bon (compétences qui reviennent souvent en jeu). - Exemples : « Éclaireur », « <span class="rpg-token token-stat">M</span>écanicien », « <span class="rpg-token token-stat">M</span>édecin », « Négociateur », « Athlète », « Analyste », « Hackeur », « Ritualiste ».

**Comment fonctionnent les Talents :** si un Talent aide réellement lors d'un test, le MJ considère cela comme une meilleure situation et vous pouvez **augmenter le dé d’un cran** pour ce jet. - En général, 1 Talent par test. - Un Talent ne remplace pas la description d'une action – il doit renforcer un plan sensé.

**Exemple :** Vous avez le Talent « <span class="rpg-token token-stat">M</span>écanicien » et vous essayez de démarrer un générateur en urgence. Le MJ considère que cela aide : vous augmentez <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span> à <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span> pour ce test.

### Étape 5 : Équipement

Listez :
- 1 outil « clé » (arme ou équipement professionnel),
- 1 protection (armure, bouclier, camouflage – selon le monde),
- 3 objets utilitaires.

L'équipement fonctionne le plus souvent comme une **autorisation** : si vous avez quelque chose, vous pouvez essayer des actions appropriées. Un bon outil peut aussi créer une meilleure situation (augmentation des dés), si cela a du sens.

### Exemple de personnage (universel)

- Rôle: Spécialiste
- F <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>, D <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>, I <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>
- Cœurs 5, <span class="rpg-token token-power">PM</span> 3, É<span class="rpg-token token-stat">S</span> 2
- Talents: « Éclaireur », « Négociateur »
- Équipement: arme à distance, crochets / trousse à outils, corde, lampe de poche



---

### 4.1 Quand vous lancez

Vous lancez lorsque :
- quelque chose est **risqué** ou incertain,
- l'échec a une **conséquence significative**.

Si quelque chose est évident et sans pression, le MJ peut dire « ça réussit » sans lancer de dé.

### 4.2 Difficulté <span class="rpg-token token-t">T</span>

Le MJ choisit la Difficulté :

- <span class="rpg-token token-t">T 3</span> facile  
- <span class="rpg-token token-t">T 4</span> standard  
- <span class="rpg-token token-t">T 5</span> difficile  
- <span class="rpg-token token-t">T 6</span> très difficile  
- <span class="rpg-token token-t">T 8</span> héroïque  
- <span class="rpg-token token-t">T 12</span> légendaire

Vous n'avez pas besoin de « deviner » la Difficulté — le MJ la dit explicitement.

### 4.3 Résultats du lancer

- **1**: échec avec conséquence (la complication se produit assurément).
- **Résultat < <span class="rpg-token token-t">T</span>**: échec (mais la scène continue).
- **Résultat ≥ <span class="rpg-token token-t">T</span>**: succès.
- **Maximum sur le dé** (par exemple, 12 sur <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>, 20 sur <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>): succès exceptionnel + avantage supplémentaire.

**Avantage supplémentaire** (exemples): plus vite, plus silencieux, plus sûr, effet plus grand, meilleure position, détail supplémentaire en votre faveur.

### 4.4 Situation améliorée/dégradée (sans bonus)

Au lieu de compter les modificateurs, jouez avec la situation :

- **Situation améliorée** → augmentez le dé d'un cran  
  (<span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>)
- **Situation dégradée** → réduisez le dé d'un cran  
  (<span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d4">k4</span>"><span class="rpg-token token-d4">k4</span></span>)

Votre rôle en tant que joueur : **créez de meilleures conditions** par la description et les décisions (couverture, préparation, outils, plan, reconnaissance).

### 4.5 Aide d'un allié

Un allié peut utiliser son Action pour vous aider. Ensuite, pour ce jet:
- vous améliorez le dé d'un degré.

L'aide doit avoir un sens dans la description (distraction, couverture, transmission d'outils, soutien de tir, deuxième paire de mains).

### Exemple de test (clair et complet)

Tu veux ouvrir une porte verrouillée avant que les gardes n'arrivent.
- MJ : « C'est de la Dextérité. <span class="rpg-token token-t">T 5</span>. Échec : tu fais du bruit et perds du temps. »
- Tu as D <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span>, mais tu utilises des crochets et as le Talent « Spécialiste des serrures » → meilleure situation, tu montes à <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span>.
- Jet <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span> = 6 → succès : la porte s'ouvre sans déclencher d'alarme.

---



---

### 5) Un Coup de Chance (UC) — quand vaut-il la peine de l'utiliser

Au début de chaque session, vous avez **2 UC**. UC est là pour :
- sauver des scènes importantes,
- ajouter de la dramaturgie,
- récompenser les décisions courageuses.

Dépensez **1 UC** pour choisir un :
- **Relancer** votre test (gardez le meilleur résultat), ou
- **Augmenter le dé d'un niveau** pour ce seul jet, ou
- **Transformer un échec en „succès avec coût”** — l'action réussit, mais le MJ ajoute immédiatement un prix à payer.

**Récupération d'UC :** au début de la session suivante, vous revenez à la limite. Le MJ peut accorder **+1 UC** pour un risque courageux, une excellente décision narrative ou pour avoir joué avec les conséquences.

**Exemple :** Un échec lors d'un saut entre les toits signifierait une chute dans la rue. Vous dépensez 1 UC et transformez l'échec en succès avec coût : vous atteignez l'autre côté, mais perdez de l'équipement ou vous tordez la cheville (pire situation dans la scène suivante).



---

### 6.1 Distances (par défaut, sans carte)

Décrivez la distance avec quatre mots :
- **Près** (à portée de main),
- **Pas loin** (quelques pas),
- **Loin** (de l'autre côté de la scène),
- **Très loin** (sniper / véhicule).

Dans un tour, vous avez : **Déplacement + 1 Action**.  
Le déplacement change généralement la distance d'un degré (Pas loin→Près, etc.).

### 6.2 Option : jouer sur une grille

Si vous jouez sur une carte :
- 1 case = 1–2 m,
- déplacement par tour : **jusqu'à 5 cases**,
- les diagonales comptent pour 1 case,
- les autres règles fonctionnent de la même manière.

### 6.3 Attaque

- **Corps à corps :** jet de **Force (<span class="rpg-token token-stat">S</span>)** contre la **Défense** de la cible.  
- **Distance :** jet de **Dextérité (<span class="rpg-token token-stat">Z</span>)** contre la **Défense** de la cible.

**Défense des adversaires (à titre indicatif) :**
- <span class="rpg-token token-t">4</span> Faible  
- <span class="rpg-token token-t">5</span> Type  
- <span class="rpg-token token-t">6</span> Elite  
- <span class="rpg-token token-t">8</span> Boss  
- <span class="rpg-token token-t">12</span> Boss légendaire

### 6.4 Couverture et position

- Cible à couvert / mauvais angle / pression → situation défavorable (réduisez le dé).
- Bonne position / surprise / supériorité numérique → situation favorable (augmentez le dé).

### 6.5 Frapper et dégâts

- Une frappe inflige **1 Cœur**. - Un succès exceptionnel inflige **2 Cœurs** ou produit un effet puissant (désarmement, renversement, repousser, délogement de la couverture).

### 6.6 0 Cœurs

Lorsque tu tombes à **0 Cœurs**, tu es hors de combat (blessé, étourdi, en état de choc - selon la convention).
- Un allié peut utiliser une Action pour te faire remonter à **1 Cœur**.
- Si la pression continue, ta priorité est la protection et l'évacuation, pas le « tanking ».

### Exemple de tour court (sans grille)

- Vous êtes **À Proximité** de l'élite. - Déplacement: vous vous placez **Près** du pilier (couverture). - Action: attaque au corps à corps (<span class="rpg-token token-stat">S</span>). La défense de l'élite est de <span class="rpg-token token-t">6</span>. Vous avez <span class="rpg-token token-stat">S</span> <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>.   Jet de 9: succès, l'élite perd 1 Cœur.



---

### 7) Pouvoirs et actions au-delà de la norme (Points de Pouvoir)

Ce que nous appelons « pouvoir » dépend du monde : sorts, psionique, foi, gadgets, piratage, super-astuces.

### 7.1 Comment utiliser une puissance

1) Décrivez l'effet.  
2) Le MJ indique la difficulté et le coût en <span class="rpg-token token-power">PM</span>.  
3) Dépensez des <span class="rpg-token token-power">PM</span> et lancez **Puissance (<span class="rpg-token token-stat">P</span>)**.

### 7.2 Niveaux d'effet (T / coût)

- **Truc:** effet court, astuce → <span class="rpg-token token-t">T 4</span>, coût 0–1 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>  
- **Standard:** attaque, bouclier, impulsion → <span class="rpg-token token-t">T 5</span>, coût 1 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>  
- **Fort:** zone, guérison, paralysie, hack « en direct » → <span class="rpg-token token-t">T 6</span>, coût 2 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>  
- **Grand:** changement de scène, intervention puissante → <span class="rpg-token token-t">T 8–12</span>, coût 3 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>

### 7.3 Échec et réussite exceptionnelle

- Échec : les <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span> dépensés sont perdus, et la conséquence survient (surcharge, trace, perte de position, effet secondaire). - Maximum sur le dé : réussite exceptionnelle + avantage supplémentaire (portée plus grande, durée plus longue, effet plus puissant, ou moins d'« effets secondaires »).

### 7.4 Récupération <span class="rpg-token token-power">PM</span>

- Après une scène de conflit, vous récupérez **1 <span class="rpg-token token-power">PM</span>**. - Après un repos en toute sécurité – jusqu'au maximum (si le monde du jeu le permet). **Exemple (fantasy):** « Saut court » – Standard, <span class="rpg-token token-t">T 5</span>, coût 1 <span class="rpg-token token-power">PM</span>. **Exemple (sci-fi):** « Surcharge de la serrure électronique » – Standard, <span class="rpg-token token-t">T 5</span>, coût 1 <span class="rpg-token token-power">PM</span>.



---

### 8) Repos et régénération

Si vous avez un moment de sécurité (abri, bandage, service, repas) :
- vous retrouvez tous vos **Cœurs**,
- et vous complétez vos **<span class="rpg-token token-power">PM</span>** selon la règle de repos de votre convention.

Dans des campagnes plus strictes, le MJ peut exiger un arrêt complet pour récupérer tout.



---

### 9) Développement du personnage (lorsque vous « évoluez »)

Le développement se fait **après l'aventure** (généralement après 1 à 3 sessions, selon le rythme de la campagne).  
Vous choisissez **une** des options suivantes:  
- augmentez une caractéristique d'un niveau de dé (max. jusqu'à <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">d20</span></span>), ou  
- +1 Cœur (max. 7), ou  
- +1 <span class="rpg-token token-power">PM</span> (max. 5), ou  
- un nouveau Atout (règle courte à une phrase convenue avec le MJ).  

**Exemple:** La Dextérité passe de <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span> à <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span>. Désormais, tous les tests D se font sur <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span>.



---

### 10) Variante « uniquement <span class="rpg-token token-d6">d6</span> » : 2d6

Si vous souhaitez jouer uniquement avec des <span class="rpg-token token-d6">d6</span> :
- Chaque test est **2d6 + modificateur de caractéristique**.
- Modificateurs de caractéristiques au départ : une caractéristique **+2**, une **+1**, une **+0**.

**Résultat :**
- **6 ou moins** – échec avec conséquence  
- **7–9** – succès avec coût  
- **10+** – succès total  
- **12** – succès exceptionnel

**Situation :** ajoutez **+1 / -1** au jet (en faveur / défaveur), au lieu de changer les seuils.

**Coup de Chance en 2d6 :** fonctionne de la même manière, mais vous remplacez « augmentation de dés » par **+1 au jet**.



---

### 11) Bonnes habitudes de joueur

- Parlez : **ce que vous faites + pourquoi**. L'objectif des actions aide le MJ à établir les enjeux. 
- Si la difficulté est élevée : ne vous "acharnons pas sur le jet" — **changez la situation** (préparation, outil, couverture, aide, autre voie). 
- Collaborez : l'aide d'un allié est l'un des leviers les plus puissants et les plus simples du système. 
- En combat, la position l'emporte : la couverture, la distance et l'avantage situationnel sont souvent plus importants que la statistique.

