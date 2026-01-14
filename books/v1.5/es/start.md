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
generated_at: "2026-01-14T12:06:55.716Z"
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

### 3) Movimiento y lucha en el tablero

- Movimiento: hasta 5 casillas (diagonales permitidas).
- Tu turno: Movimiento + 1 Acción (por ejemplo, ataque, hechizo, búsqueda, levantar palanca).
- Ataque:
  - Cuerpo a cuerpo (S): tirada contra la <span class="rpg-token token-tn">TN</span> del oponente.
  - A distancia (Z): la cobertura del objetivo aumenta la <span class="rpg-token token-tn">TN</span> en 1 grado.
- <span class="rpg-token token-tn">TN</span> de los oponentes: Peón 6, Élite 8, Jefe 12.
- Efectos de un impacto: Peón — cae tras ser impactado; Élite — el MJ puede requerir condiciones favorables; Jefe — tiene 3 Heridas (un impacto = 1 Herida). Éxito excepcional contra el Jefe = 2 Heridas.
- Contraataque: si fallas en cuerpo a cuerpo o en el rango de contraataque, pierdes 1 Corazón (a menos que tengas cobertura total).
Ejemplo: Mago (Z <span class="rpg-token token-d6">d6</span>) dispara con una honda a un peón detrás de una caja: <span class="rpg-token token-tn">TN</span> 6 + cobertura → 8. El Mago pide ayuda al Pícaro (aumenta el dado a <span class="rpg-token token-d8">d8</span>) y cambia de posición a una mejor (<span class="rpg-token token-tn">TN</span> baja a 6). <span class="rpg-token token-d8">d8</span>=7 — impactado.



---

### 4) Magia

- Lanzar un hechizo: describe el efecto, gasta Maná, lanza Magia (M).
  - Truco (llama, estruendo, niebla) — <span class="rpg-token token-tn">TN</span> 4, costo 0–1 Maná.
  - Proyectil/Protección/Salto 5 casillas — <span class="rpg-token token-tn">TN</span> 6, costo 1 Maná.
  - Área/Sanación +2 Corazones/Parálisis — <span class="rpg-token token-tn">TN</span> 8, costo 2 Maná.
  - Gran poder (puente de hielo, tormenta de fuego) — <span class="rpg-token token-tn">TN</span> 12, costo 3 Maná.
- Fracaso: el Maná se pierde; ocurre una pequeña consecuencia (falta de aliento -1 Corazón o atención no deseada de los enemigos).
- Descanso después de la batalla: recuperas todo el Maná; un descanso seguro también restaura Corazones.
Ejemplo: “Destello” (teleportación corta 5 casillas): <span class="rpg-token token-tn">TN</span> 6, costo 1 Maná. El mago <span class="rpg-token token-d10">d10</span> lanza 7 — salto exitoso tras la protección.



---

### 5) Caída y tratamiento

- 0 Corazón: caído (no estás funcionando). Un aliado puede gastar una acción para levantarte a 1 Corazón.
- Después del combate, con un breve descanso y una comida, regresan a la plenitud de Corazones y Maná.
Ejemplo: El pícaro cae a 0. El guerrero le ayuda a levantarse — el pícaro regresa a 1 Corazón.



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

