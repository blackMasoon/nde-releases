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
generated_at: "2026-01-15T07:57:22.500Z"
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
# Start (Zasady w pigułce)



---



---

### 1) Bohater w 1 minutę

* **Koncept:** kim jesteś i w jakim gatunku grasz (1 zdanie).
* **Rola (wybierz jedną):**

  * **Szturm** – presja, walka, przełamywanie przeszkód
  * **Specjalista** – skradanie, precyzja, technika, obserwacja
  * **Adept** – moce, wiedza, wpływ, improwizacja
* **Cechy (3):**

  * **Siła (<span class="rpg-token token-stat">S</span>)** – siła fizyczna, wytrzymałość, walka wręcz
  * **Zręczność (<span class="rpg-token token-stat">Z</span>)** – refleks, skradanie, strzelanie, pilotowanie
  * **Moc (<span class="rpg-token token-stat">M</span>)** – magia/psionika/technologia/blef/intuicja (zależnie od świata)
* **Kości cech:** jedna cecha **<span class="rpg-token token-d12">k12</span>**, jedna **<span class="rpg-token token-d8">k8</span>**, jedna **<span class="rpg-token token-d6">k6</span>** (wybierz zgodnie z rolą).
* **<span class="rpg-token token-heart">Serca</span>:** 5. **Punkty Mocy:** 3 (wydajesz na moce i „zagrania specjalne”).
Poniżej masz gotowy fragment do wklejenia (wariant A), w stylistyce krótkich zasad „1-page”.

**Łut Szczęścia (jak działa):** wydaj **1 Ł<span class="rpg-token token-stat">S</span>**, aby wybrać jedno:

* **Przerzut** swojego testu (zostawiasz lepszy wynik), albo
* **Podbicie kości o 1 stopień** na ten jeden rzut (**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>**), albo
* **Zamiana porażki na „sukces z kosztem”** — akcja się udaje, ale MG natychmiast dokłada cenę (np. tracisz czas, robisz hałas, zużywasz zasób, kończysz w gorszej pozycji, przyciągasz uwagę, psujesz sprzęt).

**Odzysk Ł<span class="rpg-token token-stat">S</span>:** na początku kolejnej sesji wracasz do limitu. MG może przyznać **+1 Ł<span class="rpg-token token-stat">S</span>** za odważne ryzyko, świetną decyzję fabularną lub granie konsekwencjami.

* **Ekwipunek:** 1 narzędzie „kluczowe” (np. miecz, karabin, zestaw hakerski), 1 ochrona (pancerz, tarcza energetyczna, kamuflaż), 3 drobiazgi pasujące do konceptu.

**Przykład:** Specjalista: <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">k6</span>. W cyberpunku <span class="rpg-token token-stat">M</span> to „Hacking/Influence”; w fantasy <span class="rpg-token token-stat">M</span> to „Magia/Wola”.



---

### 2) Jak rozstrzygać akcje

1. Gracz mówi **co robi** i **jak** (opis w świecie gry).
2. Prowadzący ustala **Trudność** i stawkę („co się stanie przy porażce”).
3. Rzuć kością cechy (<span class="rpg-token token-stat">S</span>/<span class="rpg-token token-stat">Z</span>/<span class="rpg-token token-stat">M</span>) i porównaj z Trudnością.

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

**Przykład:** Adept próbuje zamknąć portal (<span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span>) przy alarmie i stresie → gorsza sytuacja, spada na <span class="rpg-token token-d6">k6</span>. T = 5. Rzut 6: sukces, ale „alarm” zostaje w tle jako presja fabularna.



---

### 3) Ruch i walka – domyślnie bez siatki, siatka jako opcja

**Domyślnie: theatre of mind (zalecane)**

* Odległości opisuj jako: **Blisko** (na wyciągnięcie), **Niedaleko** (kilka kroków), **Daleko** (druga strona sceny), **Bardzo daleko** (snajpersko/pojazdowo).
* W turze masz: **Przemieszczenie + 1 Akcję**.

  * Przemieszczenie zwykle zmienia odległość o 1 „stopień” (Niedaleko→Blisko itp.).
* **Atak**: rzut **<span class="rpg-token token-stat">S</span>** (wręcz) albo **<span class="rpg-token token-stat">Z</span>** (dystans) przeciw **Obronie** celu.

**Obrona przeciwników (orientacyjnie):**

* **<span class="rpg-token token-stat">S</span>łaby** 4, **Typowy** 5, **Elita** 6, **Boss** 8 (legendarny boss 12).

**Skutki trafienia (szybka walka):**

* Trafienie zadaje **1 Serce**.
* Sukces wyjątkowy zadaje **2 <span class="rpg-token token-heart">Serca</span>** albo daje silny efekt (rozbrojenie, przewrócenie, rozproszenie).

**Osłona i przewaga pozycyjna:**

* Lekka osłona / gorszy kąt: obniż kość atakującego o 1 stopień.
* Dobra pozycja / zaskoczenie: podbij kość o 1 stopień.

**Opcja: gra na siatce**

* 1 kratka = 1–2 m. Ruch w turze: **do 5 kratek**. Reszta zasad bez zmian.

**Przykład:** Specjalista strzela z osłony (<span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">k12</span>) do elity (Obrona 6). Cel jest w lekkiej osłonie → <span class="rpg-token token-stat">Z</span> spada na <span class="rpg-token token-d8">k8</span>. Rzut 7: sukces, 1 Serce obrażeń.



---

### 4) Moce, „czary” i zagrania specjalne (uniwersalne)

To obejmuje magię, psionikę, cybernetykę, gadżety, sztuczki filmowe – zależnie od świata.

* Gdy robisz coś **ponad standard**: wydaj **Punkt Mocy** i rzuć **<span class="rpg-token token-stat">M</span>**.
* Ustal poziom efektu:

**Poziomy mocy (T / koszt):**

* **Sztuczka** (krótki efekt, trik, „flash”): **T 4 / 0–1 <span class="rpg-token token-power">PM</span>**
* **Standard** (atak, tarcza, impuls, kontrola drobna): **T 5 / 1 <span class="rpg-token token-power">PM</span>**
* **Silna** (obszar, leczenie, paraliż, hack „na żywo”): **T 6 / 2 <span class="rpg-token token-power">PM</span>**
* **Wielka** (zmiana sceny, potężna ingerencja): **T 8–12 / 3 <span class="rpg-token token-power">PM</span>**

**Porażka:** <span class="rpg-token token-power">PM</span> przepada, a konsekwencja jest natychmiastowa (przeciążenie, ślad cyfrowy, rysa w rytuale, niechciana uwaga).

**Odzysk:** po scenie konfliktu odzyskujesz **1 <span class="rpg-token token-power">PM</span>**, po bezpiecznym odpoczynku – do pełna.

**Przykład:** W space-operze Adept próbuje „zagiąć sensor” drona: Standard, T 5, koszt 1 <span class="rpg-token token-power">PM</span>. Rzut <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span> = 8: sukces wyjątkowy – dron traci sygnał i myli trop.



---

### 5) Upadek, ryzyko i leczenie

* Gdy spadasz do **0 Serc**, jesteś **wyłączony z akcji** (raniony, ogłuszony, w szoku – według konwencji).
* Sojusznik może zużyć akcję, by postawić cię na **1 Serce** (pierwsza pomoc, adrenalina, restart systemu).
* Po scenie, jeśli macie chwilę oddechu: wracacie do **pełnych Serc**, o ile macie warunki (schronienie, opatrunek, serwis, posiłek).
* Jeżeli scena była wyjątkowo brutalna albo wrogowie mają przewagę, Prowadzący może wymagać, by „pełny reset” wymagał bezpiecznego postoju.

**Przykład:** Szturm spada do 0. Specjalista wciąga go za osłonę i zużywa akcję: Szturm wraca na 1 Serce i może działać w następnej turze.



---

### 6) Rozwój postaci (kampania bez tabel i księgowości)

Po przygodzie wybierz **jedno**:

* **Podbij** jedną cechę o 1 stopień (maks. do <span class="rpg-token token-d20">k20</span>), albo
* **+1 Serce** (maks. 7), albo
* **+1 Punkt Mocy** (maks. 5), albo
* **Nowy Atut** (krótka, jednozdaniowa zasada uzgodniona z Prowadzącym).

**Przykłady atutów (uniwersalne):**

* **Nacisk:** raz na scenę, gdy trafisz wręcz, zadajesz +1 Serce obrażeń.
* **Cień:** gdy działasz z ukrycia, masz podbicie kości o 1 stopień.
* **Iskra:** raz na scenę możesz wydać 1 <span class="rpg-token token-power">PM</span>, by automatycznie uzyskać „sukces z kosztem” bez rzutu.

**Przykład:** Adept podbija <span class="rpg-token token-stat">M</span> z <span class="rpg-token token-d8">k8</span> na <span class="rpg-token token-d12">k12</span> – teraz jego moce wchodzą stabilniej przy T 5–6.



---

### 7) Wariant „tylko <span class="rpg-token token-d6">k6</span>” w trybie **2k6** (szybki i bardzo grywalny)

Jeżeli nie macie zestawu kości albo chcecie bardziej „fabularne” stopnie wyniku:

* Każdy test to: **rzuć 2k6 + modyfikator cechy**.
* **Modyfikatory cech** wybierz na starcie: jedna cecha **+2**, jedna **+1**, jedna **+0**.
* Wynik:

  * **6 lub mniej** – porażka z konsekwencją
  * **7–9** – sukces z kosztem (kompromis, utrata zasobu, gorsza pozycja)
  * **10+** – pełny sukces
  * **12** – sukces wyjątkowy (dodatkowa korzyść)

**Trudność sytuacji:** zamiast zmieniać progi, dawaj **+1 / -1** do rzutu (sprzyja / przeszkadza) albo koszt w razie 7–9.

**Mapowanie do wersji kości-cech (jeśli chcesz zgodności):**

* <span class="rpg-token token-d6">k6</span> ≈ +0, <span class="rpg-token token-d8">k8</span> ≈ +1, <span class="rpg-token token-d12">k12</span> ≈ +2, <span class="rpg-token token-d20">k20</span> ≈ +3 (dla postaci bardzo doświadczonych).

**Przykład:** Specjalista strzela w biegu: <span class="rpg-token token-stat">Z</span> = +2, sytuacja trudna (-1). Rzut 2k6 = 8, suma 9: sukces z kosztem – trafia, ale kończy w odsłoniętej pozycji.

