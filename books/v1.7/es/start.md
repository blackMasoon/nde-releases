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
generated_at: "2026-01-14T12:08:17.660Z"
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
# Reglas de un vistazo

Automatic translation placeholder for es

---



---

### [ERROR] 1) Bohater w 1 minutę

[Translation Failed] * **Koncept:** kim jesteś i w jakim gatunku grasz (1 zdanie).
* **Rola (wybierz jedną):**

  * **Szturm** – presja, walka, przełamywanie przeszkód
  * **Specjalista** – skradanie, precyzja, technika, obserwacja
  * **Adept** – moce, wiedza, wpływ, improwizacja
* **Cechy (3):**

  * **Siła (S)** – siła fizyczna, wytrzymałość, walka wręcz
  * **Zręczność (Z)** – refleks, skradanie, strzelanie, pilotowanie
  * **Moc (M)** – magia/psionika/technologia/blef/intuicja (zależnie od świata)
* **Kości cech:** jedna cecha **<span class="rpg-token token-d12">k12</span>**, jedna **<span class="rpg-token token-d8">k8</span>**, jedna **<span class="rpg-token token-d6">k6</span>** (wybierz zgodnie z rolą).
* **Serca:** 5. **Punkty Mocy:** 3 (wydajesz na moce i „zagrania specjalne”).
Poniżej masz gotowy fragment do wklejenia (wariant A), w stylistyce krótkich zasad „1-page”.

**Łut Szczęścia (jak działa):** wydaj **1 ŁS**, aby wybrać jedno:

* **Przerzut** swojego testu (zostawiasz lepszy wynik), albo
* **Podbicie kości o 1 stopień** na ten jeden rzut (**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>**), albo
* **Zamiana porażki na „sukces z kosztem”** — akcja się udaje, ale MG natychmiast dokłada cenę (np. tracisz czas, robisz hałas, zużywasz zasób, kończysz w gorszej pozycji, przyciągasz uwagę, psujesz sprzęt).

**Odzysk ŁS:** na początku kolejnej sesji wracasz do limitu. MG może przyznać **+1 ŁS** za odważne ryzyko, świetną decyzję fabularną lub granie konsekwencjami.

* **Ekwipunek:** 1 narzędzie „kluczowe” (np. miecz, karabin, zestaw hakerski), 1 ochrona (pancerz, tarcza energetyczna, kamuflaż), 3 drobiazgi pasujące do konceptu.

**Przykład:** Specjalista: Z <span class="rpg-token token-d12">k12</span>, M <span class="rpg-token token-d8">k8</span>, S <span class="rpg-token token-d6">k6</span>. W cyberpunku M to „Hacking/Influence”; w fantasy M to „Magia/Wola”.



---

### [ERROR] 2) Jak rozstrzygać akcje

[Translation Failed] 1. Gracz mówi **co robi** i **jak** (opis w świecie gry).
2. Prowadzący ustala **Trudność** i stawkę („co się stanie przy porażce”).
3. Rzuć kością cechy (S/Z/M) i porównaj z Trudnością.

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

**Przykład:** Adept próbuje zamknąć portal (M <span class="rpg-token token-d8">k8</span>) przy alarmie i stresie → gorsza sytuacja, spada na <span class="rpg-token token-d6">k6</span>. T = 5. Rzut 6: sukces, ale „alarm” zostaje w tle jako presja fabularna.



---

### [ERROR] 3) Ruch i walka – domyślnie bez siatki, siatka jako opcja

[Translation Failed] **Domyślnie: theatre of mind (zalecane)**

* Odległości opisuj jako: **Blisko** (na wyciągnięcie), **Niedaleko** (kilka kroków), **Daleko** (druga strona sceny), **Bardzo daleko** (snajpersko/pojazdowo).
* W turze masz: **Przemieszczenie + 1 Akcję**.

  * Przemieszczenie zwykle zmienia odległość o 1 „stopień” (Niedaleko→Blisko itp.).
* **Atak**: rzut **S** (wręcz) albo **Z** (dystans) przeciw **Obronie** celu.

**Obrona przeciwników (orientacyjnie):**

* **Słaby** 4, **Typowy** 5, **Elita** 6, **Boss** 8 (legendarny boss 12).

**Skutki trafienia (szybka walka):**

* Trafienie zadaje **1 Serce**.
* Sukces wyjątkowy zadaje **2 Serca** albo daje silny efekt (rozbrojenie, przewrócenie, rozproszenie).

**Osłona i przewaga pozycyjna:**

* Lekka osłona / gorszy kąt: obniż kość atakującego o 1 stopień.
* Dobra pozycja / zaskoczenie: podbij kość o 1 stopień.

**Opcja: gra na siatce**

* 1 kratka = 1–2 m. Ruch w turze: **do 5 kratek**. Reszta zasad bez zmian.

**Przykład:** Specjalista strzela z osłony (Z <span class="rpg-token token-d12">k12</span>) do elity (Obrona 6). Cel jest w lekkiej osłonie → Z spada na <span class="rpg-token token-d8">k8</span>. Rzut 7: sukces, 1 Serce obrażeń.



---

### [ERROR] 4) Moce, „czary” i zagrania specjalne (uniwersalne)

[Translation Failed] To obejmuje magię, psionikę, cybernetykę, gadżety, sztuczki filmowe – zależnie od świata.

* Gdy robisz coś **ponad standard**: wydaj **Punkt Mocy** i rzuć **M**.
* Ustal poziom efektu:

**Poziomy mocy (T / koszt):**

* **Sztuczka** (krótki efekt, trik, „flash”): **T 4 / 0–1 PM**
* **Standard** (atak, tarcza, impuls, kontrola drobna): **T 5 / 1 PM**
* **Silna** (obszar, leczenie, paraliż, hack „na żywo”): **T 6 / 2 PM**
* **Wielka** (zmiana sceny, potężna ingerencja): **T 8–12 / 3 PM**

**Porażka:** PM przepada, a konsekwencja jest natychmiastowa (przeciążenie, ślad cyfrowy, rysa w rytuale, niechciana uwaga).

**Odzysk:** po scenie konfliktu odzyskujesz **1 PM**, po bezpiecznym odpoczynku – do pełna.

**Przykład:** W space-operze Adept próbuje „zagiąć sensor” drona: Standard, T 5, koszt 1 PM. Rzut M <span class="rpg-token token-d8">k8</span> = 8: sukces wyjątkowy – dron traci sygnał i myli trop.



---

### [ERROR] 5) Upadek, ryzyko i leczenie

[Translation Failed] * Gdy spadasz do **0 Serc**, jesteś **wyłączony z akcji** (raniony, ogłuszony, w szoku – według konwencji).
* Sojusznik może zużyć akcję, by postawić cię na **1 Serce** (pierwsza pomoc, adrenalina, restart systemu).
* Po scenie, jeśli macie chwilę oddechu: wracacie do **pełnych Serc**, o ile macie warunki (schronienie, opatrunek, serwis, posiłek).
* Jeżeli scena była wyjątkowo brutalna albo wrogowie mają przewagę, Prowadzący może wymagać, by „pełny reset” wymagał bezpiecznego postoju.

**Przykład:** Szturm spada do 0. Specjalista wciąga go za osłonę i zużywa akcję: Szturm wraca na 1 Serce i może działać w następnej turze.



---

### 6) Desarrollo de PERSONAJES

Después de la aventura elige una:
- Aumenta un atributo en un tamaño de dado: <span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>,
- o +1 Corazón (máx. 7),
- o +1 Maná (máx. 5).
Ejemplo: El Guerrero aumenta su Fuerza de <span class="rpg-token token-d10">d10</span> a <span class="rpg-token token-d12">d12</span> — es más fácil alcanzar <span class="rpg-token token-tn">TN</span> 12.



---

### 7) Variante solo-<span class="rpg-token token-d6">d6</span>

Cuando solo tienen un dado <span class="rpg-token token-d6">d6</span>:
- En lugar de tamaños de dados, cada atributo tiene un umbral de éxito:
  - Maestro 3+, Entrenado 4+, Novato 5+, Sin habilidad 6.
- La <span class="rpg-token token-tn">TN</span> sigue cambiando la situación en 1 grado (más fácil/más difícil).
- Ayuda: baja el umbral en 1 (por ejemplo, de 4+ a 3+ para esta tirada).
- Desarrollo: sube el nivel de un atributo (por ejemplo, Entrenado 4+ → Maestro 3+) o +1 Corazón/Mana.
Ejemplo: Tiro de Pícaro (Entrenado 4+) a un objetivo en cobertura ligera (un grado más difícil) requiere 5+. Tirada <span class="rpg-token token-d6">d6</span>=5 — impacto.

