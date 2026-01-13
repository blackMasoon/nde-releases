---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.3
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
generated_at: "2026-01-13T12:23:01.214Z"
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
# Księga Mistrza Gry



---



---

### Jasno komunikuj stawkę.

- **Jasno komunikuj stawkę.** Zanim padnie rzut, powiedz: cecha, <span class="rpg-token token-tn">TN</span>, skutek porażki, szansa pomocy.
- **Opis → mechanika → rezultat.** Zawsze zaczynaj od fikcji, dopiero potem rzut.
- **Szybkie sceny.** Utrzymuj tempo: jeden test = jeden sensowny efekt.
- **Porażka pcha akcję.** Komplikacja zmienia sytuację, a nie „resetuje” scenę.
- **Spójność.** Te same okoliczności → te same <span class="rpg-token token-tn">TN</span> i skutki.




---

1) Gracz mówi, co robi i co chce osiągnąć.
2) Wybierz cechę: **S** (siłowe), **Z** (precyzyjne/szybkie), **M** (specjalne efekty).
3) Ustal **<span class="rpg-token token-tn">TN</span>**: 4 łatwe, 6 normalne, 8 trudne, 12 bohaterskie.
4) Powiedz, co grozi przy porażce i czy ktoś może **pomóc** (podbicie kości o 1 rozmiar).
5) Gracz rzuca kością cechy i porównuje do <span class="rpg-token token-tn">TN</span>.
6) Rozstrzygnij wynik i zaktualizuj sytuację.

Skrót dla stołu: „Cechy/<span class="rpg-token token-tn">TN</span>/Rzut/Skutek”.




---

### 4 (łatwe):

- **4 (łatwe):** warunki sprzyjają, cel nie stawia oporu.
- **6 (normalne):** standard w przygodzie bez przewagi.
- **8 (trudne):** presja czasu, zła pozycja, osłona, złożone narzędzia.
- **12 (bohaterskie):** ponadprzeciętne wyzwanie; zwykle wymaga przygotowania lub wysokiej kości.

Modyfikacja sytuacyjna: przesuwaj <span class="rpg-token token-tn">TN</span> **o 1 stopień** (maks. o 2 w skrajnościach).
- Gorsze: ciemno, ślisko, osłona, alarm → <span class="rpg-token token-tn">TN</span> +1.
- Lepsze: czas, narzędzia, przewaga pozycji, zaskoczenie → <span class="rpg-token token-tn">TN</span> −1.

Szybkie intuicje skuteczności (przybliżenia):
- <span class="rpg-token token-d6">d6</span> vs TN6 ≈ 17%; <span class="rpg-token token-d8">d8</span> vs 6 ≈ 38%; <span class="rpg-token token-d10">d10</span> vs 6 ≈ 50%; <span class="rpg-token token-d12">d12</span> vs 6 ≈ 58%.
- <span class="rpg-token token-d10">d10</span> vs TN8 ≈ 30%; <span class="rpg-token token-d12">d12</span> vs 8 ≈ 42%; <span class="rpg-token token-d20">d20</span> vs 12 ≈ 45%.
Używaj tych liczb orientacyjnie, nie licz na bieżąco.

Kiedy nie rzucać:
- Gdy wynik jest oczywisty i nie ma stawki.
- Gdy rzut niczego nie zmieni (lepiej przejść do kolejnego wyzwania).




---

### 1 na kości

- **1 na kości**: porażka + komplikacja. Przykłady: hałas, strata czasu, zły trop, drobna rana (−1 Serce), utracony zasób, gorsza pozycja.
- **Porażka (wynik < <span class="rpg-token token-tn">TN</span>)**: brak efektu oraz ewentualny „odwet” (w walce) lub postęp zagrożenia (poza walką).
- **Sukces wyjątkowy (maks na kości)**: sukces + dodatkowa korzyść: szybciej/ciszej/bez kosztu/większy efekt.

Checklista tworzenia komplikacji:
1) Uderz w zasób (czas, pozycja, serca, mana, ekwipunek).
2) Zmień układ na planszy (nowe przeszkody, odcięte drogi, wzmocnione osłony).
3) Podnieś presję (licznik, alarm, wzmocnienie przeciwników).




---

### Ruch:

- **Ruch:** do 5 kratek w turze; wolno po skosie.
- **Osłona:** częściowa → ataki dystansowe <span class="rpg-token token-tn">TN</span> +1; pełna → brak linii działania.
- **Teren utrudniony (opcjonalnie):** wejście na kratkę kosztuje 2 z 5 punktów ruchu.
- **Wypychanie/przesuwanie:** test S vs <span class="rpg-token token-tn">TN</span> 6 (modyfikuj sytuacją). Sukces: przesuń cel 1–2 kratki; wyjątkowy: +1 kratka.
- **Zasięgi:** przyjmij do 10 kratek jako „bez kary”; dalej → <span class="rpg-token token-tn">TN</span> +1.
Szybkość jest ważniejsza od drobiazgowego liczenia — trzymaj zasady lekkie.




---

### Kolejność:

- **Kolejność:** gracze → przeciwnicy → powtórz.
- **Atak:** wręcz = S, dystans = Z; <span class="rpg-token token-tn">TN</span> przeciwnika: pachołek 6, elita 8, boss 12.
- **Trafienie:** pachołek schodzi; elita/boss dostaje 1 Ranę (boss ma 3). Wyjątkowy sukces = zwykle 2 Rany.
- **Pudło:** jeśli przeciwnik mógł dosięgnąć → bohater traci 1 Serce (odwet). W osłonie/daleko — zwykle brak odwetu.

Skalowanie presji:
- Wielu pachołków „na zwarciu” → <span class="rpg-token token-tn">TN</span> +1 lub dodatkowa komplikacja przy pudle.
- Zmieniaj teren co turę: pojawiają się przeszkody, wąskie gardła, okazje do przewagi.




---

Buduj sceny w 5 krokach:
1) **Cel**: po co scena (np. przejście, zdobycie rzeczy, wyłączenie zagrożenia).
2) **Przeszkody**: 2–3 różne typy (straż, zamek, alarm, niebezpieczny teren).
3) **Zagrożenie**: pachołki/elita/boss, hazardy, pułapki.
4) **Licznik (opcjonalnie)**: 3–5 kroków; porażki go przesuwają; na końcu zły skutek.
5) **Nagroda/konsekwencja**: co da sukces, co zmieni porażka.

Progi wielkości starcia (dla 3–5 bohaterów):
- **Łatwe:** 3–5 pachołków lub elita bez wsparcia.
- **Standard:** 6–8 pachołków lub elita + 2–4 pachołki.
- **Trudne:** boss + 2–4 pachołki lub 2 elity + 3–5 pachołków.
- **Bohaterskie:** boss + 4–6 pachołków i/lub elita.
Dostosuj do stołu: teren i osłony mają duży wpływ.




---

Format (przykładowy, bez klimatu):
> **Nazwa — <span class="rpg-token token-tn">TN</span>, Rany, Taktyka, Specjal**
- **Pachołek:** <span class="rpg-token token-tn">TN</span> 6, bez Ran; taktyka prosta.
- **Elita:** <span class="rpg-token token-tn">TN</span> 8, 2 Rany; ma wyraźną przewagę (np. mobilność, osłona, kontrola pola).
- **Boss:** <span class="rpg-token token-tn">TN</span> 12, 3 Rany; 1–2 unikalne ruchy (np. odepchnięcie, przyzwanie wsparcia).

Reakcja i morale (lekki system):
- Gdy pierwszy pachołek padnie lub elita dostanie Ranę, rzuć **<span class="rpg-token token-d6">d6</span>**:
  - 1–2: wycofanie/przyczajenie; 3–4: trzymają pozycję; 5–6: nacierają.
- Modyfikuj ±1 za przewagę/strach/bossa w pobliżu.




---

Magia to „efekty specjalne”. Przydziel <span class="rpg-token token-tn">TN</span> i koszt Many wg skali:
- **Sztuczka:** <span class="rpg-token token-tn">TN</span> 4, koszt 0–1 (krótki, mały efekt).
- **Standard:** <span class="rpg-token token-tn">TN</span> 6, koszt 1 (pojedynczy cel, krótki skok, bariera).
- **Silny:** <span class="rpg-token token-tn">TN</span> 8, koszt 2 (obszar, kontrola, leczenie +2 Serca).
- **Wielka moc:** <span class="rpg-token token-tn">TN</span> 12, koszt 3 (efekt sceniczny).

Zasady pomocnicze:
- **Wiele celów:** albo +1 koszt Many, albo <span class="rpg-token token-tn">TN</span> +1 stopień.
- **Utrzymanie efektu:** co turę płać 1 Manę lub zajmuje Akcję.
- **Kontratak/unik czaru:** pozwól wykonać odpowiedni test bohatera (Z lub M) przeciw temu samemu <span class="rpg-token token-tn">TN</span>, aby zredukować lub uniknąć efektu (w zależności od fikcji).




---

### Skrytobójstwo/przemykanie:** ustaw „poziom alarmu” jako **licznik 3–5

- **Skrytobójstwo/przemykanie:** ustaw „poziom alarmu” jako **licznik 3–5**; porażki go podnoszą; po osiągnięciu maksimum pojawia się patrol, zamek się rygluje itp.
- **Pościg:** określ dystans w „krokach pościgu” (np. 3). Każda tura: obie strony testują; sukces ścigającego skraca, uciekającego wydłuża. Gdy dojdzie do 0 → dogonienie; przy 5 → ucieczka.
- **Przeszkody środowiska:** jasno komunikuj koszt ryzyka (np. spadek = −1 Serce i gorsza pozycja), <span class="rpg-token token-tn">TN</span> zależne od opisów.




---

### Rozwój:

- **Rozwój:** po przygodzie każdy wybiera jedno: podbicie rozmiaru kości cechy, +1 Serce (max 7) lub +1 Mana (max 5).
- **Nagrody rzeczowe:** dają „pozwolenia” (nowe działania) lub jednorazowe przewagi („raz na scenę obniż <span class="rpg-token token-tn">TN</span> o 1”). Unikaj stałych modyfikatorów.
- **Ekonomia (opcjonalna):** proste progi: tani/standard/drogi — rozstrzygaj testem zasobów zamiast liczyć walutę.




---

- Ustal z graczami zakres treści (co jest OK, czego unikamy).
- Umów się na prosty sygnał „stop”/„przewiń” dla niekomfortowych sytuacji.
- Konflikty rozgrywaj w fikcji, nie przy stole.




---

1) **Hak:** jednozdaniowy problem.
2) **3 miejsca** z cechami taktycznymi (osłony, wysokości, wąskie przejścia).
3) **3 przeszkody:** zamek, straż, zagrożenie środowiskowe.
4) **Zasoby w stawce:** czas, hałas, uwaga przeciwnika.
5) **Lista komplikacji** (5 szt.) i **licznik** do sceny.
6) **Przeciwnicy:** wpisy 1‑linijkowe (pachołki/elita/boss) + prosta taktyka.




---

Komplikacje — <span class="rpg-token token-d6">d6</span> (uniwersalne):
1. Utrata czasu / przewaga przeciwnika.
2. Ujawnienie pozycji / wzrost alarmu.
3. Drobna szkoda: −1 Serce lub zasób.
4. Zła pozycja: wypchnięcie/utknięcie.
5. Utrata/zakleszczenie sprzętu.
6. Nowe zagrożenie pojawia się w scenie.

Korzyści przy sukcesie wyjątkowym — <span class="rpg-token token-d6">d6</span>:
1. Szybciej.
2. Ciszej.
3. Bez kosztu (np. bez Many/bez odwetu).
4. Większy efekt (obszar/zasięg).
5. Lepsza pozycja sojuszników.
6. Dodatkowa wskazówka/informacja.




---

### Cel graczy

- Cel graczy: przejść przez zabezpieczone przejście.
- MG: zamek (<span class="rpg-token token-tn">TN</span> 6), patrol (licznik 3), wąskie przejście (osłony).
1) Gracz A: „Otwieram zamek” (Z, <span class="rpg-token token-tn">TN</span> 6). Porażka = +1 do licznika. Rzut 5 → porażka, licznik 1/3.
2) Gracz B pomaga (podbija kość). A: ponownie (nowe narzędzia, lepsza pozycja), rzut <span class="rpg-token token-d12">d12</span>=9 → sukces.
3) Patrol zbliża się (licznik 2/3). Gracz C osłania wyjście (S, <span class="rpg-token token-tn">TN</span> 6). Wyjątkowy sukces → przewaga pozycji dla drużyny.
Scena rozstrzygnięta szybko, z czytelnymi stawkami.

---
To wszystko, czego potrzebujesz do prowadzenia. Reszta (świat, potwory, skarby) jest modułowa i powinna być dopasowana do wybranego uniwersum. 

