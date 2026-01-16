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
generated_at: "2026-01-16T10:17:16.330Z"
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
# Księga Gracza



---



---

### 1) Jak wygląda gra przy stole

- **Prowadzący (MG)** opisuje sytuację i mówi, co jest w tej scenie możliwe.
- **Ty** mówisz: **co robisz** oraz **jaki chcesz efekt**.
- Jeśli wynik jest niepewny albo ryzykowny, MG mówi:
  1) **jakiej cechy** używasz (<span class="rpg-token token-stat">S</span>/<span class="rpg-token token-stat">Z</span>/<span class="rpg-token token-stat">M</span>),
  2) **jaka jest Trudność** <span class="rpg-token token-t">T</span> (albo **Obrona** celu),
  3) **co grozi przy porażce** (konsekwencja).

Potem rzucasz kością cechy i od razu wiecie, co się dzieje dalej.

### Najkrótsza zasada

**Rzuć kością cechy. Wynik ≥ <span class="rpg-token token-t">T</span> = sukces.**

---



---

### 2) Co ma Twoja postać

Twoja postać ma:
- **Koncept** (1 zdanie: kim jesteś, w jakim świecie działasz),
- **Rolę** (Szturm / Specjalista / Adept),
- 3 **cechy**: Siła (<span class="rpg-token token-stat">S</span>), Zręczność (<span class="rpg-token token-stat">Z</span>), Moc (<span class="rpg-token token-stat">M</span>),
- **<span class="rpg-token token-heart">Serca</span>** (wytrzymałość) i **Punkty Mocy** (<span class="rpg-token token-power">PM</span>),
- **Łut Szczęścia** (Ł<span class="rpg-token token-stat">S</span>),
- (opcjonalnie) **Talenty**,
- **ekwipunek**.

### 2.1 Cechy (<span class="rpg-token token-stat">S</span>/<span class="rpg-token token-stat">Z</span>/<span class="rpg-token token-stat">M</span>) — do czego są

- **Siła (<span class="rpg-token token-stat">S</span>)**: walka wręcz, forsowanie, dźwiganie, wytrzymałość.
- **Zręczność (<span class="rpg-token token-stat">Z</span>)**: strzelanie, precyzja, skradanie, uniki, akrobatyka, prowadzenie pojazdów.
- **Moc (<span class="rpg-token token-stat">M</span>)**: „efekty specjalne” świata gry: magia, psionika, wiara, supertechnologia, hacking, wpływ, intuicja — zależnie od konwencji.

### 2.2 Kości cech — jak działają

Każda cecha ma kość: <span class="rpg-token token-<span class="rpg-token token-d4">k4</span>"><span class="rpg-token token-d4">k4</span></span>, <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>, <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>, <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span> lub <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>.  
Gdy używasz cechy, rzucasz **jedną kością** tej cechy.

- Większa kość = większa szansa na sukces i na sukces wyjątkowy (maks na kości).

**Przykład:** Masz Zręczność <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>. Gdy strzelasz, wspinasz się albo skradasz, zwykle rzucasz <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>.

### 2.3 Zasoby: <span class="rpg-token token-heart">Serca</span>, Punkty Mocy i Łut Szczęścia

- **<span class="rpg-token token-heart">Serca</span>:** 5 na start. Trafienia i presja odbierają <span class="rpg-token token-heart">Serca</span>.
- **Punkty Mocy (<span class="rpg-token token-power">PM</span>):** 3 na start. Wydajesz je na moce i zagrania ponad standard.
- **Łut Szczęścia (Ł<span class="rpg-token token-stat">S</span>):** 2 na start każdej sesji. To Twoje „ratowanie scen” i podkręcanie dramaturgii.

---



---

### Krok 1: Koncept i rola

Wybierz rolę – to jest ogólny styl działania (pasuje do każdego uniwersum).

- **Szturm**: wchodzisz w ryzyko i wypychasz sceny do przodu.  
  (np. wojownik, marines, ochroniarz, łowca, barbarzyńca)
- **Specjalista**: działasz precyzyjnie, z planem i narzędziami.  
  (np. łotr, snajper, zwiadowca, haker, pilot, tropiciel)
- **Adept**: robisz rzeczy „ponad standard” – mocą, wiedzą, wpływem.  
  (np. mag, psionik, kapłan, alchemik, technomanta, dyplomata)

### Krok 2: Rozdaj kości cech

Rozdaj kości: jedna cecha <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>, jedna <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>, jedna <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>.

Szybkie podpowiedzi:
- **Szturm** zwykle ma <span class="rpg-token token-stat">S</span> najwyżej.
- **Specjalista** zwykle ma <span class="rpg-token token-stat">Z</span> najwyżej.
- **Adept** zwykle ma <span class="rpg-token token-stat">M</span> najwyżej.

### Krok 3: Zapisz zasoby

- **<span class="rpg-token token-heart">Serca</span>:** 5  
- **Punkty Mocy:** 3  
- **Łut Szczęścia:** 2 (odświeżany na początku sesji)

### Krok 4 (opcjonalnie): Wybierz 2 Talenty

Talenty to krótkie hasła opisujące, w czym jesteś dobry (kompetencje, które często wracają w grze).
- Przykłady: „Zwiadowca”, „Mechanik”, „Medyk”, „Negocjator”, „Atleta”, „Analityk”, „Haker”, „Rytualista”.

**Jak działają Talenty:** jeśli Talent realnie pomaga w teście, MG traktuje to jako lepszą sytuację i możesz **podbić kość o 1 stopień** na ten rzut.  
- Zwykle 1 Talent na 1 test.
- Talent nie zastępuje opisu działania – ma wzmacniać sensowny plan.

**Przykład:** Masz Talent „Mechanik” i próbujesz awaryjnie uruchomić generator. MG uznaje, że to pomaga: podbijasz <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span> na <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span> na ten test.

### Krok 5: Sprzęt

Wypisz:
- 1 narzędzie „kluczowe” (broń lub sprzęt zawodowy),
- 1 ochronę (pancerz, tarcza, kamuflaż – zależnie od świata),
- 3 rzeczy użytkowe.

Sprzęt najczęściej działa jako **pozwolenie**: jeśli coś masz, możesz próbować odpowiednich działań. Dobre narzędzie może też tworzyć lepszą sytuację (podbicie kości), jeśli ma to sens.

### Przykład postaci (uniwersalny)

- Rola: Specjalista  
- <span class="rpg-token token-stat">S</span> <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>, <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>  
- <span class="rpg-token token-heart">Serca</span> 5, <span class="rpg-token token-power">PM</span> 3, Ł<span class="rpg-token token-stat">S</span> 2  
- Talenty: „Zwiadowca”, „Negocjator”  
- Sprzęt: broń dystansowa, wytrychy / zestaw narzędzi, lina, latarka

---



---

### 4.1 Kiedy rzucasz

Rzucasz, gdy:
- coś jest **ryzykowne** lub niepewne,
- porażka ma **znaczącą konsekwencję**.

Jeśli coś jest oczywiste i bez presji, MG może powiedzieć „udaje się” bez rzutu.

### 4.2 Trudność <span class="rpg-token token-t">T</span>

MG wybiera Trudność:

- <span class="rpg-token token-t">T 3</span> łatwe  
- <span class="rpg-token token-t">T 4</span> standard  
- <span class="rpg-token token-t">T 5</span> trudne  
- <span class="rpg-token token-t">T 6</span> bardzo trudne  
- <span class="rpg-token token-t">T 8</span> heroiczne  
- <span class="rpg-token token-t">T 12</span> legendarne

Ty nie musisz „zgadywać” Trudności — MG mówi ją wprost.

### 4.3 Wyniki rzutu

- **1**: porażka z konsekwencją (komplikacja wchodzi na pewno).
- **Wynik < <span class="rpg-token token-t">T</span>**: porażka (ale scena idzie dalej).
- **Wynik ≥ <span class="rpg-token token-t">T</span>**: sukces.
- **Maks na kości** (np. 12 na <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>, 20 na <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>): sukces wyjątkowy + dodatkowa korzyść.

**Dodatkowa korzyść** (przykłady): szybciej, ciszej, bezpieczniej, większy efekt, lepsza pozycja, dodatkowy detal w Twoją stronę.

### 4.4 Lepsza/gorsza sytuacja (bez bonusów)

Zamiast liczyć modyfikatory, gracie sytuacją:

- **Lepsza sytuacja** → podbij kość o 1 stopień  
  (<span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>)
- **Gorsza sytuacja** → obniż kość o 1 stopień  
  (<span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d4">k4</span>"><span class="rpg-token token-d4">k4</span></span>)

Twoja rola jako gracza: **twórz lepsze warunki** przez opis i decyzje (osłona, przygotowanie, narzędzia, plan, rozpoznanie).

### 4.5 Pomoc sojusznika

Sojusznik może zużyć swoją Akcję, by Ci pomóc. Wtedy na ten jeden rzut:
- podbijasz kość o 1 stopień.

Pomoc musi mieć sens w opisie (odwrócenie uwagi, osłona, podanie narzędzi, wsparcie ogniowe, druga para rąk).

### Przykład testu (jasny i kompletny)

Chcesz otworzyć zablokowane drzwi, zanim przybiegną strażnicy.
- MG: „To Zręczność. <span class="rpg-token token-t">T 5</span>. Porażka: robisz hałas i tracisz czas.”
- Masz <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>, ale używasz wytrychów i masz Talent „Specjalista od zamków” → lepsza sytuacja, podbijasz na <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>.
- Rzut <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span> = 6 → sukces: drzwi puszczają bez alarmu.

---



---

### 5) Łut Szczęścia (Ł<span class="rpg-token token-stat">S</span>) — kiedy warto go użyć

Na początku każdej sesji masz **2 Ł<span class="rpg-token token-stat">S</span>**. Ł<span class="rpg-token token-stat">S</span> jest po to, by:
- ratować ważne sceny,
- dodawać dramaturgii,
- nagradzać odważne decyzje.

Wydaj **1 Ł<span class="rpg-token token-stat">S</span>**, aby wybrać jedno:
- **Przerzut** swojego testu (zostawiasz lepszy wynik), albo  
- **Podbicie kości o 1 stopień** na ten jeden rzut, albo  
- **Zamiana porażki na „sukces z kosztem”** — akcja się udaje, ale MG natychmiast dokłada cenę.

**Odzysk Ł<span class="rpg-token token-stat">S</span>:** na początku kolejnej sesji wracasz do limitu. MG może przyznać **+1 Ł<span class="rpg-token token-stat">S</span>** za odważne ryzyko, świetną decyzję fabularną lub granie konsekwencjami.

**Przykład:** Porażka przy skoku między dachami oznaczałaby upadek na ulicę. Wydajesz 1 Ł<span class="rpg-token token-stat">S</span> i zamieniasz porażkę na sukces z kosztem: doskakujesz, ale gubisz sprzęt albo skręcasz kostkę (gorsza sytuacja w kolejnej scenie).

---



---

### 6.1 Odległości (domyślnie, bez mapy)

Opisujcie odległość czterema słowami:
- **Blisko** (na wyciągnięcie ręki),
- **Niedaleko** (kilka kroków),
- **Daleko** (druga strona sceny),
- **Bardzo daleko** (snajpersko / pojazdowo).

W turze masz: **Przemieszczenie + 1 Akcję**.  
Przemieszczenie zwykle zmienia odległość o 1 stopień (Niedaleko→Blisko itp.).

### 6.2 Opcja: gra na siatce

Jeśli gracie na mapie:
- 1 kratka = 1–2 m,
- ruch w turze: **do 5 kratek**,
- diagonale liczą się jak 1 kratka,
- reszta zasad działa identycznie.

### 6.3 Atak

- **Wręcz:** rzut **Siły (<span class="rpg-token token-stat">S</span>)** przeciw **Obronie** celu.  
- **Dystans:** rzut **Zręczności (<span class="rpg-token token-stat">Z</span>)** przeciw **Obronie** celu.

**Obrona przeciwników (orientacyjnie):**
- <span class="rpg-token token-t">4</span> <span class="rpg-token token-stat">S</span>łaby  
- <span class="rpg-token token-t">5</span> Typowy  
- <span class="rpg-token token-t">6</span> Elita  
- <span class="rpg-token token-t">8</span> Boss  
- <span class="rpg-token token-t">12</span> Legendarny boss

### 6.4 Osłona i pozycja

- Cel w osłonie / zły kąt / presja → gorsza sytuacja (obniż kość).
- Dobra pozycja / zaskoczenie / przewaga liczebna → lepsza sytuacja (podbij kość).

### 6.5 Trafienie i obrażenia

- Trafienie zadaje **1 Serce**.
- Sukces wyjątkowy zadaje **2 <span class="rpg-token token-heart">Serca</span>** albo daje mocny efekt (rozbrojenie, przewrócenie, odepchnięcie, wybicie z osłony).

### 6.6 0 Serc

Gdy spadasz do **0 Serc**, jesteś wyłączony z akcji (raniony, ogłuszony, w szoku – według konwencji).
- Sojusznik może zużyć Akcję, by postawić Cię na **1 Serce**.
- Jeśli presja trwa, Twoim priorytetem jest osłona i ewakuacja, nie „tanking”.

### Przykład krótkiej tury (bez siatki)

- Jesteś **Niedaleko** elity.
- Przemieszczenie: wchodzisz **Blisko** za filar (osłona).
- Akcja: atak wręcz (<span class="rpg-token token-stat">S</span>). Obrona elity to <span class="rpg-token token-t">6</span>. Masz <span class="rpg-token token-stat">S</span> <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>.  
  Rzut 9: sukces, elita traci 1 Serce.

---



---

### 7) Moce i zagrania ponad standard (Punkty Mocy)

To, co nazywamy „mocą”, zależy od świata: czary, psionika, wiara, gadżety, hacking, supersztuczki.

### 7.1 Jak używasz mocy

1) Opisz efekt.  
2) MG mówi Trudność i koszt w <span class="rpg-token token-power">PM</span>.  
3) Wydaj <span class="rpg-token token-power">PM</span> i rzuć **Mocą (<span class="rpg-token token-stat">M</span>)**.

### 7.2 Poziomy efektu (T / koszt)

- **Sztuczka:** krótki efekt, trik → <span class="rpg-token token-t">T 4</span>, koszt 0–1 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>  
- **Standard:** atak, tarcza, impuls → <span class="rpg-token token-t">T 5</span>, koszt 1 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>  
- **Silna:** obszar, leczenie, paraliż, hack „na żywo” → <span class="rpg-token token-t">T 6</span>, koszt 2 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>  
- **Wielka:** zmiana sceny, potężna ingerencja → <span class="rpg-token token-t">T 8–12</span>, koszt 3 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>

### 7.3 Porażka i sukces wyjątkowy

- Porażka: wydane <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span> przepadają, a konsekwencja wchodzi (przeciążenie, ślad, utrata pozycji, efekt uboczny).
- Maks na kości: sukces wyjątkowy + dodatkowa korzyść (większy zasięg, dłuższy czas, silniejszy efekt, albo mniej „skutków ubocznych”).

### 7.4 Odzysk <span class="rpg-token token-power">PM</span>

- Po scenie konfliktu odzyskujesz **1 <span class="rpg-token token-power">PM</span>**.
- Po bezpiecznym odpoczynku – do pełna (o ile świat gry na to pozwala).

**Przykład (fantasy):** „Krótki skok” – Standard, <span class="rpg-token token-t">T 5</span>, koszt 1 <span class="rpg-token token-power">PM</span>.  
**Przykład (sci-fi):** „Przeciążam zamek elektroniczny” – Standard, <span class="rpg-token token-t">T 5</span>, koszt 1 <span class="rpg-token token-power">PM</span>.

---



---

### 8) Odpoczynek i regeneracja

Jeśli macie bezpieczną chwilę (schronienie, opatrunek, serwis, posiłek):
- wracacie do pełnych **Serc**,
- i uzupełniacie **<span class="rpg-token token-power">PM</span>** zgodnie z zasadą odpoczynku w waszej konwencji.

W bardziej surowych kampaniach MG może wymagać pełnego postoju, by odzyskać wszystko.

---



---

### 9) Rozwój postaci (kiedy „levelujesz”)

Rozwój następuje **po przygodzie** (zwykle po 1–3 sesjach, zależnie od tempa kampanii).  
Wybierasz **jedno**:
- podbij jedną cechę o 1 stopień kości (maks. do <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>), albo
- +1 Serce (maks. 7), albo
- +1 <span class="rpg-token token-power">PM</span> (maks. 5), albo
- nowy Atut (krótka, jednozdaniowa zasada uzgodniona z MG).

**Przykład:** Zręczność rośnie z <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span> do <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>. Od teraz wszystkie testy <span class="rpg-token token-stat">Z</span> robisz na <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>.

---



---

### 10) Wariant „tylko <span class="rpg-token token-d6">k6</span>”: 2k6

Jeśli chcecie grać tylko na <span class="rpg-token token-d6">k6</span>:
- Każdy test to **2k6 + modyfikator cechy**.
- Modyfikatory cech na start: jedna cecha **+2**, jedna **+1**, jedna **+0**.

**Wynik:**
- **6 lub mniej** – porażka z konsekwencją  
- **7–9** – sukces z kosztem  
- **10+** – pełny sukces  
- **12** – sukces wyjątkowy

**Sytuacja:** dawaj **+1 / -1** do rzutu (sprzyja / przeszkadza), zamiast zmieniać progi.

**Łut Szczęścia w 2k6:** działa identycznie, tylko „podbicie kości” zamieniasz na **+1 do rzutu**.

---



---

### 11) Dobre nawyki gracza

- <span class="rpg-token token-stat">M</span>ów: **co robisz + po co**. Cel działań ułatwia MG ustawienie stawki.
- Jeśli Trudność jest wysoka: nie „męcz rzutu” — **zmień sytuację** (przygotowanie, narzędzie, osłona, pomoc, inna droga).
- Współpracuj: pomoc sojusznika to jedna z najsilniejszych, najprostszych dźwigni w systemie.
- W walce wygrywa pozycja: osłona, dystans i przewaga sytuacyjna są często ważniejsze niż statystyka.

