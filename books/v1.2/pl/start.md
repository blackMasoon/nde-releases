---
pdf_options:
  displayHeaderFooter: true
  footerTemplate: |-
    <div class="pdf-footer">
      <div style="display:flex; align-items:center;">
        <span>Nano Dungeon Engine</span>
        <img src="https://nano-dungeon-engine.fly.dev/nde_logo.png" class="footer-logo" />
      </div>
      <span>Page <span class="pageNumber"></span> of <span class="totalPages"></span></span>
    </div>
  margin:
    top: "20mm"
    bottom: "20mm"
    left: "20mm"
    right: "20mm"
generated_at: "2026-01-12T09:11:03.642Z"
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
# Start (Zasady w pigułce)



---



---

### 1) Bohater w 1 minutę

- Role (wybierz jedną):
  - Wojownik — mistrz siły i walki wręcz
  - Łotr — mistrz szybkości, skradania i strzałów
  - Mag — mistrz czarów i wiedzy
- Cechy i kości: Siła (S), Zręczność (Z), Magia (M).
  - Wojownik: S <span class="rpg-token token-d10">d10</span>, Z <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d6">d6</span>
  - Łotr: S <span class="rpg-token token-d6">d6</span>,  Z <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
  - Mag:  S <span class="rpg-token token-d6">d6</span>,  Z <span class="rpg-token token-d6">d6</span>,  M <span class="rpg-token token-d10">d10</span>
- Życie: 5 Serc. Mana: 3 (używana przy czarach).
- Ekwipunek: broń, lekki pancerz, 3 przedmioty pasujące do roli.
Przykład: Łotr ma Zręczność <span class="rpg-token token-d10">d10</span>, więc do strzałów używa <span class="rpg-token token-d10">d10</span>.




---

### 2) Jak wykonujesz akcje

1. Wybierz odpowiednią cechę (S/Z/M) i rzuć kością tej cechy.
2. Porównaj do poziomu trudności (<span class="rpg-token token-tn">TN</span>):
   - Łatwe 4, Normalne 6, Trudne 8, Bohaterskie 12.
3. Wynik:
   - 1 na kości — porażka z komplikacją (hałas, strata czasu, drobna rana itp.).
   - Wynik < <span class="rpg-token token-tn">TN</span> — porażka.
   - Wynik ≥ <span class="rpg-token token-tn">TN</span> — sukces.
   - Maks na kości (np. 10 na <span class="rpg-token token-d10">d10</span>, 20 na <span class="rpg-token token-d20">d20</span>) — sukces wyjątkowy z dodatkową korzyścią.
Ulepszenia bez liczenia:
- Lepsza/ gorsza sytuacja: obniż/ podnieś <span class="rpg-token token-tn">TN</span> o 1 stopień (np. 6 → 8 przez osłonę).
- Pomoc sojusznika (swoją akcją): na ten rzut „podbij” kość o jeden rozmiar (<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>).
Przykład: Wojownik wyważa drzwi (Normalne 6). Rzuca <span class="rpg-token token-d10">d10</span> i wyrzuca 10 — sukces wyjątkowy: drzwi wylatują, a stojący za nimi pachołek przewraca się.




---

### 3) Ruch i walka na planszy

- Ruch: do 5 kratek (diagonale dozwolone).
- Twoja tura: Ruch + 1 Akcja (np. atak, czar, przeszukanie, podniesienie dźwigni).
- Atak:
  - Wręcz (S): rzut przeciw <span class="rpg-token token-tn">TN</span> przeciwnika.
  - Dystans (Z): osłona celu podnosi <span class="rpg-token token-tn">TN</span> o 1 stopień.
- <span class="rpg-token token-tn">TN</span> przeciwników: Pachołek 6, Elita 8, Boss 12.
- Skutki trafienia: Pachołek — schodzi po trafieniu; Elita — MG może wymagać sprzyjających warunków; Boss — ma 3 Rany (trafienie = 1 Rana). Sukces wyjątkowy przeciw Bossowi = 2 Rany.
- Odwet: jeśli chybisz w zwarciu lub w zasięgu odwetu, tracisz 1 Serce (chyba że masz pełną osłonę).
Przykład: Mag (Z <span class="rpg-token token-d6">d6</span>) strzela z procy w pachołka za skrzynią: <span class="rpg-token token-tn">TN</span> 6 + osłona → 8. Mag prosi Łotra o pomoc (podbija kość do <span class="rpg-token token-d8">d8</span>) i zmienia pozycję na lepszą (<span class="rpg-token token-tn">TN</span> spada do 6). <span class="rpg-token token-d8">d8</span>=7 — trafiony.




---

### 4) Magia (prosto)

- Rzucenie czaru: opisz efekt, wydaj Manę, rzuć Magię (M).
  - Sztuczka (płomień, huk, mgła) — <span class="rpg-token token-tn">TN</span> 4, koszt 0–1 Many.
  - Pocisk/Osłona/Skok 5 kratek — <span class="rpg-token token-tn">TN</span> 6, koszt 1 Many.
  - Obszar/Leczenie +2 Serca/Paraliż — <span class="rpg-token token-tn">TN</span> 8, koszt 2 Many.
  - Wielka moc (most z lodu, burza ognia) — <span class="rpg-token token-tn">TN</span> 12, koszt 3 Many.
- Porażka: Mana przepada; dochodzi drobna konsekwencja (zadyszka −1 Serce lub niechciana uwaga wrogów).
- Odpoczynek po walce: odzyskujesz całą Manę; bezpieczny postój przywraca też Serca.
Przykład: „Błysk” (krótki teleport 5 kratek): <span class="rpg-token token-tn">TN</span> 6, koszt 1 Many. Mag <span class="rpg-token token-d10">d10</span> rzuca 7 — udany skok za osłonę.




---

### 5) Upadek i leczenie

- 0 Serc: przewrócony (nie działasz). Sojusznik może zużyć akcję, by podnieść Cię do 1 Serca.
- Po starciu, przy krótkim odpoczynku i posiłku, wracacie do pełni Serc i Many.
Przykład: Łotr pada do 0. Wojownik pomaga mu wstać — Łotr wraca na 1 Serce.




---

### 6) Rozwój POSTACI

Po przygodzie wybierz jedno:
- Podbij jeden atrybut o rozmiar kości: <span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>,
- albo +1 Serce (max 7),
- albo +1 Mana (max 5).
Przykład: Wojownik podbija Siłę z <span class="rpg-token token-d10">d10</span> do <span class="rpg-token token-d12">d12</span> — łatwiej trafi <span class="rpg-token token-tn">TN</span> 12.




---

### 7) Wariant tylko-<span class="rpg-token token-d6">d6</span>

Gdy macie tylko jedną kość <span class="rpg-token token-d6">d6</span>:
- Zamiast rozmiarów kości, każda cecha ma próg powodzenia:
  - Mistrz 3+, Wyszkolony 4+, Nowicjusz 5+, Bez biegłości 6.
- <span class="rpg-token token-tn">TN</span> dalej zmienia sytuację o 1 stopień (łatwiej/trudniej).
- Pomoc: obniż próg o 1 (np. z 4+ do 3+ na ten rzut).
- Rozwój: podnieś poziom jednej cechy (np. Wyszkolony 4+ → Mistrz 3+) lub +1 Serce/Mana.
Przykład: Strzał Łotra (Wyszkolony 4+) do celu w lekkiej osłonie (o stopień trudniej) wymaga 5+. Rzut <span class="rpg-token token-d6">d6</span>=5 — trafienie.


