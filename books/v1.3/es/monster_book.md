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
generated_at: "2026-01-13T12:23:09.213Z"
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
# Manual de Monstruos

Automatic translation placeholder for es

---



---

### 1. Introducción

- Usamos los mismos conceptos que en las reglas básicas y en el libro de MG.
- **Solo los jugadores tiran.** Los oponentes ejercen presión a través de la <span class="rpg-token token-tn">TN</span> y los movimientos; los daños generalmente resultan de "represalias" o pruebas forzadas a los jugadores.



---

### 1. Introducción

> Nombre — Clase, <span class="rpg-token token-tn">TN</span>, Heridas, Rol, Movimiento, Especial

- **Clase:** Cono | Élite | Jefe
- **<span class="rpg-token token-tn">TN</span>:** número 4/6/8/12 que determina la dificultad para golpear/evitar al oponente.
- **Heridas:** solo para Élite y Jefe (Élite: 2, Jefe: 3 por defecto). El Cono no tiene Heridas (cae tras ser golpeado).
- **Rol:** Bruto (combate cuerpo a cuerpo), Escaramuzador (móvil), Artillería (distancia), Controlador (control de campo), Soporte (apoyo).
- **Movimiento:** por defecto 5 casillas. Cambia si la movilidad es única (por ejemplo, 6 Rápido, Volar, Salto 3).
- **Especial:** 1–2 habilidades descriptivas cortas (ver secciones "Características" y "Movimientos").

Ejemplo de anotación: “Guardia Élite — Élite, <span class="rpg-token token-tn">TN</span> 8, Heridas 2, Bruto, Movimiento 5, Especial: Escudo Pesado; Embestida”.



---

### Pachołek (minion):

- **Pachołek (esbirro):** <span class="rpg-token token-tn">TN</span> 6, cae tras 1 impacto. En cantidad, crea presión. Venganza al fallar: −1 Corazón.
- **Élite:** <span class="rpg-token token-tn">TN</span> 8, 2 Heridas. Normalmente tiene 1 rasgo defensivo o movilidad. Venganza al fallar: −1 Corazón; a veces efecto adicional situacional.
- **Jefe:** <span class="rpg-token token-tn">TN</span> 12, 3 Heridas. Tiene 2–3 movimientos especiales e influye en el terreno/ritmo. Puede provocar pruebas en los jugadores (por ejemplo, esquivar, estabilización).



---

### Bruto (combate cuerpo a cuerpo):

- **Bruto (combate cuerpo a cuerpo):** presiona en el cuerpo a cuerpo, empuja fuera de la cobertura.
- **Skirmisher (móvil):** entra/sale del contacto, castiga la soledad.
- **Artillería (distancia):** dispara desde detrás de la cobertura, obliga a moverse.
- **Controlador (control):** crea zonas de peligro, humo, campos de empuje.
- **Soporte (apoyo):** refuerza a los aliados, disminuye la <span class="rpg-token token-tn">TN</span> de los aliados o aumenta la <span class="rpg-token token-tn">TN</span> de los héroes en 1 grado según la situación.



---

### 1. Introducción

Añade 1–2 al statblock. Siempre funcionan descriptivamente; cambian la <span class="rpg-token token-tn">TN</span> en 1 grado solo cuando tiene sentido.
- **Escudo Natural:** a distancia, el oponente generalmente tiene cobertura parcial (ataque contra él → <span class="rpg-token token-tn">TN</span> +1 grado).
- **Armadura Ligera:** la primera pérdida de 1 Corazón por represalia contra esta unidad en la escena es ignorada.
- **Duro:** el primer éxito contra esta unidad no inflige Herida (solo rechaza/posición) — bueno para jefes.
- **Rápido (Movimiento 6):** ignora 1 casilla de terreno difícil por turno.
- **Escalador/Saltador:** se mueve verticalmente/sobre obstáculos como si estuviera en terreno llano, salto de 3 casillas.
- **Vuelo:** ignora obstáculos de terreno (el GM se encarga de las coberturas razonables).
- **Explorador:** es más difícil sorprenderlo; el primer intento de sigilo contra él tiene <span class="rpg-token token-tn">TN</span> +1.
- **Resistencia [tipo]:** el primer efecto de ese tipo en la escena es reducido (el GM explica: menor alcance, menor duración).
- **Vulnerabilidad [tipo]:** contra este tipo de ataques, la <span class="rpg-token token-tn">TN</span> es 1 grado más baja.
- **Enjambres:** cuando está al lado del objetivo, la represalia en un fallo puede afectar a dos héroes en un rango de 1.



---

### 1. Introducción

Elige 1–2 características. Los movimientos describen el efecto; si amenazan a los héroes, el DJ puede pedirles que realicen una prueba correspondiente (Z o M) contra la <span class="rpg-token token-tn">TN</span> del oponente.
- **Empuje (Brute):** tras golpear a un héroe, además muévelo 1–2 casillas.
- **Ruptura de Protección:** cuando esta unidad golpee, la protección del objetivo deja de funcionar hasta el final del siguiente turno.
- **Tirón (Skirmisher):** entrar/salir del combate cuerpo a cuerpo no provoca represalias.
- **Salva (Artillery):** área 3×3; todos en el área realizan una prueba Z contra <span class="rpg-token token-tn">TN</span>; fracaso: −1 Corazón y empujón de 1 casilla.
- **Ancla (Controller):** el área 3×3 se convierte en "terreno pegajoso" (entrar cuesta toda la Acción) hasta el final del siguiente turno.
- **Refuerzo (Support):** un aliado tiene una ventaja de 1 grado hasta el final de la ronda (los que lo atacan tienen <span class="rpg-token token-tn">TN</span> +1).
- **Invocación (Boss):** una vez al inicio, invoca 2 secuaces en casillas libres.
- **Barricada (Boss):** hasta el final de la ronda del lado divino, los héroes realizan ataques a distancia con <span class="rpg-token token-tn">TN</span> +1.
- **Impacto (Boss):** todos en un rango de 2 casillas realizan una prueba S vs <span class="rpg-token token-tn">TN</span>; fracaso: −1 Corazón o derribo (pierdes Movimiento en este turno).



---

### 1. Introducción

1) **Elige una clase:** Cono / Élite (2 Heridas) / Jefe (3 Heridas).
2) **Establece <span class="rpg-token token-tn">TN</span>:** 6 / 8 / 12 (excepcionalmente 4 para muy débiles o 10 para élites duras).
3) **Asigna un rol:** Bruto, Skirmisher, Artillería, Controlador, Soporte.
4) **Añade 1–2 rasgos** y **1 movimiento especial** (Jefe: 2–3 movimientos).
5) **Movimiento:** normalmente 5; cambia solo si es crucial.

Listo. Este esqueleto funciona en todas las realidades.



---

### 1. Introducción

7.2 Cambia las entradas por nombres/colores del mundo.

### 7.1 Conos
- **Guardia Cono — Cono, <span class="rpg-token token-tn">TN</span> 6, —, Bruto, Movimiento 5, Especial: Escudo Natural.**
- **Explorador Cono — Cono, <span class="rpg-token token-tn">TN</span> 6, —, Skirmisher, Movimiento 6, Especial: Explorador.**
- **Tirador Cono — Cono, <span class="rpg-token token-tn">TN</span> 6, —, Artillería, Movimiento 5, Especial: Salva (área pequeña 2×2, solo advierte: en fallo -1 Corazón).**
- **Controlador Cono — Cono, <span class="rpg-token token-tn">TN</span> 6, —, Controlador, Movimiento 5, Especial: Ancla (por 1 turno, una vez).**
- **Apoyo Cono — Cono, <span class="rpg-token token-tn">TN</span> 6, —, Apoyo, Movimiento 5, Especial: Refuerzo (una vez por escena).**

### 7.2 Elidades
- **Guardia Élite — Élite, <span class="rpg-token token-tn">TN</span> 8, Heridas 2, Bruto, Movimiento 5, Especial: Armadura Ligera; Embestida.**
- **Asesino Élite — Élite, <span class="rpg-token token-tn">TN</span> 8, Heridas 2, Skirmisher, Movimiento 6, Especial: Tirón; Vulnerabilidad [observación] (más fácil de detectar).**
- **Francotirador Élite — Élite, <span class="rpg-token token-tn">TN</span> 8, Heridas 2, Artillería, Movimiento 5, Especial: Cobertura Natural; Salva (3×3 tras preparación).**
- **Controlador Élite — Élite, <span class="rpg-token token-tn">TN</span> 8, Heridas 2, Controlador, Movimiento 5, Especial: Ancla; Empuje de 1 casilla con éxito excepcional.**
- **Médico Élite — Élite, <span class="rpg-token token-tn">TN</span> 8, Heridas 2, Soporte, Movimiento 5, Especial: Refuerzo; al impactar, elimina 1 complicación de un aliado (descriptivamente).**

### 7.3 Jefes
- **Líder — Jefe, <span class="rpg-token token-tn">TN</span> 12, Heridas 3, Soporte, Movimiento 5, Especial: Invocación; Refuerzo; Barrera.**
- **Coloso — Jefe, <span class="rpg-token token-tn">TN</span> 12, Heridas 3, Bruto, Movimiento 5, Especial: Embestida (hasta 2 casillas); Resistente; Sacudida.**
- **Cazador — Jefe, <span class="rpg-token token-tn">TN</span> 12, Heridas 3, Escaramuzador, Movimiento 6, Especial: Tirón; Explorador; Salva (saltar — después del movimiento).**
- **Táctico — Jefe, <span class="rpg-token token-tn">TN</span> 12, Heridas 3, Controlador, Movimiento 5, Especial: Ancla (mantener por 1 Mana/recurso de turno); Barrera; Invocación (1 peón/ turno hasta un máximo de 3).**



---

### 1. Introducción

Peligro es un "oponente sin sentido" o un efecto ambiental. Funciona por turnos o por activación.
Formato: **Nombre — <span class="rpg-token token-tn">TN</span>, Efecto, Cómo desactivarlo**
- **Torreta — <span class="rpg-token token-tn">TN</span> 8, Efecto: en el turno de los oponentes, cada uno en la línea de tiro realiza una prueba Z vs <span class="rpg-token token-tn">TN</span>, fallo: −1 Corazón; Desactivación: prueba M o Z <span class="rpg-token token-tn">TN</span> 8 junto al panel.**
- **Trampa — <span class="rpg-token token-tn">TN</span> 6, Efecto: entrar en el área obliga a realizar una prueba Z; fallo: inmovilización o −1 Corazón; Desactivación: Z <span class="rpg-token token-tn">TN</span> 6 con herramientas.**
- **Campo Repulsivo — <span class="rpg-token token-tn">TN</span> 8, Efecto: al inicio del turno empuja 2 casillas hacia el borde; Desactivación: M <span class="rpg-token token-tn">TN</span> 8 (dispersión) o corte de energía (S <span class="rpg-token token-tn">TN</span> 6).**
- **Gas/Humo — <span class="rpg-token token-tn">TN</span> 6, Efecto: en el área 3×3 prueba M o Z; fallo: punto ciego/−1 Corazón; Desactivación: ventilación (S) o sellado (Z).**



---

### 1. Introducción

Elige 1 de cada fila (o tira un [token:<span class="rpg-token token-d6">d6</span>]):
1. Objetivo de la escena: transición / recuperación / desactivación / escolta / robo / defensa
2. Terreno principal: abierto / pasillos estrechos / multicapas / cubiertas modulares / bordes peligrosos / niebla-humo
3. Oponentes: 6× peón / 4× peón + élite / 2× élite / jefe / jefe + 2× peón / élite + azar
4. Ventaja del oponente: cobertura / altura / movilidad / cuenta atrás / cuellos de botella / apoyo remoto
5. Ventaja de los jugadores: sorpresa / nivel superior / herramientas / barrera corta / atajo / aliado neutral



---

### 1. Introducción

En lugar de <span class="rpg-token token-tn">TN</span> numéricas, usa grados:
- **Peón:** "Normal" (equivalente a <span class="rpg-token token-tn">TN</span> 6)
- **Élite:** "Difícil" (+1 grado)
- **Jefe:** "Heroico" (+2 grados) y 3 Heridas
Las características y movimientos funcionan de la misma manera; cuando se menciona "<span class="rpg-token token-tn">TN</span> +1" en la descripción, aumenta el grado.



---

### 7.2 Si la pelea dura demasiado poco

- Si la pelea dura demasiado poco: añade secuaces en oleadas (2/turno) o aumenta la <span class="rpg-token token-tn">TN</span> en 1 grado a favor de los oponentes que tienen ventaja de posición.
- Si la pelea se alarga: permite el éxito excepcional con más frecuencia creando oportunidades (mejor posición), o reduce la <span class="rpg-token token-tn">TN</span> para los enemigos debilitados.
- Dos élites ≈ pequeño jefe; jefe + 4 secuaces ≈ enfrentamiento final en una sesión de 2 horas.



---

### 7.2. Guardia de Defensa — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Artillería, Movimiento 5, Especial: Protección Natural.

- **Guardia de Defensa — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Artillería, Movimiento 5, Especial: Protección Natural.**
- **Patrulla Móvil — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Skirmisher, Movimiento 6, Especial: Explorador.**
- **Asalto Pesado — Élite, <span class="rpg-token token-tn">TN</span> 8, Heridas 2, Bruto, Movimiento 5, Especial: Armadura Ligera; Embestida.**
- **Táctico de Campo — Élite, <span class="rpg-token token-tn">TN</span> 8, Heridas 2, Controlador, Movimiento 5, Especial: Ancla; Refuerzo.**
- **Líder de Campo — Jefe, <span class="rpg-token token-tn">TN</span> 12, Heridas 3, Soporte, Movimiento 5, Especial: Invocación; Barrera; Refuerzo.**
- **Coloso Terrenal — Jefe, <span class="rpg-token token-tn">TN</span> 12, Heridas 3, Bruto, Movimiento 5, Especial: Resistente; Sacudida; Embestida.**

---
Este es un conjunto de herramientas para crear rápidamente enemigos. Establece <span class="rpg-token token-tn">TN</span>, elige clase y rol, añade 1–2 características y movimiento — y tendrás un enemigo jugable listo para el tablero.

