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
generated_at: "2026-01-15T08:02:46.453Z"
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
# Księga Zasad



---



---

### Rzeczy potrzebne do rozgrywki

- Ołówek i karta postaci.
- (Opcjonalnie) mapa/siatka w kratę i znaczniki postaci (papier w kratkę, mata, VTT).
- Kości: **<span class="rpg-token token-d4">k4</span>, <span class="rpg-token token-d6">k6</span>, <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-d20">k20</span>**.
  - W praktyce wystarczy **po jednej** z każdej (rzuca się jedną kością naraz).
  - (Opcjonalnie) **k100** do tabel losowych lub generatorów.
- Jeśli macie tylko **<span class="rpg-token token-d6">k6</span>**, użyj wariantu **2k6** (na końcu).

---



---

### <span class="rpg-token token-stat">S</span>łownik pojęć

Te słowa pojawiają się w zasadach — tutaj są wyjaśnione „po ludzku”:

- **MG (Mistrz Gry)**: prowadzi świat, opisuje sytuacje, steruje przeciwnikami, ustala Trudność i konsekwencje.
- **Gracz**: opisuje działania swojej postaci i wykonuje rzuty.
- **Test**: rzut kością, który rozstrzyga niepewny wynik.
- **Cechy**: **Siła (<span class="rpg-token token-stat">S</span>)**, **Zręczność (<span class="rpg-token token-stat">Z</span>)**, **Moc (<span class="rpg-token token-stat">M</span>)**. <span class="rpg-token token-stat">M</span>ówią, *jaką kością rzucasz*.
- **Kość cechy**: rozmiar kości przypisany do cechy (np. <span class="rpg-token token-stat">Z</span> = <span class="rpg-token token-d12">k12</span>).
- **Trudność (T)**: liczba, którą trzeba osiągnąć lub przebić, żeby akcja się udała.
- **Sukces**: wynik ≥ Trudność.
- **Sukces wyjątkowy**: **maksymalny wynik** na kości (np. 12 na <span class="rpg-token token-d12">k12</span>, 20 na <span class="rpg-token token-d20">k20</span>) — sukces + dodatkowa korzyść.
- **Komplikacja**: dodatkowy problem po porażce (hałas, utrata czasu, gorsza pozycja, utrata zasobu).
- **Sukces z kosztem**: akcja się udaje, ale płacisz cenę (kompromis, utrata zasobu, ujawnienie, ryzyko).
- **Łut Szczęścia (Ł<span class="rpg-token token-stat">S</span>)**: ograniczony zasób, który pozwala ratować sceny (przerzut / podbicie kości / zamiana porażki na sukces z kosztem).
- **<span class="rpg-token token-heart">Serca</span>**: „życie” postaci (wytrzymałość, rany, kondycja — zależnie od świata).
- **Punkty Mocy (<span class="rpg-token token-power">PM</span>)**: zasób na moce i zagrania „ponad standard” (magia, psionika, gadżety, „filmowe” akcje).
- **Obrona**: próg trafienia przeciwnika w walce (zamiast mnożenia zasad o pancerz, klasy pancerza itd.).
- **Osłona**: przeszkoda między tobą a celem. Zwykle utrudnia ataki dystansowe albo działania obserwacyjne.

---



---

### 1. Postać

Tworzenie postaci jest krótkie. Postać to: **koncept + rola + cechy + zasoby + ekwipunek**.

---

### 1.1 Koncept

Jedno zdanie: kim jesteś i w jakim gatunku grasz.

> Przykład: „Była agentka korporacji, dziś łowczyni nagród, która działa po cichu i nie ufa nikomu.”

### 1.2 Role (wybierz jedną)

Role są celowo „neutralne dla świata”. W fantasy możesz je nazwać inaczej, w cyberpunku inaczej, ale działają tak samo.

- **Szturm** — presja, walka, forsowanie przeszkód, przełamywanie frontu.
- **Specjalista** — skradanie, precyzja, technika, obserwacja, plan.
- **Adept** — moce, wpływ, wiedza, improwizacja (magia/psionika/technologia zależnie od świata).

### 1.3 Cechy i kości

Masz trzy cechy:

- **Siła (<span class="rpg-token token-stat">S</span>)** — siła fizyczna, wytrzymałość, walka wręcz, forsowanie.
- **Zręczność (<span class="rpg-token token-stat">Z</span>)** — refleks, precyzja, skradanie, strzelanie, prowadzenie.
- **Moc (<span class="rpg-token token-stat">M</span>)** — „to co specjalne”: magia, psionika, zaawansowana technologia, blef społeczny, intuicja — zależnie od konwencji.

**Na start rozdziel kości tak:**
- jedna cecha ma **<span class="rpg-token token-d12">k12</span>**,
- jedna ma **<span class="rpg-token token-d8">k8</span>**,
- jedna ma **<span class="rpg-token token-d6">k6</span>**.

**Sugerowany rozkład według roli (najprościej):**
- **Szturm:** <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d6">k6</span>
- **Specjalista:** <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">k6</span>
- **Adept:** <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">k6</span>

> Przykład: jeśli masz <span class="rpg-token token-stat">Z</span> = <span class="rpg-token token-d12">k12</span>, to przy strzale, skradaniu i unikach zwykle rzucasz <span class="rpg-token token-d12">k12</span>.

### 1.4 Zasoby

- **<span class="rpg-token token-heart">Serca</span>:** 5.
- **Punkty Mocy (<span class="rpg-token token-power">PM</span>):** 3.
- **Łut Szczęścia (Ł<span class="rpg-token token-stat">S</span>):** na początku każdej sesji masz **2 Ł<span class="rpg-token token-stat">S</span>**.

**Łut Szczęścia (jak działa):** wydaj **1 Ł<span class="rpg-token token-stat">S</span>**, aby wybrać jedno:
- **Przerzut** swojego testu (zostawiasz lepszy wynik), albo
- **Podbicie kości o 1 stopień** na ten jeden rzut (**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>**), albo
- **Zamiana porażki na „sukces z kosztem”** — akcja się udaje, ale MG natychmiast dokłada cenę (np. hałas, utrata czasu, utrata zasobu, gorsza pozycja, przyciągnięcie uwagi, uszkodzenie sprzętu).

**Odzysk Ł<span class="rpg-token token-stat">S</span>:** na początku kolejnej sesji wracasz do limitu. MG może przyznać **+1 Ł<span class="rpg-token token-stat">S</span>** za odważne ryzyko, świetną decyzję fabularną lub granie konsekwencjami.

### 1.5 Talenty (opcjonalne, ale polecane)

Talenty to **2 krótkie hasła**, które opisują, w czym twoja postać jest dobra (bez listy, bez tabel).

- Przykłady: „Mechanik”, „Zwiadowca”, „Negocjator”, „Medyk”, „Haker”, „Weteran”, „Odkrywca”.

**Jak działają Talenty:** jeśli Talent realnie pomaga w teście, MG może **podbić kość o 1 stopień** (albo zneutralizować utrudnienie).
- Talent nie daje automatycznych sukcesów.
- Zwykle **maksymalnie 1 Talent** wpływa na jeden test.

### 1.6 Ekwipunek

Wypisz:
- 1 narzędzie „kluczowe” (broń / zestaw / sprzęt, bez którego nie robisz swojej roboty),
- 1 ochrona (pancerz, tarcza, kamuflaż — zależnie od świata),
- 3 drobiazgi przydatne w przygodzie.

Sprzęt w rdzeniu zasad jest głównie **pozwoleniem** (umożliwia akcje), a nie bonusem liczbowym.

### 1.7 Przykład kompletnej postaci

- Koncept: „<span class="rpg-token token-stat">Z</span>łodziejka informacji, która kradnie dane z systemów, a nie z kieszeni.”
- Rola: Specjalista
- Cechy: <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">k6</span>, <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span>
- Zasoby: 5 Serc, 3 <span class="rpg-token token-power">PM</span>, 2 Ł<span class="rpg-token token-stat">S</span>
- Talenty: „Haker”, „Cień”
- Ekwipunek: pistolet, lekki pancerz, zestaw do włamań, linka, latarka

---



---

### 2. Rdzeń zasad: testy

Ta część jest najważniejsza — jeśli ją rozumiesz, rozumiesz system.

### 2.1 Kiedy robisz test

Test robisz, gdy spełnione są oba warunki:
1) wynik jest niepewny (może się udać albo nie), oraz
2) stawka jest realna (porażka coś zmieni / coś kosztuje).

Jeśli czynność jest banalna i bez presji — MG może powiedzieć „udało się” bez rzutu.

### 2.2 Jak wykonać test (krok po kroku)

1) Gracz mówi **co robi** i **po co**.
2) MG wybiera cechę: **<span class="rpg-token token-stat">S</span>** albo **<span class="rpg-token token-stat">Z</span>** albo **<span class="rpg-token token-stat">M</span>**.
3) MG ustala **Trudność (T)** i mówi, co oznacza porażka (stawka).
4) Gracz rzuca **kością cechy**.
5) Porównaj wynik z T i rozstrzygnij skutki.

### 2.3 Trudności (T)

<span class="rpg-token token-stat">U</span>żywamy prostych progów. Jeśli masz wątpliwość — wybierz niższy próg, a „trudność” pokaż konsekwencją.

- **T 3** – łatwe (prawie na pewno, ale czasem warto sprawdzić pod presją)
- **T 4** – standard (typowe wyzwanie)
- **T 5** – trudne (wymaga kompetencji albo przewagi)
- **T 6** – bardzo trudne (bez przewagi jest ryzykownie)
- **T 8** – heroiczne (dla najlepszych lub po dobrym przygotowaniu)
- **T 12** – legendarne (rzadko „na czysto”; zwykle jako cel kampanijny, plan, rytuał, wielkie warunki)

### 2.4 Wyniki testu

- **Wynik ≥ T → Sukces.** Osiągasz zamierzony efekt.
- **Wynik < T → Porażka.** Nie osiągasz efektu, a sytuacja się zmienia (komplikacja lub koszt).
- **Wyrzucona 1 → Porażka + komplikacja.** Komplikacja wchodzi na pewno.
- **Maksymalny wynik na kości → Sukces wyjątkowy.**
  - Oprócz sukcesu dostajesz **dodatkową korzyść** (szybciej, ciszej, mocniej, bezpieczniej, dodatkowy efekt).

> Przykład sukcesu z kosztem: „Udało ci się sforsować drzwi, ale robisz hałas i ktoś idzie sprawdzić.”

### 2.5 <span class="rpg-token token-stat">U</span>łatwienia i utrudnienia (bez liczenia)

Zamiast dodawać +1/−1 do rzutów, zmieniamy **rozmiar kości**.

- **Lepsza sytuacja** → **podbij kość o 1 stopień**  
  <span class="rpg-token token-d6">k6</span> → <span class="rpg-token token-d8">k8</span> → <span class="rpg-token token-d12">k12</span> → <span class="rpg-token token-d20">k20</span>
- **Gorsza sytuacja** → **obniż kość o 1 stopień**  
  <span class="rpg-token token-d20">k20</span> → <span class="rpg-token token-d12">k12</span> → <span class="rpg-token token-d8">k8</span> → <span class="rpg-token token-d6">k6</span> → <span class="rpg-token token-d4">k4</span>

**Przykłady ułatwień:** przygotowanie, dobre narzędzia, przewaga pozycji, zaskoczenie, wsparcie.  
**Przykłady utrudnień:** ciemność, ślisko, presja czasu, hałas, rozproszenie, osłona.

**Zasada porządku:** dla szybkości przyjmij, że do jednego testu zwykle stosujecie **maksymalnie 1 ułatwienie i 1 utrudnienie** (mogą się znosić).

### 2.6 Pomoc sojusznika

Sojusznik może poświęcić swoją akcję (lub czas w scenie poza walką), aby pomóc.

**Efekt:** na ten jeden test **podbij kość o 1 stopień**.

Pomoc musi być opisana sensownie (osłanianie, podanie narzędzi, odwrócenie uwagi, stabilizacja, wskazówki).

### 2.7 Powtarzanie testów

Jeśli test się nie udał, nie powtarzaj go „w kółko” bez zmiany sytuacji.
- Albo robisz coś inaczej (inna cecha / inne narzędzia / inna droga),
- albo akceptujesz koszt (czas, alarm, zasób),
- albo wycofujesz się.

### 2.8 Przykłady testów (poza walką)

**Przykład A — ciche przejście**
- Gracz: „Przejdę przez podwórze, zanim reflektor wróci.”
- MG: Zręczność (<span class="rpg-token token-stat">Z</span>). To pod presją czasu → Trudność **T 5**.
- Postać ma Talent „Cień” → ułatwienie, kość podbita o 1 stopień.
- Rzut: <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">k12</span> = 4 → porażka. MG: „Nie zauważają cię od razu, ale ktoś słyszy szelest i zaczyna sprawdzać teren (komplikacja: rośnie presja).”

**Przykład B — siłowe forsowanie**
- Gracz: „Wyważę metalowe drzwi, zanim ochrona dojdzie do rogu.”
- MG: Siła (<span class="rpg-token token-stat">S</span>), Trudność **T 6** (bardzo trudne bez narzędzi).
- Ktoś pomaga, przytrzymując zamek i klinując drzwi → kość podbita o 1 stopień.
- Rzut: <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d12">k12</span> = 12 → sukces wyjątkowy: drzwi puszczają natychmiast i robisz to ciszej, niż się spodziewano.

---



---

### 3. Ruch i odległości (siatka jest opcją)

Domyślnie NDE działa bez mapy: opisujesz scenę i pozycje postaci.

### 3.1 Domyślnie: odległości opisowe

<span class="rpg-token token-stat">U</span>żywaj czterech stref:
- **Blisko** — na wyciągnięcie ręki, walka wręcz.
- **Niedaleko** — kilka kroków, łatwy doskok.
- **Daleko** — druga strona sceny, wymaga wyraźnego przemieszczenia.
- **Bardzo daleko** — snajpersko/pojazdowo/„na granicy sceny”.

W turze zwykle możesz zmienić odległość o **jedną strefę** (np. Daleko → Niedaleko).

### 3.2 Opcja: gra na siatce (dla taktyki)

Jeśli wolicie konkrety:
- 1 kratka = 1–2 m.
- Ruch w turze: **do 5 kratek**.
- Skosy są dozwolone (liczą się jak zwykła kratka).

### 3.3 Osłona i linia działania

- **Pełna osłona:** nie da się oddziaływać „po linii” (strzał, obserwacja, wiele mocy).
- **Częściowa osłona:** utrudnia — zwykle **obniża kość o 1 stopień** dla atakującego/obserwującego.

---



---

### 4. Walka

Walka to zwykła scena z testami, tylko uporządkowana w tury.

### 4.1 Kiedy zaczyna się walka

Walka zaczyna się, gdy:
- co najmniej jedna strona chce skrzywdzić drugą, oraz
- ważne jest kto i kiedy działa.

Jeśli sytuacja jest krótka i oczywista, MG może rozstrzygnąć ją jednym testem.

### 4.2 Kolejność tur (prosta wersja)

Najprościej:
- Najpierw działają wszyscy gracze (w dowolnej kolejności),
- potem działają przeciwnicy,
- i tak w pętli.

### 4.3 Co robisz w turze

W swojej turze masz:
- **Przemieszczenie** (zmiana strefy / do 5 kratek w wariancie siatki),
- **1 Akcję** (atak, test, pomoc, użycie mocy, sprzęt, interakcja ze sceną).

### 4.4 Atak: jak to działa

1) Wybierz cel i opisz atak.
2) Wybierz cechę:
   - **wręcz** → rzut **Siły (<span class="rpg-token token-stat">S</span>)**,
   - **dystans** → rzut **Zręczności (<span class="rpg-token token-stat">Z</span>)**,
   - **moce** → zwykle rzut **Mocy (<span class="rpg-token token-stat">M</span>)** (patrz rozdział 5).
3) Ustal **Obronę** celu.
4) Rzuć kością i porównaj z Obroną.

### 4.6 Obrażenia i „ile wytrzymują”

- Trafienie zadaje **1 Serce**.
- **Sukces wyjątkowy** zadaje **2 <span class="rpg-token token-heart">Serca</span>** *albo* daje silny efekt (rozbrojenie, przewrócenie, wypchnięcie z osłony) — wybierz jedno.

Najprostsze archetypy wrogów:
- **Pachołek:** odpada po 1 trafieniu.
- **Elita:** ma **2 <span class="rpg-token token-heart">Serca</span>**.
- **Boss:** ma **3 <span class="rpg-token token-heart">Serca</span>** (lub 5 w scenach finałowych).

> Uwaga: „odpada” nie musi oznaczać śmierci. Może być nieprzytomny, uciekł, poddał się, został wyłączony z akcji.

### 4.5 Obrona przeciwników (orientacyjnie)

- **<span class="rpg-token token-stat">S</span>łaby:** Obrona **4**
- **Typowy:** Obrona **5**
- **Elita:** Obrona **6**
- **Boss:** Obrona **8** (legendarny boss: **12**)

Osłona i warunki zwykle zmieniają rozmiar kości atakującego (ułatwienia/utrudnienia), a nie Obrony.

### (OUTDATED)

_Treść usunięta w wersji 1.4_

### (OUTDATED)

_Treść usunięta w wersji 1.4_

### 4.7 Przykłady walki

**Przykład A — walka wręcz z pachołkiem**
- Szturm (<span class="rpg-token token-stat">S</span> <span class="rpg-token token-d12">k12</span>) atakuje pachołka (Obrona 5).
- Warunki są dobre (zaskoczenie) → kość podbita o 1 stopień, ale już jest <span class="rpg-token token-d12">k12</span>, więc podbicie daje <span class="rpg-token token-d20">k20</span>.
- Rzut <span class="rpg-token token-d20">k20</span> = 7 → trafienie, pachołek odpada.

**Przykład B — strzał w elitę zza osłony**
- Specjalista (<span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">k12</span>) strzela do elity (Obrona 6).
- Cel jest w częściowej osłonie → utrudnienie, kość spada na <span class="rpg-token token-d8">k8</span>.
- Rzut <span class="rpg-token token-d8">k8</span> = 6 → trafienie, elita traci 1 Serce (zostaje jej 1).

**Przykład C — boss i Łut Szczęścia**
- Adept (<span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">k12</span>) próbuje obezwładnić bossa (Obrona 8) mocą.
- Rzut <span class="rpg-token token-d12">k12</span> = 4 → porażka. Gracz wydaje 1 Ł<span class="rpg-token token-stat">S</span> na przerzut.
- Przerzut = 10 → sukces. Boss traci 1 Serce, ale MG dokłada koszt: „efekt jest głośny, włącza się alarm.”

---



---

### 5. Moce (<span class="rpg-token token-stat">M</span>) i Punkty Mocy (<span class="rpg-token token-power">PM</span>)

W NDE „Moc” to kategoria efektów specjalnych. W zależności od świata może oznaczać:
- magię, psionikę, rytuały,
- zaawansowaną technologię, drony, hacking „na żywo”,
- filmowe zagrania bohaterów (np. „mistrzowska koncentracja”),
- wpływ społeczny w grach, gdzie rozmowa jest „mocą”.

### 5.1 Kiedy wydajesz <span class="rpg-token token-power">PM</span>

Wydajesz <span class="rpg-token token-power">PM</span>, gdy próbujesz uzyskać efekt **ponad standard**.

---

### 5.2 Jak użyć mocy (krok po kroku)

1) Opisz efekt, który chcesz uzyskać.
2) MG ustala Trudność i koszt <span class="rpg-token token-power">PM</span>.
3) Wydaj <span class="rpg-token token-power">PM</span>.
4) Rzuć **<span class="rpg-token token-stat">M</span>** i porównaj do Trudności.

**Porażka:** efekt nie działa; <span class="rpg-token token-power">PM</span> przepada; wchodzi komplikacja (przeciążenie, ślad, ujawnienie, efekt uboczny).

### 5.3 Poziomy efektów (Trudność / koszt)

- **Sztuczka** (krótki trik): **T 4 / 0–1 <span class="rpg-token token-power">PM</span>**  
  światło, dźwięk, drobna zasłona, chwilowe rozproszenie.
- **Standard**: **T 5 / 1 <span class="rpg-token token-power">PM</span>**  
  pocisk, tarcza, impuls, skok, wzmocnienie.
- **Silna**: **T 6 / 2 <span class="rpg-token token-power">PM</span>**  
  obszar, kontrola, leczenie, paraliż, „hack w trakcie walki”.
- **Wielka**: **T 8–12 / 3 <span class="rpg-token token-power">PM</span>**  
  efekt, który zmienia scenę lub ma konsekwencje kampanijne.

### 5.4 Sukces wyjątkowy w mocy

Jeśli wyrzucisz maks na kości <span class="rpg-token token-stat">M</span>:
- zwiększ skalę (większy obszar / dłużej / mocniej), albo
- dodaj dodatkową korzyść (ciszej, precyzyjniej, bezpieczniej), albo
- MG może zwrócić **1 <span class="rpg-token token-power">PM</span>** (jeśli pasuje do fikcji).

### 5.5 Odzysk <span class="rpg-token token-power">PM</span>

- Po scenie konfliktu odzyskujesz **1 <span class="rpg-token token-power">PM</span>**.
- Po bezpiecznym odpoczynku wracasz do pełna.

### 5.6 Przykłady mocy

**Przykład A — tarcza na dobiegnięcie**
- Gracz: „Stawiam krótką osłonę, żeby przebiec na lepszą pozycję.”
- MG: Standard **T 5**, koszt 1 <span class="rpg-token token-power">PM</span>.
- Rzut <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">k12</span> = 9 → sukces: przebiegasz bezpiecznie.

**Przykład B — porażka z konsekwencją**
- Gracz: „Zatrzymuję elitę na miejscu.”
- MG: Silna **T 6**, koszt 2 <span class="rpg-token token-power">PM</span>.
- Rzut = 1 → porażka + komplikacja: tracisz 2 <span class="rpg-token token-power">PM</span>, a efekt odbija i zdradza twoją pozycję.

---



---

### 6.1 0 Serc

Jeśli spadniesz do 0 Serc:
- jesteś **wyłączony z akcji** (raniony, ogłuszony, w szoku — zależnie od konwencji),
- sojusznik może poświęcić akcję, aby postawić cię na nogi z **1 Sercem**.

### 6.2 Odpoczynek

- Po scenie konfliktu, jeśli macie chwilę oddechu i podstawowe warunki, możecie wrócić do pełnych Serc.
- W surowszych kampaniach MG może wymagać bezpiecznego postoju, aby wrócić do pełni.

---

### (OUTDATED)

_Treść usunięta w wersji 1.4_



---

### 7. Rozwój postaci

**Kiedy rośniesz:** po przygodzie, misji lub ważnym rozdziale fabuły (zwykle co 1–3 sesje).

Wybierz **jedno**:
- **Podbij** jedną cechę o 1 stopień kości (maks. do <span class="rpg-token token-d20">k20</span>), albo
- **+1 Serce** (maks. 7), albo
- **+1 <span class="rpg-token token-power">PM</span>** (maks. 5), albo
- **Nowy Atut** (jednozdaniowa, konkretna zdolność uzgodniona z MG).

> Przykład: Specjalista podbija <span class="rpg-token token-stat">Z</span> z <span class="rpg-token token-d12">k12</span> do <span class="rpg-token token-d20">k20</span>, bo kampania weszła w etap pościgów i strzelanin.

---



---

### 8. Wariant tylko <span class="rpg-token token-d6">k6</span>: 2k6

Jeśli nie chcecie używać różnych kości, grajcie na **2k6**.

### 8.1 Cechy jako modyfikatory

Zamiast rozmiarów kości, rozdziel modyfikatory:
- jedna cecha ma **+2**
- jedna ma **+1**
- jedna ma **+0**

### 8.2 Test

Rzuć **2k6 + modyfikator cechy**.

**Wynik:**
- **6 lub mniej** – porażka z konsekwencją
- **7–9** – sukces z kosztem
- **10+** – pełny sukces
- **12** – sukces wyjątkowy (dodatkowa korzyść)

### 8.3 Trudność sytuacji

Zamiast zmieniać progi, dawaj:
- **+1** za przewagę, przygotowanie, dobry plan,
- **−1** za utrudnienia, presję, osłonę, chaos.

### 8.4 Łut Szczęścia w 2k6

Wydaj 1 Ł<span class="rpg-token token-stat">S</span>, aby:
- przerzucić 2k6, albo
- dodać **+1** do wyniku testu, albo
- zamienić porażkę na sukces z kosztem.

### 8.5 Szybkie mapowanie (opcjonalnie)

Jeśli kiedyś chcesz „przeliczyć” postać między wariantami:
- <span class="rpg-token token-d6">k6</span> ≈ +0
- <span class="rpg-token token-d8">k8</span> ≈ +1
- <span class="rpg-token token-d12">k12</span> ≈ +2
- <span class="rpg-token token-d20">k20</span> ≈ +3 (dla bardzo doświadczonych)

---



---

### (OUTDATED)

_Treść usunięta w wersji 1.4_



---

### 9.1 Ochrona (pancerz) jako prosty zasób

Jeśli chcesz, żeby „ochrona” miała wyraźny efekt:
- postać z ochroną ma **1 żeton Pancerza na scenę**,
- gdy miałaby stracić 1 Serce, może zamiast tego zużyć żeton Pancerza.

### 9.2 Presja czasu jako stoper

Jeśli scena ma limit czasu, MG ustala „licznik” (np. 3 kroki). Każda porażka przesuwa licznik o 1. Gdy dojdzie do końca — wydarza się konsekwencja (alarm, ucieczka celu, zawalenie przejścia).

---

### 9.3 Odwet (wariant ryzykownej walki)

Jeśli chcesz, żeby walka była bardziej „ostra” i szybka:
- gdy **atakujesz wręcz** i **pudłujesz**, tracisz **1 Serce**, o ile przeciwnik mógł cię realnie dosięgnąć.
To jest wariant — w rdzeniu NDE konsekwencje porażek w walce wynikają głównie z fikcji i decyzji MG.

