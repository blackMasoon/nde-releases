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
generated_at: "2026-01-12T20:13:56.007Z"
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
# Księga Zasad



---



---

### Plansza w kratę (papier w kratkę, mata, VTT) i znaczniki postaci.
- Ołówek i karta postaci.
- Kości

- Plansza w kratę (papier w kratkę, mata, VTT) i znaczniki postaci.
- Ołówek i karta postaci.
- Kości: **<span class="rpg-token token-d6">d6</span>, <span class="rpg-token token-d8">d8</span>, <span class="rpg-token token-d10">d10</span>, <span class="rpg-token token-d12">d12</span>, <span class="rpg-token token-d20">d20</span>**.
  - W praktyce wystarczy **po jednej** z każdej (na stół / na drużynę), bo rzuca się jedną kością naraz.
  - Jeśli macie tylko <span class="rpg-token token-d6">d6</span>, użyj wariantu „tylko‑<span class="rpg-token token-d6">d6</span>” (na końcu).




---

Te słowa pojawiają się w zasadach — tutaj są wyjaśnione „po ludzku”:

- **MG (Mistrz Gry)**: osoba prowadząca — opisuje sytuacje, steruje światem i przeciwnikami, ustala trudności (<span class="rpg-token token-tn">TN</span>) i konsekwencje.
- **Gracz**: opisuje działania swojej postaci i wykonuje rzuty.
- **Kratka**: jedno pole na planszy. Używamy kratek do odległości i ruchu.
- **Ruch**: przemieszczenie postaci o określoną liczbę kratek.
- **Akcja**: „jedna ważna rzecz” w turze (atak, rzut zdolności, uruchomienie mechanizmu, czar itd.).
- **Tura**: kolej na wykonanie ruchu i akcji.
- **Test**: rzut kością, który rozstrzyga niepewny wynik.
- **<span class="rpg-token token-tn">TN</span> (Trudność)**: liczba, którą trzeba osiągnąć lub przebić, żeby się udało.
- **Cechy**: Siła (S), Zręczność (Z), Magia (M). Określają jaką kością rzucasz.
- **Kość cechy**: rozmiar kości przypisany do cechy (np. Z <span class="rpg-token token-d10">d10</span>).
- **Sukces**: wynik ≥ <span class="rpg-token token-tn">TN</span>.
- **Sukces wyjątkowy**: **maksymalny wynik** na kości (np. 12 na <span class="rpg-token token-d12">d12</span>). Oprócz sukcesu daje dodatkową korzyść.
- **Komplikacja**: dodatkowy problem po porażce — np. hałas, utrata czasu, zgubienie rzeczy, gorsza pozycja, utrata zasobu.
- **Osłona**: przeszkoda między tobą a celem. Zwykle podnosi <span class="rpg-token token-tn">TN</span> ataku dystansowego.
- **Odwet**: konsekwencja pudła w walce — tracisz 1 Serce, jeśli przeciwnik mógł cię realnie dosięgnąć.
- **Serce**: punkt życia (HP w najprostszym sensie).
- **Mana**: zasób do zdolności „Magia” (może oznaczać też technologię/psionikę — zależnie od świata).
- **Rana (Boss)**: „trafienia” Bossa. Boss pada po kilku Ranach.




---

Tworzenie postaci jest celowo krótkie. Postać to: rola + trzy cechy + zasoby.


### 2.1 Role (wybierz jedną)
- **Wojownik** — specjalizuje się w Siłę (walka wręcz, forsowanie przeszkód).
- **Łotr** — specjalizuje się w Zręczność (strzały, skradanie, precyzja, uniki).
- **Mag** — specjalizuje się w Magię (efekty specjalne, kontrola, „moc”).

Role są nazwami technicznymi. W innym świecie mogą oznaczać np. żołnierza/agenta/specjalistę.


### 2.2 Cechy i kości
Masz trzy cechy:
- **Siła (S)** — wszystko, co opiera się na sile fizycznej i wytrzymałości.
- **Zręczność (Z)** — szybkość, refleks, precyzja, skradanie.
- **Magia (M)** — efekty specjalne: czary, psionika, technologia, „umiejętności nadludzkie” (zależnie od świata).

Każda cecha ma rozmiar kości. Na start:
- **Wojownik**: S <span class="rpg-token token-d10">d10</span>, Z <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d6">d6</span>
- **Łotr**: S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
- **Mag**:  S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d10">d10</span>


### 2.3 Zasoby
- **Życie**: 5 Serc.
- **Mana**: 3.


### 2.4 Talenty (opcjonalne, ale polecane)
Talenty to **2 krótkie hasła**, które opisują w czym twoja postać jest dobra (bez świata i bez listy):
- np. „Negocjator”, „Mechanik”, „Zwiadowca”, „Analityk”, „Atleta”, „Medyk”, „Haker”.

**Jak działają Talenty (prosto):** jeśli Talent realnie pomaga w teście, MG może **obniżyć <span class="rpg-token token-tn">TN</span> o 1 stopień**.
- Talent nie daje automatycznych sukcesów.
- Zwykle **maksymalnie jeden Talent** może pomóc w jednym teście.


### 2.5 Ekwipunek
Wypisz:
- broń lub narzędzie do walki,
- ochronę (opcjonalnie),
- 3 rzeczy przydatne w przygodzie.

Sprzęt w rdzeniu zasad jest „pozwoleniem” (umożliwia akcje), a nie bonusem liczbowym.


### 2.6 Przykład kompletnej postaci
- Rola: Łotr
- Cechy: S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
- Życie: 5 Serc, Mana: 3
- Talenty: „Zwiadowca”, „Negocjator”
- Sprzęt: narzędzie do walki dystansowej, wytrychy, lina, latarka




---

Ta część jest najważniejsza — jeśli ją rozumiesz, rozumiesz system.


### 3.1 Kiedy robisz test
Test robisz wtedy, gdy spełnione są oba warunki:
1) wynik jest niepewny (może się udać albo nie), oraz
2) stawka jest realna (porażka coś zmieni / coś kosztuje).

Jeśli czynność jest banalna i bez presji — MG może powiedzieć „udało się” bez rzutu.


### 3.2 Jak wykonać test (krok po kroku)
1) Gracz mówi **co robi** i **jaki chce efekt**.
2) MG wybiera cechę: S albo Z albo M.
3) MG ustala **<span class="rpg-token token-tn">TN</span>** (Trudność) i ewentualne modyfikacje sytuacyjne.
4) Gracz rzuca **jedną kością cechy**.
5) Porównuj wynik do <span class="rpg-token token-tn">TN</span> i rozstrzygnij skutki.


### 3.3 Skala trudności (<span class="rpg-token token-tn">TN</span>)
Używamy czterech poziomów:
- **<span class="rpg-token token-tn">TN</span> 4 (Łatwe):** uda się często, jeśli postać jest choć trochę kompetentna.
- **<span class="rpg-token token-tn">TN</span> 6 (Normalne):** standardowa trudność w przygodzie.
- **<span class="rpg-token token-tn">TN</span> 8 (Trudne):** wymaga przewagi sytuacyjnej, przygotowania lub specjalizacji.
- **<span class="rpg-token token-tn">TN</span> 12 (Bohaterskie):** duże wyzwanie. Zwykle dla bardzo dobrych kości (<span class="rpg-token token-d12">d12</span>/<span class="rpg-token token-d20">d20</span>), świetnych warunków lub obu naraz.


### Wyniki Testu

> **Poziom Trudności (<span class="rpg-token token-tn">TN</span>)**: 4 (Łatwy), 6 (Normalny), 8 (Trudny).
> 
> **Wynik Rzutu:**
> - **1**: Porażka + Komplikacja.
> - **< <span class="rpg-token token-tn">TN</span>**: Porażka.
> - **≥ <span class="rpg-token token-tn">TN</span>**: Sukces.
> - **Max (10/20)**: Sukces + Korzyść.

---

### 3.4 Wyniki testu
- **Wynik ≥ <span class="rpg-token token-tn">TN</span> → Sukces.** Postać osiąga zamierzony efekt.
- **Wynik < <span class="rpg-token token-tn">TN</span> → Porażka.** Efekt nie wychodzi.
- **Wyrzucona 1 → Porażka + komplikacja.** (Nawet gdy <span class="rpg-token token-tn">TN</span> jest niskie.)
- **Maksymalny wynik na kości → Sukces wyjątkowy.**
  - Oprócz sukcesu dostajesz **dodatkową korzyść**.
  - Dodatkowa korzyść powinna wynikać z sytuacji (więcej efektu, mniej ryzyka, szybciej, ciszej, itp.).


### 3.5 Modyfikowanie trudności „bez liczenia”
Zamiast dodawać +1/−1 do rzutów, zmieniamy <span class="rpg-token token-tn">TN</span> o **jeden stopień**.

- **Gorsze warunki** → <span class="rpg-token token-tn">TN</span> +1 stopień (np. 6→8):
  - osłona celu, ciemność, ślisko, presja czasu, hałas, rozproszenie.
- **Lepsze warunki** → <span class="rpg-token token-tn">TN</span> −1 stopień (np. 8→6):
  - przygotowanie, dobre narzędzia, przewaga pozycji, zaskoczenie, pełna koncentracja.

Jeśli coś jest „skrajnie” trudne/łatwe, MG może przesunąć o **2 stopnie**.

**Granice:**
- Jeśli po obniżkach <span class="rpg-token token-tn">TN</span> spada poniżej 4, uznaj to za „prawie pewne” (zwykle bez rzutu).
- Jeśli po podwyżkach <span class="rpg-token token-tn">TN</span> wychodzi powyżej 12, uznaj to za „prawie niemożliwe” (zwykle wymaga planu lub innego podejścia).


### 3.6 Pomoc sojusznika
Sojusznik może w swojej turze (albo w scenie poza walką) poświęcić Akcję, by pomóc.

**Efekt pomocy (rdzeń):** na ten jeden test podbij kość o 1 rozmiar:
- <span class="rpg-token token-d6">d6</span> → <span class="rpg-token token-d8">d8</span> → <span class="rpg-token token-d10">d10</span> → <span class="rpg-token token-d12">d12</span> → <span class="rpg-token token-d20">d20</span>

Zasady porządku:
- Zwykle **jedna osoba** może dać pomoc do jednego testu (żeby nie robić „wieży pomocy”).
- Pomoc musi być opisana sensownie: osłanianie, podanie narzędzi, odwrócenie uwagi, stabilizacja, wskazówki.


### 3.7 Powtarzanie testów
Jeśli test się nie udał, nie powtarzaj go „w kółko” bez zmiany sytuacji.
- Albo robisz coś inaczej (inna cecha / inne narzędzia / inna droga),
- albo akceptujesz komplikację (np. zużycie czasu, alarm),
- albo wycofujesz się.


### 3.8 Przykłady testów (poza walką)
**Przykład A — ciche przejście:**
- Gracz: „Chcę przejść niezauważony przez otwartą przestrzeń”.
- MG: Zręczność (Z). Jest półmrok i są przeszkody → <span class="rpg-token token-tn">TN</span> 6 (Normalne).
- Rzut <span class="rpg-token token-d10">d10</span>=5 → porażka. MG: „Nie zostajesz zauważony od razu, ale ktoś słyszy dźwięk i zaczyna sprawdzać teren (komplikacja: presja czasu)”.

**Przykład B — praca z narzędziami:**
- Gracz: „Chcę szybko uruchomić mechanizm”.
- MG: Siła, jeśli to czysto fizyczne, albo Magia, jeśli to efekt specjalny; tu: Siła (S). <span class="rpg-token token-tn">TN</span> 6.
- Sojusznik pomaga (podbija kość). Rzut <span class="rpg-token token-d12">d12</span>=12 → sukces wyjątkowy: działa od razu i dodatkowo nie robi hałasu.




---

Ta sekcja mówi jak „mierzyć” na planszy.


### 4.1 Kratki
- 1 kratka = podstawowa jednostka odległości.
- Możesz poruszać się także po skosie — liczy się jak zwykła kratka.


### 4.2 Ruch
- Standardowy ruch: **do 5 kratek** w swojej turze.
- Ruch możesz wykonać przed lub po Akcji (albo rozdzielić: część przed, część po).


### 4.3 Linia działania i osłona (prosto)
- **Pełna osłona:** cel jest całkowicie zasłonięty → nie da się go trafić dystansowo.
- **Częściowa osłona:** widać cel, ale jest zasłona → <span class="rpg-token token-tn">TN</span> +1 stopień przy ataku dystansowym.

MG może używać osłony także w innych testach (np. trudniej zauważyć kogoś za przeszkodą).




---

Walka jest „zwykłą sceną z testami”, tylko uporządkowaną w tury.


### 5.1 Kiedy zaczyna się walka
Walka zaczyna się, gdy:
- co najmniej jedna strona chce skrzywdzić drugą, oraz
- ważne jest kto i kiedy działa.

Jeśli sytuacja jest krótka i oczywista, MG może rozstrzygnąć ją bez pełnej walki (np. jednym testem).


### 5.2 Kolejność tur (prosta wersja)
Najprościej:
- Najpierw działają wszyscy gracze (w dowolnej kolejności),
- potem działają przeciwnicy,
- i tak w pętli.

To jest celowo proste i szybkie. Jeśli kiedyś zechcesz bardziej taktycznie, można dodać inicjatywę (to materiał do księgi MG).


### 5.3 Co możesz zrobić w turze
W swojej turze masz:
- **Ruch** (do 5 kratek),
- **1 Akcję**.

Akcja to np.:
- atak,
- rzut cechy (np. wyrwanie dźwigni, przebiegnięcie przez zagrożenie),
- użycie sprzętu,
- pomoc sojusznikowi,
- użycie Magii.


### Atak

> 1) Wybierz cel (w zasięgu i w linii widzenia).
> 2) Wybierz broń/czar.
> 3) Sprawdź, jakiej Cechy używa (np. Siła wręcz, Zręczność na dystans, Magia do czaru).
> 4) **Rzuć.** Porównaj z **<span class="rpg-token token-tn">TN</span>** przeciwnika.

---

### 5.4 Atak — jak to działa
1) Wybierz cel (w zasięgu i w linii działania).
2) Wybierz typ ataku:
   - wręcz → rzut Siły (S),
   - dystans → rzut Zręczności (Z).
3) Ustal <span class="rpg-token token-tn">TN</span> celu.
4) Rzuć kością.

**<span class="rpg-token token-tn">TN</span> przeciwników (rdzeń):**
- **Pachołek:** <span class="rpg-token token-tn">TN</span> 6
- **Elita:** <span class="rpg-token token-tn">TN</span> 8
- **Boss:** <span class="rpg-token token-tn">TN</span> 12


### Trafienie

> - **Pachołek**: Ginie (lub odpada z walki).
> - **Elita/Boss**: Traci **1 Serce**.
> - **Gracz**: Traci **1 Serce** (chyba że ma Pancerz — wtedy Pancerz pochłania trafienie, ale się zużywa).

---

### 5.5 Co się dzieje po trafieniu
- **Pachołek:** po sukcesie „schodzi” (przestaje być zagrożeniem w walce).
- **Elita:** po sukcesie dostaje 1 Ranę; standardowo Elita ma **2 Rany**.
- **Boss:** po sukcesie dostaje 1 Ranę; Boss ma **3 Rany**.
- **Sukces wyjątkowy:**
  - na Elitę/Bossa: zadaj +1 Ranę (czyli łącznie 2 Rany),
  - lub uzyskaj inny sensowny bonus (odepchnięcie, rozbrojenie, przejęcie pozycji) — wybierz jeden.

Jeśli chcesz jeszcze prostszej księgi potworów, możesz zrezygnować z elit i używać tylko pachołków i bossów.


### Pudło i Odwet

> Walka ma ryzyko. Jeśli **nie trafisz** (wynik < <span class="rpg-token token-tn">TN</span>) lub wyrzucisz **1**:
> - Przeciwnik kontratakuje: tracisz **1 Serce**.
> - Albo dzieje się inna logiczna komplikacja (np. tracisz broń, zostajesz przewrócony).
> 
> *To nie jest tura przeciwnika — to efekt Twojego nieudanego ataku.*

---

### 5.6 Pudło i „Odwet”
Walka ma ryzyko. Gdy atakujesz i nie trafiasz, przeciwnik często „odpowiada”.

**Zasada odwetu (rdzeń):** jeśli wynik ataku < <span class="rpg-token token-tn">TN</span> i przeciwnik mógł cię realnie dosięgnąć, tracisz **1 Serce**.

Jak rozumieć „mógł dosięgnąć” (bez zawiłości):
- jeśli atakujesz wręcz (stoisz obok) — prawie zawsze tak,
- jeśli atakujesz dystansowo, a jesteś na otwartej przestrzeni i przeciwnik ma możliwość oddania ataku — zwykle tak,
- jeśli masz pełną osłonę lub jesteś poza realnym zasięgiem zagrożenia — zwykle nie.

**Wyrzucona 1 w walce:** porażka + komplikacja. Najczęściej oznacza to: tracisz 1 Serce i dodatkowo coś się pogarsza (np. upadasz, gubisz broń, zostajesz wypchnięty z osłony).


### 5.7 Zasięg ataków (domyślny)
Żeby nie mnożyć liczb, użyj prostych zasad:
- Wręcz: cel na sąsiedniej kratce.
- Dystans: cel w „zasięgu wzroku” na planszy.
  - Jeśli MG chce ograniczenia: przyjmij **do 10 kratek** bez kary; powyżej 10 kratek <span class="rpg-token token-tn">TN</span> +1 stopień.


### 5.8 Kilku przeciwników naraz
Jeśli kilku pachołków jest „w zwarciu” z jedną postacią, MG może:
- podnieść <span class="rpg-token token-tn">TN</span> o 1 stopień (presja), albo
- uznać, że porażka oznacza dodatkową komplikację (np. tracisz pozycję).

Zasada ma być szybka: **jedno rozstrzygnięcie → jeden efekt**.


### 5.9 Przykłady walki (krok po kroku)
**Przykład A — prosta wymiana w zwarciu:**
- Wojownik (S <span class="rpg-token token-d10">d10</span>) stoi obok pachołka (<span class="rpg-token token-tn">TN</span> 6).
- Rzut <span class="rpg-token token-d10">d10</span>=4 → pudło. Ponieważ to zwarcie, działa odwet → Wojownik traci 1 Serce.

**Przykład B — boss i sukces wyjątkowy:**
- Łotr (Z <span class="rpg-token token-d10">d10</span>) strzela do Bossa (<span class="rpg-token token-tn">TN</span> 12). MG mówi: „Bez przygotowania to trudne”.
- Sojusznik pomaga (kość <span class="rpg-token token-d12">d12</span>) i Łotr ma dobrą pozycję (<span class="rpg-token token-tn">TN</span> 12 → 8).
- Rzut <span class="rpg-token token-d12">d12</span>=12 → sukces wyjątkowy: Boss dostaje 2 Rany.




---

W tej mechanice „Magia” to kategoria efektów specjalnych. W zależności od świata może oznaczać:
- czary, psionikę,
- sprzęt/technologię,
- zdolności nadludzkie,
- dowolny inny „specjalny zasób” postaci.


### 6.1 Mana
- Na start masz **3 Many**.
- Mana jest wydawana, gdy próbujesz uzyskać efekt „ponad normalne możliwości”.


### 6.2 Jak działa użycie Magii
1) Opisz efekt, który chcesz uzyskać.
2) MG przypisuje <span class="rpg-token token-tn">TN</span> i koszt Many.
3) Wydaj Manę.
4) Rzuć kością Magii (M) i porównaj do <span class="rpg-token token-tn">TN</span>.

**Porażka:** efekt nie działa; Mana przepada; dochodzi drobna konsekwencja.


### 6.3 Poziomy efektów (<span class="rpg-token token-tn">TN</span> i koszt)
- **Sztuczka:** <span class="rpg-token token-tn">TN</span> 4, koszt 0–1
  - mały efekt: światło, dźwięk, zasłona dymna, chwilowe rozproszenie.
- **Standard:** <span class="rpg-token token-tn">TN</span> 6, koszt 1
  - pocisk, bariera, skok 5 kratek, krótkie wzmocnienie.
- **Silny:** <span class="rpg-token token-tn">TN</span> 8, koszt 2
  - obszar, kontrola, leczenie +2 Serca, unieruchomienie.
- **Wielka moc:** <span class="rpg-token token-tn">TN</span> 12, koszt 3
  - duży, sceniczny efekt, który zmienia sytuację.


### 6.4 Sukces wyjątkowy w Magii
Jeśli wyrzucisz maks na kości Magii:
- zwiększ skalę efektu (np. większy obszar / dłużej / mocniej), albo
- obniż koszt (MG może zwrócić 1 Manę), albo
- dodaj dodatkową korzyść (np. efekt jest cichy, precyzyjny, bezpieczny dla sojuszników).


### 6.5 Przykłady Magii
**Przykład A — defensywa:**
- Gracz: „Chcę postawić krótką osłonę, żeby bezpiecznie przebiec 5 kratek”.
- MG: Standard <span class="rpg-token token-tn">TN</span> 6, koszt 1.
- Rzut M <span class="rpg-token token-d10">d10</span>=9 → sukces: przebiegasz, sytuacja jest bezpieczniejsza.

**Przykład B — porażka i konsekwencja:**
- Gracz: „Chcę unieruchomić elitę” (<span class="rpg-token token-tn">TN</span> 8, koszt 2).
- Rzut=3 → porażka: efekt nie działa, tracisz 2 Many i pojawia się komplikacja (np. odsłaniasz się).




---

### 7.1 Serce (życie)
- Standardowo masz **5 Serc**.
- Utrata Serca oznacza realną szkodę lub wyczerpanie — zależnie od świata.


### 0 Serc

> Jeśli spadniesz do 0 Serc:
> - Jesteś **Powalony**.
> - Nie możesz wykonywać akcji (tylko czołganie i mówienie resztką sił).
> - Sojusznik może Cię „podnieść” (akcja Pomocy), przywracając 1 Serce.
> - Jeśli otrzymasz obrażenia będąc Powalonym — **Ginisz**.

---

### 7.2 0 Serc
Jeśli spadniesz do 0 Serc:
- jesteś **przewrócony** i nie wykonujesz akcji,
- sojusznik może poświęcić Akcję, aby postawić cię na nogi z **1 Sercem**.


### 7.3 Odpoczynek
Po scenie walki/konfliktu, jeśli macie chwilę bezpiecznego odpoczynku (i podstawowe warunki), wracacie do pełni:
- Serc,
- Many.

To utrzymuje system szybki i nie wymaga długiego leczenia.




---

Po zakończeniu przygody (lub istotnego etapu) postać wybiera **jedno**:
- podbij S/Z/M o 1 rozmiar kości (<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>),
- albo +1 Serce (max 7),
- albo +1 Mana (max 5).

**Wskazówka:** podbicie kości oznacza większą skuteczność w danej dziedzinie, bez dokładania kolejnych kości do rzutów.




---

Jeśli nie chcesz używać różnych kości, użyj tego wariantu.


### 9.1 Zamiast rozmiarów kości — progi
Każda cecha ma próg sukcesu na <span class="rpg-token token-d6">d6</span>:
- **Mistrz:** sukces na 3+
- **Wyszkolony:** sukces na 4+
- **Nowicjusz:** sukces na 5+
- **Bez biegłości:** sukces tylko na 6


### 9.2 Trudności i sytuacja
Zamiast <span class="rpg-token token-tn">TN</span> 4/6/8/12 używaj „stopni trudności” przez zmianę progu:
- normalnie rzucasz na swój próg,
- trudniej o 1 stopień → próg +1,
- łatwiej o 1 stopień → próg −1,
- (minimalnie 2+, maksymalnie 6).


### 9.3 Pomoc
Pomoc sojusznika obniża próg o 1 na ten rzut.


### 9.4 Walka w tylko‑<span class="rpg-token token-d6">d6</span>
Możesz zostawić te same kategorie przeciwników, ale zamiast <span class="rpg-token token-tn">TN</span> użyj „stopni”:
- Pachołek: „Normalne” (bez zmiany progu),
- Elita: „Trudne” (+1 do progu),
- Boss: „Bohaterskie” (+2 do progu) oraz 3 Rany.


### 9.5 Rozwój
Rozwój w tylko‑<span class="rpg-token token-d6">d6</span>:
- podnieś poziom jednej cechy (np. Nowicjusz→Wyszkolony),
- albo +1 Serce/Mana.




---

Gdy nie wiesz co zrobić, użyj tej kolejności:
1) Co dokładnie gracz chce osiągnąć?
2) Jaka cecha ma sens: S/Z/M?
3) Jakie jest <span class="rpg-token token-tn">TN</span> (4/6/8/12) i czy warunki zmieniają je o 1 stopień?
4) Czy ktoś pomaga (podbicie kości)?
5) Rzut → sukces/porażka.
6) Jeśli porażka: jaka komplikacja (albo odwet w walce)?
7) Jeśli sukces wyjątkowy: jaka dodatkowa korzyść?




---

Te dodatki nie są wymagane, ale czasem ułatwiają prowadzenie.


### 11.1 Ochrona (pancerz) jako prosty zasób
Jeśli chcesz, żeby „ochrona” miała znaczenie mechaniczne:
- Postać z ochroną ma 1 żeton **Pancerza** na scenę.
- Gdy miałaby stracić 1 Serce (odwet/cios), może zamiast tego zużyć Pancerz.


### 11.2 Presja czasu jako stoper
Jeśli scena ma limit czasu, MG ustala „licznik” (np. 3 kroki). Każda porażka przesuwa licznik o 1. Gdy dojdzie do końca — wydarza się konsekwencja (alarm, ucieczka celu, zawalenie przejścia).

---
Koniec księgi podstawowych zasad.


