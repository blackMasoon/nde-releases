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
generated_at: "2026-01-14T12:06:55.793Z"
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

### [ERROR] 1) Bohater w 1 minutę

[Translation Failed] * **Koncept:** kim jesteś i w jakim gatunku grasz (1 zdanie).
* **Rola (wybierz jedną):**

  * **Szturm** – presja, walka, przełamywanie przeszkód
  * **Specjalista** – skradanie, precyzja, technika, obserwacja
  * **Adept** – moce, wiedza, wpływ, improwizacja
* **Cechy (3):**

  * **Siła (S)** – siła fizyczna, wytrzymałość, walka wręcz
  * **Zręczność (Z)** – refleks, skradanie, strzelanie, pilotowanie
  * **Moc (M)** – magia/psionika/technologia/blef/intuicja (zależnie od świata)
* **Kości cech:** jedna cecha **<span class="rpg-token token-d12">k12</span>**, jedna **<span class="rpg-token token-d8">k8</span>**, jedna **<span class="rpg-token token-d6">k6</span>** (wybierz zgodnie z rolą).
* **Serca:** 5. **Punkty Mocy:** 3 (wydajesz na moce i „zagrania specjalne”).
Poniżej masz gotowy fragment do wklejenia (wariant A), w stylistyce krótkich zasad „1-page”.

**Łut Szczęścia (jak działa):** wydaj **1 ŁS**, aby wybrać jedno:

* **Przerzut** swojego testu (zostawiasz lepszy wynik), albo
* **Podbicie kości o 1 stopień** na ten jeden rzut (**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>**), albo
* **Zamiana porażki na „sukces z kosztem”** — akcja się udaje, ale MG natychmiast dokłada cenę (np. tracisz czas, robisz hałas, zużywasz zasób, kończysz w gorszej pozycji, przyciągasz uwagę, psujesz sprzęt).

**Odzysk ŁS:** na początku kolejnej sesji wracasz do limitu. MG może przyznać **+1 ŁS** za odważne ryzyko, świetną decyzję fabularną lub granie konsekwencjami.

* **Ekwipunek:** 1 narzędzie „kluczowe” (np. miecz, karabin, zestaw hakerski), 1 ochrona (pancerz, tarcza energetyczna, kamuflaż), 3 drobiazgi pasujące do konceptu.

**Przykład:** Specjalista: Z <span class="rpg-token token-d12">k12</span>, M <span class="rpg-token token-d8">k8</span>, S <span class="rpg-token token-d6">k6</span>. W cyberpunku M to „Hacking/Influence”; w fantasy M to „Magia/Wola”.



---

### [ERROR] 2) Jak rozstrzygać akcje

[Translation Failed] 1. Gracz mówi **co robi** i **jak** (opis w świecie gry).
2. Prowadzący ustala **Trudność** i stawkę („co się stanie przy porażce”).
3. Rzuć kością cechy (S/Z/M) i porównaj z Trudnością.

**Trudność (T):**

* **3** łatwe, **4** standard, **5** trudne, **6** bardzo trudne, **8** heroiczne, **12** legendarne.

**Wynik rzutu:**

* **1** – porażka z konsekwencją (komplikacja wchodzi na pewno).
* **< T** – porażka (ale scena idzie dalej: strata czasu, hałas, gorsza pozycja, utrata zasobu).
* **≥ T** – sukces.
* **Maks na kości** (np. 12 na <span class="rpg-token token-d12">k12</span>, 20 na <span class="rpg-token token-d20">k20</span>) – sukces wyjątkowy: dostajesz dodatkową korzyść.

**Modyfikatory bez liczenia:**

* **Lepsza sytuacja**: podbij kość o 1 stopień (<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>).
* **Gorsza sytuacja**: obniż kość o 1 stopień (<span class="rpg-token token-d20">k20</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d4">k4</span>).
* **Pomoc sojusznika** (kosztuje jego akcję): podbij kość o 1 stopień.

**Przykład:** Adept próbuje zamknąć portal (M <span class="rpg-token token-d8">k8</span>) przy alarmie i stresie → gorsza sytuacja, spada na <span class="rpg-token token-d6">k6</span>. T = 5. Rzut 6: sukces, ale „alarm” zostaje w tle jako presja fabularna.



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

### 4) Magie

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

