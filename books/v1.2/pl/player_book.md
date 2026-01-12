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
generated_at: "2026-01-12T10:14:57.822Z"
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
# Księga Gracza



---



---

### MG opisuje sytuację i mówi, co jest możliwe.
- Ty mówisz, **co robisz** i **jaki chcesz efekt**.
- Jeśli wynik jest niepewny, MG mówi

- MG opisuje sytuację i mówi, co jest możliwe.
- Ty mówisz, **co robisz** i **jaki chcesz efekt**.
- Jeśli wynik jest niepewny, MG mówi:
  1) jakiej cechy używasz (S/Z/M),
  2) jaka jest trudność (<span class="rpg-token token-tn">TN</span>),
  3) co może się stać przy porażce.
- Ty rzucasz **jedną kością** swojej cechy i patrzysz, czy wynik ≥ <span class="rpg-token token-tn">TN</span>.


### Najkrótsza zasada
**Rzuć kością cechy. Wynik ≥ <span class="rpg-token token-tn">TN</span> = sukces.**




---

Twoja postać ma:
- **Rolę** (Wojownik / Łotr / Mag),
- 3 **cechy**: Siła (S), Zręczność (Z), Magia (M),
- **Życie** (Serca) i **Manę**,
- 2 **Talenty** (opcjonalnie, ale polecane),
- ekwipunek.


### 2.1 Cechy (S/Z/M) — do czego są
- **Siła (S)**: walka wręcz, forsowanie, dźwiganie, wytrzymałość.
- **Zręczność (Z)**: strzały, precyzja, skradanie, unik, akrobatyka.
- **Magia (M)**: efekty „specjalne” (czary/psionika/technologia — zależnie od gry).


### 2.2 Kości cech
Każda cecha ma swoją kość (np. <span class="rpg-token token-d6">d6</span>, <span class="rpg-token token-d8">d8</span>, <span class="rpg-token token-d10">d10</span>, <span class="rpg-token token-d12">d12</span>, <span class="rpg-token token-d20">d20</span>). Zawsze rzucasz **jedną** kością.
- Większa kość = większa szansa na wysokie wyniki.


### 2.3 Życie i Mana
- **Życie:** 5 Serc (start).
- **Mana:** 3 (start). Wydajesz ją, gdy używasz Magii.




---

### Krok 1: Wybierz rolę
Wybierz jedną rolę. Ustawia startowe kości cech:
- **Wojownik:** S <span class="rpg-token token-d10">d10</span>, Z <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d6">d6</span>
- **Łotr:** S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
- **Mag:**  S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d6">d6</span>,  M <span class="rpg-token token-d10">d10</span>


### Krok 2: Zapisz zasoby
- Życie: 5 Serc
- Mana: 3


### Krok 3: Wybierz 2 Talenty (opcjonalnie)
Talenty to krótkie hasła opisujące, w czym jesteś dobry.
- Przykłady neutralne: „Negocjator”, „Zwiadowca”, „Mechanik”, „Medyk”, „Atleta”, „Analityk”, „Haker”.

**Jak działają Talenty:** jeśli Talent realnie pomaga w teście, MG może **obniżyć trudność (<span class="rpg-token token-tn">TN</span>) o 1 stopień**.
- Zwykle 1 Talent na 1 test.
- Talent nie zastępuje opisu działania — pomaga, gdy faktycznie ma sens.


### Krok 4: Sprzęt
Wypisz:
- 1 narzędzie do walki (wręcz lub dystans),
- ochronę (jeśli pasuje),
- 3 rzeczy użytkowe.

Sprzęt w tej grze najczęściej działa jako **„pozwolenie”**: masz coś, więc możesz próbować określonych działań.


### Przykład postaci
- Rola: Łotr
- S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
- Życie 5, Mana 3
- Talenty: „Zwiadowca”, „Negocjator”
- Sprzęt: narzędzie dystansowe, wytrychy, lina, latarka




---

### 4.1 Kiedy rzucasz
Rzucasz, gdy:
- coś jest **ryzykowne** lub niepewne,
- a porażka ma konsekwencję.

Jeśli coś jest oczywiste i bez presji, MG może powiedzieć „udaje się” bez rzutu.


### 4.2 Trudności (<span class="rpg-token token-tn">TN</span>)
Używane są 4 poziomy:
- **<span class="rpg-token token-tn">TN</span> 4 — Łatwe**
- **<span class="rpg-token token-tn">TN</span> 6 — Normalne**
- **<span class="rpg-token token-tn">TN</span> 8 — Trudne**
- **<span class="rpg-token token-tn">TN</span> 12 — Bohaterskie**

MG wybiera <span class="rpg-token token-tn">TN</span>. Ty nie musisz go „zgadywać” — MG po prostu mówi, jaka jest trudność.


### Wyniki Testu

> **Poziom Trudności (<span class="rpg-token token-tn">TN</span>)**: 4 (Łatwy), 6 (Normalny), 8 (Trudny).
> 
> **Wynik Rzutu:**
> - **1**: Porażka + Komplikacja.
> - **< <span class="rpg-token token-tn">TN</span>**: Porażka.
> - **≥ <span class="rpg-token token-tn">TN</span>**: Sukces.
> - **Max (10/20)**: Sukces + Korzyść.

---

### 4.3 Wyniki rzutu
- **Wynik ≥ <span class="rpg-token token-tn">TN</span>:** sukces.
- **Wynik < <span class="rpg-token token-tn">TN</span>:** porażka.
- **Wyrzucona 1:** porażka z komplikacją.
- **Maks na kości** (np. 10 na <span class="rpg-token token-d10">d10</span>): sukces wyjątkowy + dodatkowa korzyść.

**Dodatkowa korzyść** (przykłady): szybciej, ciszej, bezpieczniej, większy efekt, lepsza pozycja.


### 4.4 Zmiany trudności „o stopień”
Zamiast liczyć bonusy, MG czasem zmienia <span class="rpg-token token-tn">TN</span> o 1 stopień:
- gorsze warunki → <span class="rpg-token token-tn">TN</span> wyżej (np. 6 → 8),
- lepsze warunki → <span class="rpg-token token-tn">TN</span> niżej (np. 8 → 6).

Twoja rola jako gracza: **twórz lepsze warunki** przez opis i decyzje (osłona, przygotowanie, narzędzia, plan).


### 4.5 Pomoc sojusznika
Sojusznik może zużyć swoją Akcję, by ci pomóc. Wtedy na ten jeden rzut możesz:
- podbić kość o 1 rozmiar: **<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>**.

Pomoc musi mieć sens w opisie (np. osłanianie, odwrócenie uwagi, podanie narzędzi).


### Przykład testu
Chcesz szybko otworzyć zablokowane przejście.
- MG: „To Zręczność, <span class="rpg-token token-tn">TN</span> 6.”
- Rzucasz Z <span class="rpg-token token-d10">d10</span> i wypada 7 → sukces: przejście otwarte.




---

### 1 kratka

- **1 kratka** to podstawowa jednostka odległości.
- W turze masz **ruch do 5 kratek**.
- Możesz chodzić po skosie (skos liczy się jak 1 kratka).
- Osłona jest ważna: jeśli coś zasłania cię przed atakiem dystansowym, zwykle robi się trudniej trafić.




---

### 6.1 Jak wygląda tura
W swojej turze masz:
- **Ruch** (do 5 kratek),
- **1 Akcję**.

Akcja to np.: atak, użycie sprzętu, test cechy, pomoc, użycie Magii.


### Atak

> 1) Wybierz cel (w zasięgu i w linii widzenia).
> 2) Wybierz broń/czar.
> 3) Sprawdź, jakiej Cechy używa (np. Siła wręcz, Zręczność na dystans, Magia do czaru).
> 4) **Rzuć.** Porównaj z **<span class="rpg-token token-tn">TN</span>** przeciwnika.

---

### 6.2 Atak
- **Wręcz:** rzut **Siły (S)**.
- **Dystans:** rzut **Zręczności (Z)**.
- MG mówi <span class="rpg-token token-tn">TN</span> przeciwnika.

Domyślne <span class="rpg-token token-tn">TN</span> przeciwników:
- **Pachołek:** <span class="rpg-token token-tn">TN</span> 6
- **Elita:** <span class="rpg-token token-tn">TN</span> 8
- **Boss:** <span class="rpg-token token-tn">TN</span> 12


### Trafienie

> - **Pachołek**: Ginie (lub odpada z walki).
> - **Elita/Boss**: Traci **1 Serce**.
> - **Gracz**: Traci **1 Serce** (chyba że ma Pancerz — wtedy Pancerz pochłania trafienie, ale się zużywa).

---

### 6.3 Co oznacza trafienie
- Trafiasz pachołka → schodzi z walki.
- Trafiasz elitę/bossa → dostaje Ranę (Boss standardowo ma 3 Rany).
- Sukces wyjątkowy przeciw elicie/bossowi → zwykle zadajesz +1 Ranę (łącznie 2), albo zyskujesz jedną przewagę sytuacyjną (np. wypchnięcie z osłony).


### Pudło i Odwet

> Walka ma ryzyko. Jeśli **nie trafisz** (wynik < <span class="rpg-token token-tn">TN</span>) lub wyrzucisz **1**:
> - Przeciwnik kontratakuje: tracisz **1 Serce**.
> - Albo dzieje się inna logiczna komplikacja (np. tracisz broń, zostajesz przewrócony).
> 
> *To nie jest tura przeciwnika — to efekt Twojego nieudanego ataku.*

---

### 6.4 Pudło i „odwet”
Jeśli **pudłujesz** (wynik < <span class="rpg-token token-tn">TN</span>) i przeciwnik mógł cię realnie dosięgnąć, tracisz **1 Serce**.
- W zwarciu jest to częste.
- Przy atakach dystansowych dużo zależy od osłony i sytuacji.

Twoja lekcja taktyczna: **ustawiaj się tak, żeby przy pudle nie dostawać odwetu** (osłona, dystans, plan, pomoc).


### 0 Serc

> Jeśli spadniesz do 0 Serc:
> - Jesteś **Powalony**.
> - Nie możesz wykonywać akcji (tylko czołganie i mówienie resztką sił).
> - Sojusznik może Cię „podnieść” (akcja Pomocy), przywracając 1 Serce.
> - Jeśli otrzymasz obrażenia będąc Powalonym — **Ginisz**.

---

### 6.5 0 Serc
Gdy spadasz do 0 Serc:
- jesteś przewrócony i nie wykonujesz akcji,
- sojusznik może zużyć Akcję, żeby postawić cię na nogi z **1 Sercem**.


### Przykład krótkiej tury
- Ruch: podbiegasz 3 kratki do osłony.
- Akcja: strzelasz (Z). MG: „<span class="rpg-token token-tn">TN</span> 6, ale cel jest za osłoną → <span class="rpg-token token-tn">TN</span> 8”. Rzucasz <span class="rpg-token token-d10">d10</span>=9 → trafienie.




---

Magia to mechanika „efektów specjalnych”. Ty opisujesz efekt, MG ustala <span class="rpg-token token-tn">TN</span> i koszt Many.


### 7.1 Koszty i poziomy
- **Sztuczka:** <span class="rpg-token token-tn">TN</span> 4, koszt 0–1
- **Standard:** <span class="rpg-token token-tn">TN</span> 6, koszt 1
- **Silny efekt:** <span class="rpg-token token-tn">TN</span> 8, koszt 2
- **Wielka moc:** <span class="rpg-token token-tn">TN</span> 12, koszt 3


### 7.2 Porażka w Magii
Gdy Magia się nie uda:
- tracisz wydaną Manę,
- pojawia się konsekwencja (np. −1 Serce, utrata pozycji, dodatkowe zagrożenie).


### 7.3 Sukces wyjątkowy
Maks na kości Magii daje dodatkową korzyść:
- większy zasięg/obszar,
- dłuższy czas,
- większa skuteczność,
- albo mniejszy koszt (MG może zwrócić 1 Manę).


### Przykład Magii
Chcesz wykonać krótki „skok” na 5 kratek.
- MG: „To Standard: <span class="rpg-token token-tn">TN</span> 6, koszt 1.”
- Płacisz 1 Manę, rzucasz M <span class="rpg-token token-d10">d10</span>=7 → sukces: przeskakujesz za osłonę.




---

Po konflikcie, jeśli macie bezpieczną chwilę i podstawowe warunki odpoczynku:
- Życie i Mana wracają do pełna.




---

Po przygodzie wybierasz **jedno**:
- podbij S/Z/M o 1 rozmiar kości: <span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>,
- albo +1 Serce (max 7),
- albo +1 Mana (max 5).

To oznacza rozwój bez dokładania kolejnych kości do rzutów.




---

Jeśli na stole jest tylko <span class="rpg-token token-d6">d6</span>, zamiast rozmiaru kości masz próg sukcesu:
- Mistrz 3+, Wyszkolony 4+, Nowicjusz 5+, Bez biegłości 6.

MG może podnosić/obniżać próg o 1 stopień za sytuację lub pomoc.




---

### Zawsze mów

- Zawsze mów: **co robisz** + **po co**. „Chcę wcisnąć dźwignię” jest ok, ale „chcę wcisnąć dźwignię, żeby zamknąć przejście” jest jeszcze lepsze.
- Jeśli <span class="rpg-token token-tn">TN</span> jest wysokie: nie „męcz rzutu” — zmień sytuację (osłona, narzędzia, pomoc, inna droga).
- Ustalajcie współpracę: jedna osoba pomaga, druga wykonuje test.
- W walce szanuj osłonę i pozycję — często jest ważniejsza niż sam rzut.

---
Koniec księgi gracza.


