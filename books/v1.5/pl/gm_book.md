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
generated_at: "2026-01-16T08:33:24.423Z"
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
# Księga Mistrza Gry



---



---

### 0) Zasady prowadzenia w 30 sekund

- **Zaczynaj od fikcji.** Najpierw opis sytuacji i działania graczy, dopiero potem test.
- **Ustal stawkę przed rzutem.** Powiedz: *co jest na szali* i *co się stanie przy porażce*.
- **Jedna decyzja → jeden rzut → sensowny efekt.** Nie rozbijaj jednej intencji na 3 testy.
- **Porażka pcha grę do przodu.** Nie „resetuj” sceny – zmień ją komplikacją, kosztem lub presją.
- **Trzymaj spójność.** Te same warunki → podobna Trudność, podobne konsekwencje.
- **Siatka jest opcją.** Domyślnie gra działa bez mapy: „Blisko / Niedaleko / Daleko / Bardzo daleko”.

---



---

### 1.1. Kiedy w ogóle rzucać?

Rzut ma sens tylko wtedy, gdy jednocześnie:
- wynik **nie jest oczywisty**,
- istnieje **realna stawka** (coś się zmieni),
- obie strony akceptują, że **mechanika ma prawo zdecydować**.

**Nie rzucaj**, gdy:
- działanie jest rutynowe i bez presji,
- porażka nie wniesie nic ciekawego,
- sukces jest pewny, a cena już zapłacona (np. gracze mają czas, narzędzia i bezpieczeństwo).

**Przykład (bez rzutu):** Specjalista ma dostęp administracyjny i spokojne warunki – otwarcie standardowych drzwi w bazie nie wymaga testu.  
**Przykład (z rzutem):** Te same drzwi, ale alarm jest aktywny, a patrol zbliża się za 30 sekund – to jest test, bo stawką jest czas i ujawnienie.

---

### 1.2. Checklista rozstrzygnięcia (procedura stołowa)

1) Gracz mówi: **co robi** i **co chce osiągnąć**.  
2) Ty odpowiadasz: **co stoi na przeszkodzie** i **jaka jest stawka**.  
3) Wybieracie cechę: **Siła (<span class="rpg-token token-stat">S</span>)** / **Zręczność (<span class="rpg-token token-stat">Z</span>)** / **Moc (<span class="rpg-token token-stat">M</span>)**.  
4) Ustalasz **Trudność (T)** albo **Obronę** (w walce).  
5) Określasz modyfikator sytuacji: **podbicie/obniżenie kości** oraz ewentualną **pomoc**.  
6) Rzut → wynik → konsekwencja → aktualizacja sceny.

Skrót: **Opis → Stawka → Cecha → T/Obrona → Rzut → Konsekwencja**.

---

### 1.3. Trudność (T): skala i praktyczne reguły

<span class="rpg-token token-stat">U</span>żywaj jednej skali w całej grze. To buduje zaufanie graczy do decyzji MG.

- **T 3 – łatwe:** sprzyjające warunki, brak presji, minimalny opór.  
- **T 4 – standard:** „normalna robota” w przygodzie.  
- **T 5 – trudne:** presja czasu, ryzyko, przeciwnik, wąskie okno.  
- **T 6 – bardzo trudne:** wyraźna przewaga wroga, wysokie ryzyko, złożone działanie w stresie.  
- **T 8 – heroiczne:** ponadprzeciętny wyczyn; zwykle wymaga przewagi, planu lub zasobu.  
- **T 12 – legendarne:** moment „wow”; rzadko bez przygotowania i często z dużą ceną.

**Zasada praktyczna:** jeśli nie wiesz, co ustawić – zacznij od **T 4** i dopiero potem uzasadnij „w górę” lub „w dół”.

---

### 1.4. Modyfikatory bez liczenia: podbij/obniż kość

Zamiast dodawać bonusy i kary, w NDE zmieniasz **rozmiar kości** na jeden test.

- **Lepsza sytuacja:** podbij kość o 1 stopień  
  <span class="rpg-token token-<span class="rpg-token token-d4">d4</span>"><span class="rpg-token token-d4">k4</span></span>→<span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">k6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">d8</span>"><span class="rpg-token token-d8">k8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">d12</span>"><span class="rpg-token token-d12">k12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d20">d20</span>"><span class="rpg-token token-d20">k20</span></span>
- **Gorsza sytuacja:** obniż kość o 1 stopień (w drugą stronę).

**Pomoc sojusznika:** kosztuje jego akcję i daje **podbicie kości o 1 stopień** na dany test.

**Przykład:** Zamek w ciszy (T 4) vs zamek w deszczu i pod ostrzałem (T 5 + obniżenie kości, bo drżą ręce i brak widoczności).  
To zwykle działa lepiej niż „T 6 i +2 i -1”.

---

### 1.5. Wyniki testów: sukces, porażka i tempo gry

- **1 na kości:** porażka + komplikacja (komplikacja wchodzi na pewno).  
- **Wynik < T:** porażka (ale sytuacja się zmienia).  
- **Wynik ≥ T:** sukces.  
- **Maksymalny wynik na kości:** sukces wyjątkowy (dodatkowa korzyść).

#### Jak projektować porażkę, żeby nie blokowała gry?

Zanim gracz rzuci, ustal 1–2 rodzaje kosztu:
- **czas** (ktoś zdąży, coś się zamknie),
- **pozycja** (gorzej ustawieni, odsłonięci),
- **zasób** (sprzęt, amunicja, energia, Punkt Mocy),
- **uwaga** (alarm, podejrzenia, trop).

**Przykład (fail-forward):**  
Gracz chce sforsować drzwi. Porażka nie oznacza „nie otwierasz”.  
Porażka oznacza: „otwierasz, ale robisz hałas – patrol ma teraz Blisko, a poziom alarmu rośnie”.

---



---

### 2) Łut Szczęścia (Ł<span class="rpg-token token-stat">S</span>): jak wspierać dramaturgię bez psucia gry

Każdy bohater ma na start sesji **2 Ł<span class="rpg-token token-stat">S</span>**. To jest narzędzie graczy, ale MG odpowiada za jego „ekonomię” na stole.

### 2.1. Na co gracze wydają Ł<span class="rpg-token token-stat">S</span>?

Wydaj 1 Ł<span class="rpg-token token-stat">S</span>, aby:
- wykonać **przerzut** (zostawiają lepszy),
- **podbić kość o 1 stopień** na jeden rzut,
- zamienić porażkę na **sukces z kosztem** (MG dokłada cenę).

### 2.2. Kiedy przyznać dodatkowy Ł<span class="rpg-token token-stat">S</span>?

MG może przyznać **+1 Ł<span class="rpg-token token-stat">S</span>** za:
- świadome podjęcie ryzyka, które napędza scenę,
- wejście w konsekwencje bez „targowania się”,
- kreatywne rozwiązanie zgodne z konwencją,
- bardzo dobre granie relacją, motywacją lub stawką.

**Zasada higieny:** przyznawaj oszczędnie (1–2 na sesję na osobę w skrajnie hojnej grze). Ł<span class="rpg-token token-stat">S</span> ma być „iskrą”, nie stałym paliwem.

---



---

### 3) Konflikt i walka

NDE ma walczyć szybko. Jeżeli walka trwa 60 minut, to prawie zawsze oznacza: za dużo wrogów „na <span class="rpg-token token-heart">HP</span>” albo za dużo drobnych rzutów.

### 3.1. Domyślnie bez mapy: dystanse sceniczne

<span class="rpg-token token-stat">U</span>żywaj czterech dystansów:
- **Blisko** – na wyciągnięcie ręki (zwarcie),
- **Niedaleko** – kilka kroków,
- **Daleko** – druga strona sceny,
- **Bardzo daleko** – snajpersko/pojazdowo.

W turze postać ma: **Przemieszczenie + 1 Akcję**.  
Przemieszczenie zwykle zmienia dystans o **1 stopień** (Niedaleko→Blisko).

**Przykład:** Wojownik jest Niedaleko. W turze: podbiega (Blisko) i atakuje.

### 3.2. Opcja: siatka (grid) – gdy potrzebujesz precyzji

Jeżeli gracie na siatce:
- ruch w turze: **do 5 kratek**,
- skosy dozwolone,
- teren utrudniony może kosztować „2 kratki za 1 wejście” (opcjonalnie).

Wszystkie inne zasady pozostają identyczne.

---

### 3.3. Obrona przeciwników i obrażenia

W walce zamiast Trudności używasz **Obrony** (taki „T dla walki”).

**Obrona (orientacyjnie):**
- **<span class="rpg-token token-stat">S</span>łaby** 4
- **Typowy** 5
- **Elita** 6
- **Boss** 8 (legendarny boss 12)

**Atak:** rzut **Siły** (wręcz) albo **Zręczności** (dystans) przeciw Obronie.

**Obrażenia (tempo):**
- trafienie zadaje **1 Serce**,
- sukces wyjątkowy zadaje **2 <span class="rpg-token token-heart">Serca</span>** albo daje silny efekt (rozbrojenie, przewrócenie, wybicie z rytmu, rozproszenie).

**Pachołki i elity (polecany model):**
- **Pachołek:** 1 trafienie = znika z walki (pokonany, ucieka, obezwładniony).  
- **Elita:** ma **2 <span class="rpg-token token-heart">Serca</span>** (albo „2 trafienia”), często ma jedną przewagę taktyczną.  
- **Boss:** ma **3 <span class="rpg-token token-heart">Serca</span>** + 1–2 „ruchy bossa” (patrz 3.6).

To daje szybkie starcia bez liczenia punktów.

---

### 3.4. Osłona, przewaga i „czytelny teren”

Zamiast mnożyć reguły, używaj jednego języka: **kość w górę / kość w dół**.

- Lekka osłona, dym, kiepski kąt: **obniż kość atakującego** o 1 stopień.  
- Dobra pozycja, zaskoczenie, przewaga wysokości: **podbij kość** o 1 stopień.  
- Pełna osłona: atak jest niemożliwy, dopóki sytuacja się nie zmieni.

**Przykład:** Snajper w oknie jest „Daleko” i ma przewagę wysokości → atakujący dostaje obniżenie kości.  
Drużyna zmienia scenę: granat dymny, flankowanie, obejście – i przewaga znika.

---

### 3.5. Kolejność w walce bez liczenia inicjatywy

Polecany, szybki schemat:
1) **Gracze działają** (w dowolnej kolejności przy stole).
2) **Przeciwnicy działają**.
3) Powtórz.

To pozwala graczom planować krótkie kombinacje bez obciążania stołu inicjatywą.

---

### 3.6. Jak prowadzić bossa, żeby był ciekawy (a nie „gąbką na obrażenia”)

Boss w NDE powinien mieć:
- **Obronę 8** (albo 12 w wersji „finał sezonu”),
- **3 <span class="rpg-token token-heart">Serca</span>**,
- **1–2 unikalne ruchy**, które zmieniają scenę.

**Przykładowe ruchy bossa (uniwersalne):**
- **Odepchnięcie:** ktoś trafiony cofa się o 1 dystans (Blisko→Niedaleko) i traci pozycję.
- **Przełamanie osłony:** boss niszczy osłonę lub zmusza do wyjścia z ukrycia.
- **Wezwanie wsparcia:** dołączają 2 pachołki lub jedna elita (najlepiej raz na walkę).
- **Strefa zagrożenia:** obszar staje się niebezpieczny (ogień, prąd, runy) – kto w nim zostaje, ryzykuje test.

**Zasada:** ruch bossa ma zmieniać pole gry, a nie tylko „zadawać więcej”.

---

### 3.7. Morale i zachowanie wrogów (lekka procedura)

Gdy:
- padnie pierwszy pachołek, albo
- elita straci pierwsze Serce, albo
- boss straci drugie Serce,

rzuć <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">k6</span></span> i zdecyduj:
- **1–2:** wycofują się / szukają osłony / negocjują,
- **3–4:** trzymają pozycję,
- **5–6:** nacierają agresywnie.

Modyfikuj o **+1** jeśli mają przewagę, **-1** jeśli są przerażeni lub odcięci.

---



---

### 4) Moce (<span class="rpg-token token-stat">M</span>) po stronie MG: jak je wyceniać i jak nie psuć tempa

W NDE „Moc” obejmuje magię, psionikę, cybernetykę, hackowanie, charyzmę „na poziomie filmu” – zależnie od świata.

### 4.1. Skala mocy: Trudność i koszt Punktów Mocy

- **Sztuczka:** T 4, koszt 0–1 <span class="rpg-token token-power">PM</span> (mały, krótki efekt).  
- **Standard:** T 5, koszt 1 <span class="rpg-token token-power">PM</span> (pojedynczy cel, krótki skok, tarcza).  
- **Silna:** T 6, koszt 2 <span class="rpg-token token-power">PM</span> (obszar, kontrola, leczenie).  
- **Wielka:** T 8–12, koszt 3 <span class="rpg-token token-power">PM</span> (efekt zmieniający scenę).

**Wskazówka:** jeżeli efekt ma „zmienić zasady sceny” (most z lodu, blackout w dzielnicy) – to jest Wielka moc.

### 4.2. Konsekwencje porażki mocy

Porażka powinna być konkretna i natychmiastowa:
- utrata <span class="rpg-token token-power">PM</span> (zawsze),
- przeciążenie (spadek pozycji, odsłonięcie),
- ślad (cyfrowy/astralny),
- efekt uboczny w środowisku (hałas, błysk, zapach, echo).

**Przykład:** Hack „na żywo” w walce. Porażka: <span class="rpg-token token-power">PM</span> przepada, a system loguje intruza – wchodzi licznik „kontr-ICE”.

### 4.3. Obrona przed mocą

Jeśli fikcja to uzasadnia, pozwól na „kontr-test”:
- **Zręczność** (unik, refleks) albo
- **Moc** (odporność, kontr-rytuał, zapora).

Kontr-test nie powinien mnożyć rzutów. Stosuj go tam, gdzie to robi scenę ciekawszą (np. paraliż, kontrola umysłu).

---



---

### 5.1. Buduj sceny w 5 krokach

1) **Cel sceny:** co drużyna ma osiągnąć (konkret).  
2) **Przeszkody:** 2–3 różne typy (ludzie, urządzenia, środowisko).  
3) **Zagrożenie:** przeciwnicy, hazardy, pułapki, presja czasu.  
4) **Licznik (opcjonalnie):** 3–5 pól; porażki przesuwają licznik; na końcu wchodzi duży skutek.  
5) **Nagroda i konsekwencje:** co zmienia sukces, co zmienia porażka.

To jest minimalny „silnik sceny” – działa w fantasy, sci‑fi i kryminale.

---

### 5.2. Liczniki (clocks) – prosta wersja

Licznik ma 3–5 pól. Zapełnia się, gdy:
- test kończy się porażką,
- ktoś robi hałas,
- wrogowie mają czas na reakcję.

Gdy licznik się zapełni, wchodzi skutek:
- alarm,
- posiłki,
- zamknięcie drogi,
- utrata zasobu,
- eskalacja konfliktu.

**Przykład:** „Alarm 0/4”. Porażka w skradaniu = +1. Sukces wyjątkowy = -1 (opcjonalnie).  
Gdy dojdzie do 4/4 – pojawia się patrol i drzwi się ryglują.

---

### 5.3. Jak dobrać „trudność sceny”, nie licząc wszystkiego

Dla drużyny 3–5 bohaterów:

- **Łatwo:** 3–5 pachołków lub jedna elita bez przewag terenu.  
- **Standard:** 6–8 pachołków albo elita + 2–4 pachołki, albo hazard środowiskowy.  
- **Trudno:** boss + 2–4 pachołki, albo 2 elity + 3–5 pachołków, albo licznik 3.  
- **Heroicznie:** boss + wsparcie + presja terenu + licznik 3–5.

**Najważniejsze:** teren i osłony często znaczą więcej niż liczba wrogów.

---



---

### 6.1. Skradanie i infiltracja: „Alarm”

1) Ustal licznik **Alarm 0/3 do 0/5**.  
2) Każda porażka = +1 alarm.  
3) Gracze mogą zmniejszać alarm działaniami (np. fałszywy sygnał, sabotaż) – to są normalne testy.  
4) Na maksimum wchodzi skutek: patrol, ryglowanie, lockdown.

**Przykład:** Drużyna idzie korytarzem. Specjalista chce obejść kamery (<span class="rpg-token token-stat">M</span>, T 5). Porażka = +1 alarm.  
Zanim rzuci, wie, co ryzykuje – i to jest klucz.

---

### 6.2. Pościg: „Dystans pościgu”

Ustal **Dystans** w krokach, np. **3** (średnio).  
Każda „tura pościgu”:
- uciekający robi test (<span class="rpg-token token-stat">Z</span> lub <span class="rpg-token token-stat">M</span> zależnie od sposobu),
- ścigający robi test,
- sukces uciekającego zwiększa dystans, sukces ścigającego zmniejsza,
- gdy dystans spadnie do **0** – dogonienie,
- gdy wzrośnie do **5** – ucieczka.

Dodawaj przeszkody (skręt, tłum, barykada) jako opis + modyfikator kości.

---

### 6.3. Śledztwo: „Wskazówki zamiast ściany testów”

Zasada: **wskazówka kluczowa nie może utknąć na jednym teście**.  
Jeżeli scena śledcza ma iść dalej, wskazówka kluczowa jest dostępna:
- automatycznie (jeśli gracze zrobili sensowną rzecz),
- albo po teście, ale porażka daje ją „z kosztem” (czas, fałszywy trop, alarm).

**Przykład:** Badanie ciała. Sukces: dostają prawdę. Porażka: dostają prawdę, ale przyjeżdża straż lub ktoś ich zauważa.

---

### 6.4. Konflikt społeczny: stawka, presja, konsekwencja

Nie rób z rozmowy „walki na rzutach”. Ustal:
- czego chce NPC,
- czego chcą gracze,
- co jest stawką,
- ile jest „ruchów” do przesilenia (licznik 3–5).

Testy **<span class="rpg-token token-stat">M</span>** (wpływ, blef, autorytet) lub **<span class="rpg-token token-stat">Z</span>** (czytanie intencji) zmieniają pozycję rozmowy.  
Porażka daje koszt (złe wrażenie, utrata zasobu, czas, wrogość).

---



---

### 7.1. Komplikacje przy porażce (rzuć <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">k6</span></span>)

1. Strata czasu / ktoś zdążył zareagować.  
2. Ujawnienie pozycji / wzrost alarmu.  
3. Drobna szkoda: -1 Serce lub utrata zasobu.  
4. <span class="rpg-token token-stat">Z</span>ła pozycja: wypchnięcie, upadek, odsłonięcie.  
5. Utrata lub uszkodzenie sprzętu.  
6. Pojawia się nowe zagrożenie w scenie.

---

### 7.2. Korzyści przy sukcesie wyjątkowym (rzuć <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">k6</span></span>)

1. Szybciej (oszczędzasz czas lub ruch).  
2. Ciszej (brak wzrostu alarmu).  
3. Bez kosztu (np. bez wydania <span class="rpg-token token-power">PM</span> / bez konsekwencji terenu).  
4. Większy efekt (większy zasięg, dodatkowy cel).  
5. Lepsza pozycja sojusznika (ktoś dostaje podbicie kości w następnej akcji).  
6. Dodatkowa wskazówka lub przewaga fabularna.

---

### 7.3. Szybki wpis przeciwnika (format do notatek)

> **Nazwa — Obrona, <span class="rpg-token token-heart">Serca</span>, Taktyka, Sztuczka/Przewaga**

- **Pachołek:** Obrona 4–5, 1 trafienie = znika.  
- **Elita:** Obrona 6, 2 <span class="rpg-token token-heart">Serca</span>, jedna przewaga (mobilność/kontra/osłona).  
- **Boss:** Obrona 8 (lub 12), 3 <span class="rpg-token token-heart">Serca</span>, 1–2 ruchy bossa.

**Przykład (uniwersalny):**  
> **Ochroniarz — Obrona 5, 1 trafienie, trzyma korytarz, granat dymny (raz)**

---



---

### 8) Bezpieczeństwo i umowa stołu (minimum)

- Ustalcie, czego nie gracie (tematy tabu) i co „przewijacie”.  
- Uzgodnijcie prosty sygnał przerwania sceny (np. „stop” lub „pauza”).  
- Konflikty przy stole rozwiązuj rozmową poza fikcją, nie „rulings w złości”.

To poprawia jakość gry bardziej niż jakakolwiek mechanika.

---



---

### 9) Modułowość i rozwój przez społeczność: jak to utrzymać w ryzach

Jeśli budujesz NDE jako „engine”, to społeczność najłatwiej będzie rozwijać przez paczki:

- **Pakiet gatunkowy** (fantasy/cyberpunk/horror): mapowanie Mocy, lista atutów, sprzęt, przeciwnicy, 1–2 procedury (np. strach, pościg).  
- **Pakiet przeciwników:** 10–20 wpisów pachołek/elita/boss + taktyki.  
- **Pakiet przygód:** 1‑stronicowe sceny z licznikami i stawkami.

**Wymóg jakości wkładu:** każda nowa reguła powinna mieć:
- zdanie „po co to jest” (jaki problem rozwiązuje),
- krótki zapis reguły,
- przykład 3–5 linijek.

Dzięki temu dodatki nie rozsadzą rdzenia i będą czytelne dla nowych.

---

