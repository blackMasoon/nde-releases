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
generated_at: "2026-01-12T20:14:22.095Z"
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
# Księga Potworów



---



---

- Używamy tych samych pojęć co w podstawowych zasadach i księdze MG.
- **Tylko gracze rzucają.** Przeciwnicy wywierają presję poprzez <span class="rpg-token token-tn">TN</span> i ruchy; obrażenia zwykle wynikają z „odwetu” lub testów wymuszonych na graczach.




---

> Nazwa — Klasa, <span class="rpg-token token-tn">TN</span>, Rany, Rola, Ruch, Specjal

- **Klasa:** Pachołek | Elita | Boss
- **<span class="rpg-token token-tn">TN</span>:** liczba 4/6/8/12 określająca trudność trafienia/obejścia przeciwnika.
- **Rany:** tylko dla Elity i Bossa (Elita: 2, Boss: 3 domyślnie). Pachołek nie ma Ran (schodzi po trafieniu).
- **Rola:** Brute (bijatyka), Skirmisher (mobilny), Artillery (dystans), Controller (kontrola pola), Support (wsparcie).
- **Ruch:** domyślnie 5 kratek. Zmień, jeśli mobilność jest unikalna (np. 6 Szybki, Latanie, Skok 3).
- **Specjal:** 1–2 krótkie zdolności opisowe (patrz sekcje „Cechy” i „Ruchy”).

Przykład zapisu: „Strażnik Elitarny — Elita, <span class="rpg-token token-tn">TN</span> 8, Rany 2, Brute, Ruch 5, Specjal: Osłona Ciężka; Napór”.




---

### Pachołek (minion):

- **Pachołek (minion):** <span class="rpg-token token-tn">TN</span> 6, schodzi po 1 trafieniu. W ilości tworzą presję. Odwet przy pudle: −1 Serce.
- **Elita:** <span class="rpg-token token-tn">TN</span> 8, 2 Rany. Zwykle ma 1 cechę defensywną lub mobilność. Odwet przy pudle: −1 Serce; czasem dodatkowy skutek sytuacyjny.
- **Boss:** <span class="rpg-token token-tn">TN</span> 12, 3 Rany. Ma 2–3 ruchy specjalne i wpływa na teren/tempo. Może wywoływać testy na graczach (np. unik, stabilizacja).




---

### Brute (walka wręcz):

- **Brute (walka wręcz):** naciska w zwarciu, wypycha z osłon.
- **Skirmisher (mobilny):** wchodzi/wychodzi z kontaktu, karze za samotność.
- **Artillery (dystans):** strzela zza osłon, zmusza do ruchu.
- **Controller (kontrola):** tworzy strefy zagrożeń, dymy, pola wypychające.
- **Support (wsparcie):** wzmacnia sojuszników, obniża <span class="rpg-token token-tn">TN</span> sojuszników lub podnosi <span class="rpg-token token-tn">TN</span> bohaterów o 1 stopień sytuacyjnie.




---

Dodaj 1–2 do statblocka. Zawsze działają opisowo; zmieniają <span class="rpg-token token-tn">TN</span> o 1 stopień tylko gdy ma to sens.
- **Osłona Naturalna:** w zasięgu dystansowym przeciwnik zwykle ma częściową osłonę (atak na niego → <span class="rpg-token token-tn">TN</span> +1 stopień).
- **Pancerz Lekki:** pierwsza utrata 1 Serca z odwetu na tej jednostce w scenie jest ignorowana.
- **Twardy:** pierwszy sukces przeciw tej jednostce nie zadaje Rany (tylko odrzuca/pozycja) — dobre dla bossów.
- **Szybki (Ruch 6):** ignoruje 1 kratkę terenu utrudnionego na turę.
- **Wspinacz/Skoczek:** porusza się pionowo/po przeszkodach jak po płaskim, skok 3 kratek.
- **Latanie:** ignoruje przeszkody terenowe (MG dba o sensowne osłony).
- **Zwiadowca:** trudniej go zaskoczyć; pierwsza próba skradania przeciw niemu ma <span class="rpg-token token-tn">TN</span> +1.
- **Odporność [typ]:** pierwszy efekt danego typu w scenie jest zredukowany (MG wyjaśnia: słabszy zasięg, krótszy czas).
- **Wrażliwość [typ]:** przeciw temu typowi ataków <span class="rpg-token token-tn">TN</span> o 1 stopień niższe.
- **Roje:** gdy stoi obok celu, odwet na pudle może dotknąć dwóch bohaterów w zasięgu 1.




---

Wybierz 1–2 charakterystyczne. Ruchy opisują efekt; jeśli grożą bohaterom, MG może kazać im wykonać odpowiedni test (Z lub M) przeciw <span class="rpg-token token-tn">TN</span> przeciwnika.
- **Napór (Brute):** po trafieniu bohatera, dodatkowo przesuń go o 1–2 kratki.
- **Zerwanie Osłony:** gdy ta jednostka trafi, osłona celu przestaje działać do końca następnej tury.
- **Szarpnięcie (Skirmisher):** wejście/wyjście ze zwarcia nie prowokuje odwetu.
- **Salwa (Artillery):** obszar 3×3; wszyscy w obszarze test Z przeciw <span class="rpg-token token-tn">TN</span>; porażka: −1 Serce i wypchnięcie o 1 kratkę.
- **Kotwica (Controller):** pole 3×3 staje się „lepki teren” (wejście kosztuje całą Akcję) do końca następnej tury.
- **Wzmocnienie (Support):** jeden sojusznik do końca rundy ma łatwiej o 1 stopień (atakujący w niego mają <span class="rpg-token token-tn">TN</span> +1).
- **Przyzwanie (Boss):** raz na starcie przywołuje 2 pachołków w wolnych kratkach.
- **Bariera (Boss):** do końca kolejki boskiej strony bohaterowie wykonują ataki dystansowe na <span class="rpg-token token-tn">TN</span> +1.
- **Wstrząs (Boss):** wszyscy w zasięgu 2 kratek test S vs <span class="rpg-token token-tn">TN</span>; porażka: −1 Serce lub powalenie (tracisz Ruch w tej turze).




---

1) **Wybierz klasę:** Pachołek / Elita (2 Rany) / Boss (3 Rany).
2) **Ustaw <span class="rpg-token token-tn">TN</span>:** 6 / 8 / 12 (wyjątkowo 4 dla bardzo słabych lub 10 dla twardych elit).
3) **Nadaj rolę:** Brute, Skirmisher, Artillery, Controller, Support.
4) **Dodaj 1–2 cechy** i **1 ruch specjalny** (Boss: 2–3 ruchy).
5) **Ruch:** zwykle 5; zmień tylko, jeśli to kluczowe.

Gotowe. Ten szkielet działa we wszystkich realiach.




---

Poniższe wpisy podmieniaj nazwami/kolorami świata.


### 7.1 Pachołki
- **Strażnik Pachołek — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Brute, Ruch 5, Specjal: Osłona Naturalna.**
- **Zwiadowca Pachołek — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Skirmisher, Ruch 6, Specjal: Zwiadowca.**
- **Strzelec Pachołek — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Artillery, Ruch 5, Specjal: Salwa (mały obszar 2×2, tylko ostrzega: na porażce −1 Serce).**
- **Kontroler Pachołek — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Controller, Ruch 5, Specjal: Kotwica (na 1 turę, jednorazowo).**
- **Wsparcie Pachołek — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Support, Ruch 5, Specjal: Wzmocnienie (raz na scenę).**


### 7.2 Elity
- **Strażnik Elitarny — Elita, <span class="rpg-token token-tn">TN</span> 8, Rany 2, Brute, Ruch 5, Specjal: Pancerz Lekki; Napór.**
- **Skrytobójca Elitarny — Elita, <span class="rpg-token token-tn">TN</span> 8, Rany 2, Skirmisher, Ruch 6, Specjal: Szarpnięcie; Wrażliwość [obserwacja] (łatwiej go wykryć).**
- **Strzelec Elitarny — Elita, <span class="rpg-token token-tn">TN</span> 8, Rany 2, Artillery, Ruch 5, Specjal: Osłona Naturalna; Salwa (3×3 po przygotowaniu).**
- **Kontroler Elitarny — Elita, <span class="rpg-token token-tn">TN</span> 8, Rany 2, Controller, Ruch 5, Specjal: Kotwica; Wypchnięcie o 1 kratkę przy sukcesie wyjątkowym.**
- **Medyk Elitarny — Elita, <span class="rpg-token token-tn">TN</span> 8, Rany 2, Support, Ruch 5, Specjal: Wzmocnienie; przy trafieniu cofa 1 komplikację sojusznika (opisowo).**


### 7.3 Bossowie
- **Przywódca — Boss, <span class="rpg-token token-tn">TN</span> 12, Rany 3, Support, Ruch 5, Specjal: Przyzwanie; Wzmocnienie; Bariera.**
- **Kolos — Boss, <span class="rpg-token token-tn">TN</span> 12, Rany 3, Brute, Ruch 5, Specjal: Napór (do 2 kratek); Twardy; Wstrząs.**
- **Łowca — Boss, <span class="rpg-token token-tn">TN</span> 12, Rany 3, Skirmisher, Ruch 6, Specjal: Szarpnięcie; Zwiadowca; Salwa (skokowa — po ruchu).**
- **Taktik — Boss, <span class="rpg-token token-tn">TN</span> 12, Rany 3, Controller, Ruch 5, Specjal: Kotwica (utrzymanie za 1 Manę/zasób tury); Bariera; Przyzwanie (1 pachołek/ turę do maks 3).**




---

Hazard to „bezmyślny przeciwnik” lub efekt środowiskowy. Działa turami albo na wyzwalacz.
Format: **Nazwa — <span class="rpg-token token-tn">TN</span>, Efekt, Jak wyłączyć**
- **Wieżyczka — <span class="rpg-token token-tn">TN</span> 8, Efekt: przy turze przeciwników każdy w linii strzału test Z vs <span class="rpg-token token-tn">TN</span>, porażka: −1 Serce; Wyłączenie: test M lub Z <span class="rpg-token token-tn">TN</span> 8 przy panelu.**
- **Zatrzask — <span class="rpg-token token-tn">TN</span> 6, Efekt: wejście w pole wymusza test Z; porażka: unieruchomienie lub −1 Serce; Wyłączenie: Z <span class="rpg-token token-tn">TN</span> 6 z narzędziami.**
- **Pole Repulsyjne — <span class="rpg-token token-tn">TN</span> 8, Efekt: na początku tury przesuwa o 2 kratki w kierunku krawędzi; Wyłączenie: M <span class="rpg-token token-tn">TN</span> 8 (rozproszenie) lub odcięcie zasilania (S <span class="rpg-token token-tn">TN</span> 6).**
- **Gaz/Dym — <span class="rpg-token token-tn">TN</span> 6, Efekt: w obszarze 3×3 test M lub Z; porażka: ślepa plamka/−1 Serce; Wyłączenie: przewietrzenie (S) lub uszczelnienie (Z).**




---

Wybierz 1 z każdego wiersza (lub rzuć <span class="rpg-token token-d6">d6</span>):
1. Cel sceny: przejście / odzyskanie / wyłączenie / eskortowanie / kradzież / obrona
2. Teren wiodący: otwarty / wąskie korytarze / wielopoziom / osłony modułowe / niebezpieczne krawędzie / mgła-dym
3. Przeciwnicy: 6× pachołek / 4× pachołek + elita / 2× elita / boss / boss + 2× pachołek / elita + hazard
4. Przewaga przeciwnika: osłona / wysokość / mobilność / licznik czasu / wąskie gardła / wsparcie odległe
5. Przewaga graczy: zaskoczenie / wyższy poziom / narzędzia / krótka bariera / skrót / sojusznik neutralny




---

Zamiast <span class="rpg-token token-tn">TN</span> liczbowych użyj stopni:
- **Pachołek:** „Normalne” (odpowiednik <span class="rpg-token token-tn">TN</span> 6)
- **Elita:** „Trudne” (+1 stopień)
- **Boss:** „Bohaterskie” (+2 stopnie) i 3 Rany
Cechy i ruchy działają tak samo; gdy „<span class="rpg-token token-tn">TN</span> +1” w opisie, podnieś stopień.




---

### Jeśli walka trwa za krótko

- Jeśli walka trwa za krótko: dodaj pachołków falami (2/ turę) lub podnieś <span class="rpg-token token-tn">TN</span> o 1 stopień na rzecz przeciwników mających przewagę pozycji.
- Jeśli walka dłuży się: pozwól na sukces wyjątkowy częściej przez tworzenie okazji (lepsza pozycja), albo obniż <span class="rpg-token token-tn">TN</span> osłabionym wrogom.
- Dwie elity ≈ mały boss; boss + 4 pachołki ≈ starcie finałowe na sesję 2‑godzinną.




---

### Straż Obronny — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Artillery, Ruch 5, Specjal: Osłona Naturalna.

- **Straż Obronny — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Artillery, Ruch 5, Specjal: Osłona Naturalna.**
- **Patrol Mobilny — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Skirmisher, Ruch 6, Specjal: Zwiadowca.**
- **Ciężki Szturm — Elita, <span class="rpg-token token-tn">TN</span> 8, Rany 2, Brute, Ruch 5, Specjal: Pancerz Lekki; Napór.**
- **Taktyk Pola — Elita, <span class="rpg-token token-tn">TN</span> 8, Rany 2, Controller, Ruch 5, Specjal: Kotwica; Wzmocnienie.**
- **Przywódca Polowy — Boss, <span class="rpg-token token-tn">TN</span> 12, Rany 3, Support, Ruch 5, Specjal: Przyzwanie; Bariera; Wzmocnienie.**
- **Kolos Terenowy — Boss, <span class="rpg-token token-tn">TN</span> 12, Rany 3, Brute, Ruch 5, Specjal: Twardy; Wstrząs; Napór.**

---
To zestaw narzędzi do szybkiego tworzenia przeciwników. Ustal <span class="rpg-token token-tn">TN</span>, wybierz klasę i rolę, dodaj 1–2 cechy oraz ruch — i masz grywalnego wroga gotowego na planszę.

