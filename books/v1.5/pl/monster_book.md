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
generated_at: "2026-01-16T08:50:46.404Z"
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
# Księga Potworów



---



---

### Po co jest ta księga

Ta księga jest zestawem **narzędzi** do budowania przeciwników i zagrożeń w NDE:
- szybko (w 2–5 minut),
- bez liczenia współczynników,
- w sposób spójny z zasadami z **Basic Rules** i **Księgi MG**.

**Najważniejsze założenie NDE:** *tylko gracze rzucają kośćmi.*  
Przeciwnicy nie „atakują rzutem” — atakują **presją w fikcji**: stawiają przeszkody, wymuszają testy, tworzą zagrożenia i konsekwencje.

---



---

### 0. <span class="rpg-token token-stat">S</span>łowniczek (terminy w tej księdze)

- **Obrona**: próg trafienia/obejścia przeciwnika w walce. Gracz rzuca i porównuje wynik do Obrony.
- **Trudność (T)**: próg testu przeciw środowisku, zjawisku, ruchowi specjalnemu albo „sztuczce” wroga.
- **<span class="rpg-token token-heart">Serca</span>**: ile obrażeń wytrzymuje istota w tej scenie.
- **Pachołek / Elita / Boss**: trzy poziomy „ważności” przeciwnika w scenie.
- **<span class="rpg-token token-stat">U</span>łatwienie / Utrudnienie**: zmiana rozmiaru kości gracza o 1 stopień (**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>** / w dół).
- **Ruch specjalny**: aktywna zdolność wroga, która zmienia sytuację (często wymusza test <span class="rpg-token token-stat">S</span>/<span class="rpg-token token-stat">Z</span>/<span class="rpg-token token-stat">M</span> gracza).
- **Cecha (pasywna)**: stała właściwość wroga (pancerz, lot, odporność, strefa zagrożenia), która zwykle daje ułatwienie/utrudnienie albo zmienia stawkę.

---



---

### 1. Jak działa przeciwnik w NDE (w skrócie)

W NDE przeciwnik jest prosty, ale „żywy” dzięki zachowaniu.

1) **Gracz działa → gracz rzuca.**  
   - Atak wręcz: Siła (<span class="rpg-token token-stat">S</span>) vs **Obrona** celu.  
   - Atak dystansowy: Zręczność (<span class="rpg-token token-stat">Z</span>) vs **Obrona** celu.  
   - Moce: Moc (<span class="rpg-token token-stat">M</span>) vs **Trudność (T)** lub vs Obrona (jeśli to atak/obezwładnienie).

2) **Jeśli gracz pudłuje / przegrywa test**, scena idzie dalej: pojawia się koszt lub komplikacja.  
   W walce koszt może oznaczać:
   - utratę pozycji,
   - utratę czasu,
   - wejście w zasięg niebezpiecznej strefy,
   - albo **utracone Serce**, jeżeli to ma sens (np. walka w zwarciu, ostrzał krzyżowy, pole rażenia).

3) **Przeciwnik „działa” bez rzutu:**  
   MG opisuje, co robi wróg, a jeśli to realnie zagraża bohaterom, to:
   - wymusza test (<span class="rpg-token token-stat">S</span>/<span class="rpg-token token-stat">Z</span>/<span class="rpg-token token-stat">M</span>) przeciw **Trudności (T)**,
   - albo stawia warunek („dopóki nie…”, „kiedy wejdziesz w…”, „kto stoi Blisko…”),
   - albo zmienia kości graczy (ułatwienie/utrudnienie).

4) **Walka jest zrozumiała, gdy wróg ma jednozdaniową taktykę.**  
   Każdy statblock powinien zawierać: „co ten wróg robi w pierwszej rundzie” i „co robi, gdy dostanie po twarzy”.

---



---

### 2. Statblock — format i pola

Minimalny statblock ma tylko to, co jest potrzebne w scenie.

> **Nazwa — Klasa, Obrona, <span class="rpg-token token-heart">Serca</span>, Rola, Mobilność, Zdolności, Ruchy, Taktyka**

### 2.1 Pola obowiązkowe

- **Klasa:** Pachołek | Elita | Boss  
- **Obrona:** liczba, którą trzeba przebić, żeby trafić/obejść wroga.  
- **<span class="rpg-token token-heart">Serca</span>:** ile trafień wytrzymuje (w NDE „trafienie” standardowo = 1 Serce).  
- **Rola:** jaką presję tworzy w walce (patrz rozdział 4).  
- **Mobilność:** jak się porusza (opisowo strefami; siatka jest opcją).  
- **Zdolności (pasywne):** 1–2 krótkie cechy.  
- **Ruchy (aktywne):** 1 ruch (Elita) albo 2–3 ruchy (Boss).  
- **Taktyka:** 1–3 zdania, żeby MG prowadził wroga konsekwentnie.

### 2.2 Pola opcjonalne (warto mieć, jeśli pasują)

- **Zasięg:** jeśli wróg jest dystansowy (np. „Daleko”, „Bardzo daleko”).  
- **Strefa:** jeśli wróg tworzy obszar niebezpieczny (dym, ogień, pole siłowe).  
- **<span class="rpg-token token-stat">S</span>łabość:** jasna „dźwignia” dla graczy (woda, światło UV, zakłócanie sygnału).  
- **Nagroda / Ślad:** co zostaje po pokonaniu (łup, trop, informacja).  
- **Warianty:** 1–2 szybkie podmiany (np. „zamiast lotu ma skok”; „zamiast ognia ma kwas”).

### 2.3 Przykład statblocka (uniwersalny)

**Strażnik — Pachołek, Obrona 5, <span class="rpg-token token-heart">Serca</span> 1, Brute, Mobilność: Niedaleko→Blisko, Zdolności: Tarcza, Ruchy: Napór, Taktyka: blokuje przejście i wypycha z osłon.**

- **Tarcza (pasywne):** dopóki stoi **Blisko** osłony lub tarczownika, atakujący ma **utrudnienie** (kość w dół o 1 stopień).  
- **Napór (ruch):** jeśli Strażnik trafi w zwarciu (albo jeśli gracz spudłuje atak wręcz przeciw niemu), MG może wypchnąć bohatera o 1 strefę (Blisko→Niedaleko) lub o 1–2 kratki w wariancie siatki.  
- **Taktyka:** wchodzi w zwarcie z najsłabszym celem, broni korytarza, nie ucieka.

---



---

### 3. Klasy przeciwników: Pachołek, Elita, Boss

W NDE „trudność” przeciwnika składa się z dwóch rzeczy:
- **jak trudno go trafić** (Obrona),
- **ile wytrzyma** (<span class="rpg-token token-heart">Serca</span>),
- oraz **jaką presję robi** (rola + ruchy).

### 3.1 Pachołek (minion)

- **Obrona:** zwykle **5** (łatwiejszy: 4, trudniejszy: 6).  
- **<span class="rpg-token token-heart">Serca</span>:** **1** (odpada po trafieniu).  
- **Ruchy:** zwykle 0–1 (prosty, czytelny).  
- **Po co jest:** daje tempo, tło i poczucie „walki z grupą”.  
- **Jak prowadzić:** wchodzi w liczbie 3–8, ginie szybko, ale robi hałas i zajmuje przestrzeń.

> Dobra zasada: pachołek ma przede wszystkim *pozycję* (osłonę, przewagę liczby, wysoki teren), a nie „złożoną mechanikę”.

### 3.2 Elita

- **Obrona:** zwykle **6** (łatwiejsza elita: 5, „twarda elita”: 8).  
- **<span class="rpg-token token-heart">Serca</span>:** **2**.  
- **Ruchy:** 1 charakterystyczny ruch + 1 cecha pasywna.  
- **Po co jest:** jest „mini-bossem” w scenie, zmusza do adaptacji.

> Elita powinna robić *jedną rzecz wyraźnie*: „łamie osłony”, „rozstawia strefy”, „skacze po ścianach”, „leczy pachołków”.

### 3.3 Boss

- **Obrona:** zwykle **8** (legendarny: 12).  
- **<span class="rpg-token token-heart">Serca</span>:** **3** (finał: 5).  
- **Ruchy:** 2–3 ruchy + 1–2 cechy pasywne.  
- **Po co jest:** jest sceną samą w sobie — wpływa na teren i tempo.

**Boss bez sztuczek jest nudny.** Żeby boss był „grywalny”, daj mu przynajmniej jedno z poniższych:
- ruch, który wymusza test na wielu bohaterach,
- strefę (teren, który trzeba ogarniać),
- albo mechanikę „fazy” (po utracie 1 <span class="rpg-token token-heart">Serca</span> zmienia zachowanie).

### 3.4 „Legendarny” (opcjonalny poziom)

Jeśli potrzebujesz przeciwnika kampanijnego:
- **Obrona 12**, **<span class="rpg-token token-heart">Serca</span> 5**, 3–4 ruchy, strefy i fazy.
To jest „boss na finał aktu” — nie dawaj tego przypadkowo.

---



---

### 4. Role przeciwników (czytelna presja)

Role są po to, żeby MG od razu wiedział „jak tym grać”.  
Rola nie jest statystyką — to **styl zagrożenia**.

- **Brute (napór wręcz):** wchodzi Blisko, pcha, przewraca, łamie front.  
  *Pytanie do graczy:* „kto stoi z przodu i co ryzykuje?”

- **Skirmisher (mobilny):** wchodzi, robi swoje i ucieka; karze samotność.  
  *Pytanie:* „kto jest odłączony od drużyny?”

- **Artillery (dystans):** strzela zza osłon; wymusza ruch i zmianę pozycji.  
  *Pytanie:* „gdzie jest bezpiecznie, a gdzie jest linia ostrzału?”

- **Controller (kontrola):** strefy, dym, lepki teren, pułapki, parcie na cele.  
  *Pytanie:* „jak ominąć strefę, zamiast się w niej siłować?”

- **Support (wsparcie):** wzmacnia, leczy, przesuwa, daje osłony.  
  *Pytanie:* „kogo wyłączyć najpierw, żeby walka się uprościła?”

---



---

### 5. <span class="rpg-token token-stat">U</span>łatwienia/utrudnienia w potworach — zasada prowadzenia

W NDE **nie komplikujemy liczb**.  
Zamiast: „+2 do trafienia, -1 do obrażeń, premia do AC” — robimy:

- **ułatwienie:** podbij kość gracza o 1 stopień,
- **utrudnienie:** obniż kość gracza o 1 stopień,
- **zmiana stawki:** sukces działa, ale wymaga innego podejścia (np. najpierw zdjąć osłonę).

### 5.1 Kiedy zmieniasz Obrona, a kiedy kość

- **Najczęściej zmieniaj kość gracza** (ułatwienie/utrudnienie).  
- **Obronę zmieniaj rzadko**, głównie gdy:
  - wróg ma „pancerz / niewidzialność / pole siłowe”, które *rzeczywiście* czynią go trudniejszym do trafienia,
  - albo gdy to jest mechanika fazy bossa.

### 5.2 Przykłady „czystych” utrudnień

- „Wróg jest w częściowej osłonie” → atakujący ma **utrudnienie**.  
- „Wróg jest ogłuszony / związany” → atakujący ma **ułatwienie**.  
- „Wróg jest szybki i skacze po ścianach” → atakujący ma **utrudnienie**, dopóki go nie zablokują.

---



---

### 6. Zdolności pasywne (cechy) — katalog do sklejania

Poniżej masz cechy, które możesz dokleić do statblocka.  
Wybieraj **1–2** (boss: 2–3). Zawsze opisuj je w świecie gry.

### 6.1 Ochrona i twardość

- **Pancerz Lekki:** pierwsze trafienie w tej scenie zadaje o 1 Serce mniej (czyli 0) *albo* wymaga „doprecyzowania” (sukces zadaje Serce dopiero, gdy atak obejdzie pancerz).  
  *Najprostsza wersja:* „pierwsze trafienie nie zadaje <span class="rpg-token token-heart">Serca</span>”.

- **Pancerz Ciężki:** dopóki nie obejdziesz pancerza (flank, eksplozja, hak, magia), ataki mają **utrudnienie**.  
  *Uwaga:* dawaj graczom jasną drogę obejścia.

- **Twardy:** po utracie 1 <span class="rpg-token token-heart">Serca</span> wróg nie zmienia pozycji (nie da się go łatwo wypchnąć/obalić).  
  Dobre dla kolosów i bossów.

### 6.2 Mobilność

- **Szybki:** raz na rundę może zmienić odległość o dodatkową strefę (np. Daleko→Niedaleko).  
  W siatce: +1–2 kratki.

- **Skoczek / Wspinacz:** traktuje przeszkody pionowe jak normalne.  
  Daje sensowne „skrótowe wejścia” na tyły.

- **Latanie:** ignoruje przeszkody terenu, ale wymaga osłon „od góry” albo wymusza testy reakcji (np. <span class="rpg-token token-stat">Z</span>, by uniknąć nalotu).

### 6.3 Percepcja i skradanie

- **Zwiadowca:** pierwsza próba podejścia go z zaskoczenia ma **utrudnienie**.  
- **Czujki:** jeśli ktoś wykona głośną akcję w scenie, wróg natychmiast zmienia pozycję na lepszą (wchodzi w osłonę / wzywa wsparcie).

### 6.4 Odporności i słabości (prosto)

- **Odporność [typ]:** pierwszy raz w scenie, gdy wróg miałby dostać dany efekt (ogień, lód, psychika, prąd), efekt jest **słabszy** (mniejszy obszar / krócej / bez utraty <span class="rpg-token token-heart">Serca</span>).  
- **Wrażliwość [typ]:** przeciw temu typowi ataków gracz ma **ułatwienie**.

> Zasada przejrzystości: odporność i wrażliwość mają sens tylko, jeśli gracze mogą to odkryć i wykorzystać.

### 6.5 „Rój” i presja liczby

- **Rój:** jeśli co najmniej dwa takie stworzenia są Blisko jednego bohatera, bohater ma **utrudnienie** na testy ruchu/ucieczki, dopóki nie zmieni strefy.

---



---

### 7. Ruchy aktywne — jak pisać i jak prowadzić

Ruch aktywny powinien odpowiadać na 3 pytania:
1) **Co robi w fikcji?** (opis)
2) **Kogo dotyczy i kiedy?** (wyzwalacz)
3) **Jak rozstrzyga się mechanicznie?** (test / efekt / koszt)

### 7.1 Prosty format ruchu

- **Nazwa ruchu:** jedno zdanie opisu.
- **Wyzwalacz:** kiedy to się dzieje (np. „gdy bohater jest Blisko”, „gdy ktoś strzela z osłony”).
- **Test:** jaka cecha i jaka Trudność.
- **Skutek porażki:** co tracisz, co się zmienia.
- **Skutek sukcesu:** zwykle unikasz skutku, albo zyskujesz przewagę.

### 7.2 Jak ustalać Trudność ruchu wroga (bez tabel)

Jeśli ruch jest „atakujący” i dotyczy pojedynczego celu:
- ustaw **T ruchu = Obrona wroga** (to jest spójne i łatwe do zapamiętania).

Jeśli ruch jest obszarowy albo „duży”:
- ustaw T o 1 próg wyżej niż standard sceny (zwykle **T 6** albo **T 8**).

### 7.3 Przykładowe ruchy (moduły)

**Napór (Brute)**  
- **Opis:** wróg wchodzi w zwarcie i spycha.  
- **Wyzwalacz:** gdy wróg jest Blisko bohatera.  
- **Test:** bohater robi test **<span class="rpg-token token-stat">S</span> lub <span class="rpg-token token-stat">Z</span>** przeciw **T = Obrona wroga**.  
- **Porażka:** bohater traci 1 Serce *albo* zostaje wypchnięty o 1 strefę (MG wybiera to, co ma sens).  
- **Sukces:** unikasz obrażeń i utrzymujesz pozycję.

**Salwa (Artillery)**  
- **Opis:** seria strzałów / odłamków w obszar.  
- **Wyzwalacz:** gdy co najmniej 2 bohaterów jest w tej samej strefie i nie w osłonie.  
- **Test:** każdy cel testuje **<span class="rpg-token token-stat">Z</span>** przeciw **T 6** (albo T = Obrona wroga, jeśli wróg jest elitą).  
- **Porażka:** −1 Serce i „musisz się przemieścić” (Blisko→Niedaleko).  
- **Sukces:** chowasz się / nie dostajesz.

**Kotwica (Controller)**  
- **Opis:** lepki teren, pole siłowe, pajęczyna, lód.  
- **Wyzwalacz:** wróg ma chwilę, by ustawić strefę.  
- **Test:** gdy wejdziesz w strefę, test **<span class="rpg-token token-stat">Z</span> lub <span class="rpg-token token-stat">M</span>** przeciw **T 5–6**.  
- **Porażka:** tracisz przemieszczenie w tej turze i jesteś „w złej pozycji” (utrudnienie na ataki).  
- **Sukces:** przechodzisz lub neutralizujesz strefę.

**Wzmocnienie (Support)**  
- **Opis:** wróg osłania sojusznika / leczy / daje przewagę.  
- **Wyzwalacz:** raz na rundę, gdy sojusznik jest zagrożony.  
- **Efekt:** wybrany sojusznik dostaje „tarcze” — atakujący mają **utrudnienie** do końca rundy, albo sojusznik odzyskuje 1 Serce (boss/elite).  
- **Kontra graczy:** wyłącz supporta albo zmuszaj go do wyboru (kogo ratuje).

---



---

### 8.1 Domyślnie: strefy odległości

W opisowej walce używaj: **Blisko / Niedaleko / Daleko / Bardzo daleko**.

W statblocku zapisuj mobilność jako:
- „**Mobilność:** zmienia strefę o 1 (standard)”
- albo „**Mobilność:** Szybki (zmienia strefę o 2)”
- albo „**Mobilność:** Lata (ignoruje przeszkody, ale wymusza testy przy nalotach)”.

### 8.2 Opcja: siatka (jeśli <span class="rpg-token token-math">st</span>ół lubi taktykę)

Jeśli gracie na mapie:
- standardowy ruch = **5 kratek**,
- Szybki = **6–7**,
- Skok = 3 kratki „w pionie” albo przez przeszkody.

**Wszystkie zdolności opisowe działają tak samo** — siatka tylko „daje metrówkę”.

---



---

### 9. Budowa przeciwnika w 2 minuty (procedura)

1) **Wybierz klasę**: Pachołek / Elita / Boss.  
2) **Ustaw Obrona**: 5 / 6 / 8 (legendarny: 12).  
3) **Ustaw <span class="rpg-token token-heart">Serca</span>**: 1 / 2 / 3 (finał: 5).  
4) **Wybierz rolę**: Brute / Skirmisher / Artillery / Controller / Support.  
5) **Dodaj 1–2 cechy pasywne** (boss: 2–3).  
6) **Dodaj ruchy**: Elita 1, Boss 2–3.  
7) **Napisz taktykę w 2 zdaniach** (pierwsza runda + reakcja na zagrożenie).  
8) (Opcjonalnie) Dodaj **słabość** i **nagrodę**.

> Test praktyczny: jeśli możesz poprowadzić wroga bez patrzenia w tabelę — statblock jest dobry.

---



---

### 10. Gotowe szablony (do reskinu na każdy świat)

Poniższe wpisy są celowo „bez koloru”. Zmieniasz nazwę i opis — mechanika zostaje.

### 10.1 Pachołki

- **Strażnik — Pachołek, Obrona 5, <span class="rpg-token token-heart">Serca</span> 1, Brute, Mobilność: standard, Zdolności: Tarcza, Ruchy: Napór, Taktyka: blokuje i wypycha.**
- **Zwiadowca — Pachołek, Obrona 5, <span class="rpg-token token-heart">Serca</span> 1, Skirmisher, Mobilność: Szybki, Zdolności: Zwiadowca, Ruchy: Ucieczka, Taktyka: podchodzi, oznacza cele i znika.**
- **Strzelec — Pachołek, Obrona 5, <span class="rpg-token token-heart">Serca</span> 1, Artillery, Mobilność: standard, Zdolności: Osłona, Ruchy: Ostrzał, Taktyka: trzyma Daleko i zmusza do biegu.**
- **Kontroler — Pachołek, Obrona 5, <span class="rpg-token token-heart">Serca</span> 1, Controller, Mobilność: standard, Zdolności: Strefa, Ruchy: Kotwica, Taktyka: dzieli drużynę.**
- **Wsparcie — Pachołek, Obrona 5, <span class="rpg-token token-heart">Serca</span> 1, Support, Mobilność: standard, Zdolności: Medyk, Ruchy: Wzmocnienie, Taktyka: chroni elitę.**

**Szybkie ruchy do pachołków:**
- **Ucieczka:** gdy zostanie trafiony (ale jeszcze „nie odpada” w fikcji, np. pancerz), oddala się o 1 strefę.
- **Ostrzał:** jeśli ktoś stoi w otwartym, daje mu utrudnienie na kolejne działanie („kulki, odłamki, strach”).
- **Strefa:** raz na scenę stawia małą strefę utrudnienia (dym, olej, błoto).

### 10.2 Elity

- **Twardziel — Elita, Obrona 6, <span class="rpg-token token-heart">Serca</span> 2, Brute, Mobilność: standard, Zdolności: Pancerz Lekki, Ruchy: Napór, Taktyka: wchodzi Blisko i trzyma linię.**
- **Skrytobójca — Elita, Obrona 6, <span class="rpg-token token-heart">Serca</span> 2, Skirmisher, Mobilność: Szybki + Skoczek, Zdolności: Zwiadowca, Ruchy: Cięcie z flanki, Taktyka: uderza w tył i wycofuje się.**
- **Snajper — Elita, Obrona 6, <span class="rpg-token token-heart">Serca</span> 2, Artillery, Mobilność: Daleko, Zdolności: Osłona, Ruchy: Strzał wyborowy, Taktyka: wymusza ruch i karze brak osłony.**
- **Manipulator Terenu — Elita, Obrona 6, <span class="rpg-token token-heart">Serca</span> 2, Controller, Mobilność: standard, Zdolności: Strefa (2×), Ruchy: Kotwica, Taktyka: odcina drogę ucieczki.**
- **Dowódca — Elita, Obrona 6, <span class="rpg-token token-heart">Serca</span> 2, Support, Mobilność: standard, Zdolności: Czujki, Ruchy: Wzmocnienie, Taktyka: wzmacnia sojuszników i ustawia ich w osłonach.**

### 10.3 Bossowie

- **Przywódca — Boss, Obrona 8, <span class="rpg-token token-heart">Serca</span> 3, Support, Mobilność: standard, Zdolności: Czujki + Tarcza, Ruchy: Wzmocnienie + Przyzwanie + Bariera, Taktyka: trzyma wsparcie i kontroluje tempo.**
- **Kolos — Boss, Obrona 8, <span class="rpg-token token-heart">Serca</span> 3, Brute, Mobilność: standard, Zdolności: Twardy + Pancerz Ciężki, Ruchy: Wstrząs + Napór, Taktyka: rozbija ustawienie i wymusza testy.**
- **Łowca — Boss, Obrona 8, <span class="rpg-token token-heart">Serca</span> 3, Skirmisher, Mobilność: Szybki + Skoczek, Zdolności: Zwiadowca, Ruchy: Zasadzka + Cięcie + Ucieczka, Taktyka: izoluje i eliminuje.**
- **Architekt Stref — Boss, Obrona 8, <span class="rpg-token token-heart">Serca</span> 3, Controller, Mobilność: standard, Zdolności: Strefa (2×) + Odporność [typ], Ruchy: Kotwica + Salwa + Przesunięcie, Taktyka: dzieli drużynę i zmusza do decyzji.**

---



---

### 11. Zagrożenia środowiskowe (Hazardy)

Hazard to „przeciwnik bez woli” albo mechanizm sceny: wieżyczka, ogień, lawina, alarm.

**Format: Nazwa — Trudność (T), Kiedy działa, Skutek, Jak wyłączyć / ominąć**

### 11.1 Przykłady hazardów (uniwersalne)

**Wieżyczka / Dron obronny — T 6**  
- **Kiedy działa:** na koniec rundy, jeśli ktoś jest w linii.  
- **Skutek:** test **<span class="rpg-token token-stat">Z</span> vs T 6**; porażka: −1 Serce i musisz wejść w osłonę.  
- **Wyłączenie:** test **<span class="rpg-token token-stat">M</span> lub <span class="rpg-token token-stat">Z</span> vs T 6** przy panelu / zakłócanie / odcięcie zasilania.

**Zatrzask / Mina / Sidełko — T 5**  
- **Kiedy działa:** gdy wejdziesz w strefę.  
- **Skutek:** test **<span class="rpg-token token-stat">Z</span> vs T 5**; porażka: −1 Serce albo unieruchomienie (tracisz przemieszczenie).  
- **Wyłączenie:** narzędzia + test **<span class="rpg-token token-stat">Z</span> vs T 4–5**.

**Gaz / Dym / Skażenie — T 5**  
- **Kiedy działa:** na początku tury, jeśli jesteś w strefie.  
- **Skutek:** test **<span class="rpg-token token-stat">S</span> lub <span class="rpg-token token-stat">M</span> vs T 5**; porażka: −1 Serce albo utrudnienie na testy do wyjścia.  
- **Wyłączenie:** przewietrzenie, maski, uszczelnienie.

**Alarm / Licznik czasu — T (zależnie od sceny)**  
- **Kiedy działa:** gdy padnie komplikacja albo ktoś zrobi hałas.  
- **Skutek:** pojawia się presja czasu (kolejna fala, zamknięcie drzwi, posiłki).  
- **Wyłączenie:** test **<span class="rpg-token token-stat">M</span>** (hack/rytuał) lub „fizycznie” test **<span class="rpg-token token-stat">S</span>/<span class="rpg-token token-stat">Z</span>**.

---



---

### 12. Generator sceny walki (szybki, czytelny)

Wybierz po 1 z każdej linii (albo rzuć <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">k6</span></span>):

1) **Cel sceny:** przejście / odzyskanie / wyłączenie / eskortowanie / kradzież / obrona  
2) **Teren:** otwarty / wąskie gardła / wielopoziom / dużo osłon / krawędzie / mgła-dym  
3) **Przeciwnicy:** 6× pachołek / 4× pachołek + elita / 2× elita / boss / boss + 2× pachołek / elita + hazard  
4) **Przewaga wroga:** osłona / wysokość / mobilność / licznik czasu / zasadzka / wsparcie z dystansu  
5) **Przewaga graczy:** zaskoczenie / narzędzia / skrót / sojusznik neutralny / teren daje osłonę / informacja (wiedzą, co to za wróg)

---



---

### 13. Balans w praktyce (bez matematyki)

W NDE balans robi się *tempem* i *presją*, a nie „CR”.

### 13.1 Szybkie reguły do ustawiania trudności sceny

- **Łatwa scena:** 4–6 pachołków albo 1 elita.  
- **Standardowa scena:** 4 pachołki + 1 elita, albo 2 elity.  
- **Trudna scena:** boss + 2–4 pachołki, albo boss + hazard.  
- **Finał:** boss (<span class="rpg-token token-heart">Serca</span> 5) + elita + presja czasu.

### 13.2 Jeśli walka trwa za krótko

- Daj **falę pachołków** (2–3 na rundę przez 2 rundy).  
- Zwiększ presję terenu: strefa dymu, alarm, brak osłon.  
- Zmień taktykę: wróg przestaje walczyć „uczciwie” (wycofuje się, bierze zakładnika, blokuje wyjście).

### 13.3 Jeśli walka się dłuży

- Daj graczom „dźwignię”: odsłonięty zbiornik, panel, rytuał, słabość.  
- Pozwól na **korzyści za sukces wyjątkowy**: wybicie osłony, rozbrojenie, rozproszenie wsparcia.  
- Zredukuj <span class="rpg-token token-heart">Serca</span> bossa z 5 do 3, jeśli to nie jest finał.

---



---

### 14. Reskin: jak przerobić jednego wroga na każdy setting

Masz statblock „Zwiadowca”. Teraz zmieniasz tylko opis:

- **Fantasy:** gobliński łucznik zwiadowca (Zwiadowca + Ostrzał).  
- **Sci-fi:** dron rozpoznawczy (Zwiadowca + Czujki).  
- **Cyberpunk:** gangowy skaut na deskorolce (Szybki + Ucieczka).  
- **<span class="rpg-token token-stat">S</span>łowiańskie:** bies, który śledzi po śladach (Wrażliwość: żelazo; Odporność: strach).

Mechanika zostaje ta sama. To pozwala społeczności dokładać setki wpisów bez rozbijania spójności rdzenia.

---

