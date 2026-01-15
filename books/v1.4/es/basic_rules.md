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
generated_at: "2026-01-15T08:02:46.285Z"
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
# Libro de Reglas Básicas



---



---

### Cosas necesarias para jugar

- Lápiz y hoja de personaje.
- (Opcionalmente) mapa/rejilla de cuadros y marcadores de personajes (papel cuadriculado, tapete, VTT).
- Dados: **<span class="rpg-token token-d4">k4</span>, <span class="rpg-token token-d6">k6</span>, <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-d20">k20</span>**.
  - En la práctica, es suficiente **uno de cada uno** (se lanza un dado a la vez).
  - (Opcionalmente) **k100** para tablas aleatorias o generadores.
- Si solo tienen **<span class="rpg-token token-d6">k6</span>**, usen la variante **2k6** (al final).

---



---

### Glosario de términos


Te palabras aparecen en las reglas — aquí están explicadas "en términos simples":

- **DJ (Dungeon Master)**: dirige el mundo, describe situaciones, controla enemigos, establece la Dificultad y las consecuencias.
- **Jugador**: describe las acciones de su personaje y realiza tiradas.
- **Prueba**: tirada de dados que resuelve un resultado incierto.
- **Atributos**: **Fuerza (F)**, **Destreza (D)**, **Poder (<span class="rpg-token token-stat">P</span>)**. Indican *qué dado lanzas*.
- **Dado de atributo**: tamaño del dado asignado al atributo (por ejemplo, D = <span class="rpg-token token-d12">d12</span>).
- **Dificultad (D)**: número que se debe alcanzar o superar para que la acción tenga éxito.
- **Éxito**: resultado ≥ Dificultad.
- **Éxito excepcional**: **resultado máximo** en el dado (por ejemplo, 12 en <span class="rpg-token token-d12">d12</span>, 20 en <span class="rpg-token token-d20">d20</span>) — éxito + beneficio adicional.
- **Complicación**: problema adicional tras un fracaso (ruido, pérdida de tiempo, peor posición, pérdida de recurso).
- **Éxito con costo**: la acción tiene éxito, pero pagas un precio (compromiso, pérdida de recurso, revelación, riesgo).
- **Golpe de Suerte (GS)**: recurso limitado que permite salvar escenas (re-tirada / aumento de dado / convertir un fracaso en éxito con costo).
- **Corazones**: "vida" del personaje (resistencia, heridas, condición — dependiendo del mundo).
- **Puntos de Poder (PP)**: recurso para poderes y jugadas "más allá de lo estándar" (magia, psiónica, gadgets, acciones "cinematográficas").
- **Defensa**: umbral para golpear al enemigo en combate (en lugar de multiplicar reglas sobre armadura, clase de armadura, etc.).
- **Cobertura**: obstáculo entre tú y el objetivo. Generalmente dificulta ataques a distancia o acciones de observación.

---



---

### 1. Personaje


La creación de personajes es breve. Un personaje es: **concepto + rol + características + recursos + equipo**.

---

### 1.1 Concepto

Una frase: quién eres y en qué género juegas.

> Ejemplo: "Era una agente de la corporación, hoy cazadora de recompensas, que actúa en silencio y no confía en nadie."


### 1.2 Rol (elige uno)


Rol son intencionadamente "neutras para el mundo". En fantasía puedes llamarlas de otra manera, en ciberpunk de otra, pero funcionan igual.

- **Asalto** — presión, combate, forzar obstáculos, romper la línea del frente.
- **Especialista** — sigilo, precisión, técnica, observación, plan.
- **Adepto** — poderes, influencia, conocimiento, improvisación (magia/psiónica/tecnología dependiendo del mundo).


### 1.3 Atributos y dados


Tienes tres atributos:

- **Fuerza (F)** — fuerza física, resistencia, combate cuerpo a cuerpo, empuje.
- **Destreza (D)** — reflejos, precisión, sigilo, disparo, conducción.
- **Poder (<span class="rpg-token token-stat">P</span>)** — "lo especial": magia, psiónica, tecnología avanzada, engaño social, intuición — dependiendo de la convención.

**Al inicio, distribuye los dados así:**
- un atributo tiene **<span class="rpg-token token-d12">k12</span>**,
- uno tiene **<span class="rpg-token token-d8">k8</span>**,
- uno tiene **<span class="rpg-token token-d6">k6</span>**.

**Distribución sugerida según el rol (de manera más simple):**
- **Asalto:** F <span class="rpg-token token-d12">k12</span>, D <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-stat">P</span> <span class="rpg-token token-d6">k6</span>
- **Especialista:** D <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">P</span> <span class="rpg-token token-d8">k8</span>, F <span class="rpg-token token-d6">k6</span>
- **Adepto:** <span class="rpg-token token-stat">P</span> <span class="rpg-token token-d12">k12</span>, D <span class="rpg-token token-d8">k8</span>, F <span class="rpg-token token-d6">k6</span>

> Ejemplo: si tienes D = <span class="rpg-token token-d12">k12</span>, entonces al disparar, sigilar y esquivar, normalmente tiras <span class="rpg-token token-d12">k12</span>.

### 1.4 Recursos

- **Corazones:** 5.
- **Puntos de Poder (PP):** 3.
- **Suerte (<span class="rpg-token token-stat">S</span>):** al comienzo de cada sesión tienes **2 <span class="rpg-token token-stat">S</span>**.

**Suerte (cómo funciona):** gasta **1 <span class="rpg-token token-stat">S</span>** para elegir una:
- **Repetición** de tu prueba (dejas el mejor resultado), o
- **Aumento del dado en 1 nivel** para esa tirada (**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>**), o
- **Cambio de un fallo a un “éxito con costo”** — la acción tiene éxito, pero el DJ inmediatamente impone un precio (por ejemplo, ruido, pérdida de tiempo, pérdida de recurso, peor posición, atracción de atención, daño al equipo).

**Recuperación de <span class="rpg-token token-stat">S</span>:** al comienzo de la siguiente sesión vuelves al límite. El DJ puede otorgar **+1 <span class="rpg-token token-stat">S</span>** por un riesgo audaz, una gran decisión narrativa o jugar con las consecuencias.

### 1.5 Talentos (opcionales, pero recomendados)

Los talentos son **2 frases cortas** que describen en qué es buena tu personaje (sin lista, sin tablas).

- Ejemplos: "Mecánico", "Explorador", "Negociador", "<span class="rpg-token token-stat">M</span>édico", "Hackers", "Veterano", "Descubridor".

**Cómo funcionan los Talentos:** si un Talento ayuda realmente en la prueba, el DJ puede **aumentar el dado en 1 grado** (o neutralizar la dificultad).
- Un Talento no otorga éxitos automáticos.
- Normalmente, **máximo 1 Talento** influye en una prueba.

### 1.6 Equipo

Escribe:
- 1 herramienta "clave" (arma / conjunto / equipo, sin el cual no haces tu trabajo),
- 1 protección (armadura, escudo, camuflaje — dependiendo del mundo),
- 3 objetos pequeños útiles en la aventura.

El equipo en el núcleo de las reglas es principalmente **un permiso** (permite acciones), y no un bono numérico.

### 1.7 Ejemplo de personaje completo

- Concepto: "Ladrón de información que roba datos de los sistemas, no de los bolsillos."
- Rol: Especialista
- Atributos: <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">k6</span>, <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span>
- Recursos: 5 Corazones, 3 <span class="rpg-token token-power">PM</span>, 2 LS
- Talentos: "Hacker", "Sombra"
- Equipo: pistola, armadura ligera, kit de infiltración, cuerda, linterna

---



---

### 2. Núcleo de reglas: pruebas

Esta parte es la más importante: si la entiendes, entiendes el sistema.

### 2.1 Cuándo haces una prueba

Haces una prueba cuando se cumplen ambas condiciones:
1) el resultado es incierto (puede tener éxito o no), y
2) la apuesta es real (un fracaso cambia algo / cuesta algo).

Si la acción es trivial y sin presión, el DJ puede decir "tuviste éxito" sin tirar.

### 2.2 Cómo realizar una prueba (paso a paso)

1) El jugador dice **qué hace** y **por qué**.
2) El MJ elige un atributo: **F** o **D** o **<span class="rpg-token token-stat">M</span>**.
3) El MJ establece la **Dificultad (D)** y dice qué significa el fracaso (la apuesta).
4) El jugador tira **el dado del atributo**.
5) Compara el resultado con D y determina las consecuencias.

### 2.3 Dificultades (T)


Usamos umbrales simples. Si tienes dudas, elige un umbral más bajo y la "dificultad" se mostrará con consecuencias.

- **T 3** – fácil (casi seguro, pero a veces vale la pena comprobar bajo presión)
- **T 4** – estándar (desafío típico)
- **T 5** – difícil (requiere competencia o ventaja)
- **T 6** – muy difícil (sin ventaja es arriesgado)
- **T 8** – heroico (para los mejores o tras una buena preparación)
- **T 12** – legendario (raramente "en limpio"; generalmente como objetivo de campaña, plan, ritual, grandes condiciones)


### 2.4 Resultados de la prueba

- **Resultado ≥ T → Éxito.** Logras el efecto deseado.
- **Resultado < T → Fracaso.** No logras el efecto, y la situación cambia (complicación o costo).
- **Salió un 1 → Fracaso + complicación.** La complicación entra seguro.
- **Resultado máximo en el dado → Éxito excepcional.**
  - Además del éxito, obtienes **un beneficio adicional** (más rápido, más silencioso, más fuerte, más seguro, efecto adicional).

> Ejemplo de éxito con costo: “Lograste abrir la puerta, pero haces ruido y alguien viene a investigar.”

### 2.5 Facilidades y dificultades (sin contar)


En lugar de añadir +1/−1 a las tiradas, cambiamos el **tamaño del dado**.

- **Situación favorable** → **sube el dado 1 grado**  
  <span class="rpg-token token-d6">k6</span> → <span class="rpg-token token-d8">k8</span> → <span class="rpg-token token-d12">k12</span> → <span class="rpg-token token-d20">k20</span>
- **Situación desfavorable** → **baja el dado 1 grado**  
  <span class="rpg-token token-d20">k20</span> → <span class="rpg-token token-d12">k12</span> → <span class="rpg-token token-d8">k8</span> → <span class="rpg-token token-d6">k6</span> → <span class="rpg-token token-d4">k4</span>

**Ejemplos de facilidades:** preparación, buenas herramientas, ventaja de posición, sorpresa, apoyo.  
**Ejemplos de dificultades:** oscuridad, resbaladizo, presión del tiempo, ruido, distracción, cobertura.

**Regla de orden:** para mayor rapidez, asume que para una sola prueba generalmente aplicas **máximamente 1 facilidad y 1 dificultad** (pueden cancelarse entre sí).

### 2.6 Ayuda de un aliado

Un aliado puede dedicar su acción (o tiempo en la escena fuera de combate) para ayudar.

**Efecto:** en esta única prueba **aumenta el dado en 1 grado**.

La ayuda debe ser descrita de manera sensata (cubrir, proporcionar herramientas, distraer, estabilizar, dar indicaciones).

### 2.7 Repetición de pruebas

Si la prueba no tuvo éxito, no la repitas "una y otra vez" sin cambiar la situación.
- O haces algo diferente (otra característica / otras herramientas / otro camino),
- o aceptas el costo (tiempo, alarma, recurso),
- o te retiras.

### 2.8 Ejemplos de pruebas (fuera de combate)

**Ejemplo A — paso silencioso**
- Jugador: "Cruzaré el patio antes de que el reflector regrese."
- MJ: Destreza (D). Es bajo presión de tiempo → Dificultad **D 5**.
- El personaje tiene el Talento "Sombra" → ventaja, dado aumentado en 1 grado.
- Tirada: D <span class="rpg-token token-d12">k12</span> = 4 → fracaso. MJ: "No te notan de inmediato, pero alguien escucha un susurro y comienza a revisar el área (complicación: aumenta la presión)."

**Ejemplo B — forzar con fuerza**
- Jugador: "Forzaré la puerta de metal antes de que la seguridad llegue a la esquina."
- MJ: Fuerza (F), Dificultad **D 6** (muy difícil sin herramientas).
- Alguien ayuda, sosteniendo la cerradura y bloqueando la puerta → dado aumentado en 1 grado.
- Tirada: F <span class="rpg-token token-d12">k12</span> = 12 → éxito excepcional: la puerta se abre de inmediato y lo haces más silenciosamente de lo que se esperaba.



---

### 3. Movimiento y distancias (la cuadrícula es una opción)

Por defecto, NDE funciona sin mapa: describes la escena y las posiciones de los personajes.

### 3.1 Por defecto: distancias descriptivas


Usa cuatro zonas:
- **Cerca** — al alcance de la mano, combate cuerpo a cuerpo.
- **No muy lejos** — unos pasos, fácil acercamiento.
- **Lejos** — el otro lado de la escena, requiere un movimiento claro.
- **Muy lejos** — francotirador/vehicular/"en el límite de la escena".

En un turno, normalmente puedes cambiar la distancia por **una zona** (por ejemplo, Lejos → No muy lejos).


### 3.2 Opción: juego en cuadrícula (para tácticas)


Si prefieren lo concreto:
- 1 cuadrícula = 1–2 m.
- Movimiento en un turno: **hasta 5 cuadrículas**.
- Las diagonales están permitidas (se cuentan como una cuadrícula normal).


### 3.3 Cobertura y línea de acción

- **Cobertura total:** no se puede interactuar "en línea" (disparo, observación, muchos poderes).
- **Cobertura parcial:** dificulta — generalmente **reduce el dado en 1 grado** para el atacante/observador.

---



---

### 4. Combate

El combate es una escena ordinaria con pruebas, solo que ordenada en turnos.

### 4.1 Cuándo comienza la lucha

La lucha comienza cuando:
- al menos una parte quiere hacer daño a la otra, y
- es importante quién y cuándo actúa.

Si la situación es breve y obvia, el DJ puede resolverla con una sola tirada.

### 4.2 Orden de turnos (versión simple)

Lo más simple:
- Primero actúan todos los jugadores (en cualquier orden),
- luego actúan los oponentes,
- y así en un bucle.

### 4.3 Qué haces en tu turno


En tu turno tienes:
- **Movimiento** (cambio de zona / hasta 5 casillas en la variante de cuadrícula),
- **1 Acción** (ataque, prueba, ayuda, uso de poder, equipo, interacción con la escena).


### 4.4 Ataque: cómo funciona

1) Elige un objetivo y describe el ataque.
2) Elige un atributo:
   - **cuerpo a cuerpo** → tirada de **Fuerza (F)**,
   - **distancia** → tirada de **Destreza (D)**,
   - **poderes** → normalmente tirada de **Poder (<span class="rpg-token token-stat">P</span>)** (ver capítulo 5).
3) Establece la **Defensa** del objetivo.
4) Lanza el dado y compáralo con la Defensa.

### 4.6 Daños y 'cuánto aguantan'

- Un golpe causa **1 Corazón**.
- **Éxito excepcional** causa **2 Corazones** *o* proporciona un efecto fuerte (desarme, derribo, empuje fuera de cobertura) — elige uno.

Arquetipos más simples de enemigos:
- **Esbirro:** cae tras 1 golpe.
- **Élite:** tiene **2 Corazones**.
- **Jefe:** tiene **3 Corazones** (o 5 en escenas finales).

> Nota: “caer” no necesariamente significa muerte. Puede estar inconsciente, haber huido, rendido, o haber sido sacado de la acción.

### 4.5 Defensa de los oponentes (orientativamente)

- **Débil:** Defensa **4**
- **Típico:** Defensa **5**
- **Élite:** Defensa **6**
- **Jefe:** Defensa **8** (jefe legendario: **12**)

La cobertura y las condiciones suelen cambiar el tamaño de los dados del atacante (facilitaciones/dificultades), y no la Defensa.

### 5.7 Rango de ataques (predeterminado)
Para no multiplicar números, utiliza reglas simples:
- A quemarropa: objetivo en la casilla adyacente.
- Distancia: objetivo en "rango de visión" en el tablero.
  - Si el MJ desea limitaciones: acepta **hasta 10 casillas** sin penalización; más de 10 casillas <span class="rpg-token token-<span class="rpg-token token-math">tn</span>"><span class="rpg-token token-math">TN</span></span> +1 grado.

### 5.8 Varios oponentes a la vez
Si varios matones están "en combate" con un personaje, el MJ puede:
- aumentar la <span class="rpg-token token-<span class="rpg-token token-math">tn</span>"><span class="rpg-token token-math">TN</span></span> en 1 grado (presión), o
- considerar que un fallo significa una complicación adicional (por ejemplo, pierdes la posición).

La regla debe ser rápida: **una resolución → un efecto**.

### 4.7 Ejemplos de combate

**Ejemplo A — combate cuerpo a cuerpo con un esbirro**
- Asalto (<span class="rpg-token token-stat">S</span> <span class="rpg-token token-d12">k12</span>) ataca al esbirro (Defensa 5).
- Las condiciones son buenas (sorpresa) → el dado se incrementa en 1 grado, pero ya es <span class="rpg-token token-d12">k12</span>, así que el incremento da <span class="rpg-token token-d20">k20</span>.
- Tiro <span class="rpg-token token-d20">k20</span> = 7 → impacto, el esbirro cae.

**Ejemplo B — disparo a la élite desde cobertura**
- Especialista (<span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">k12</span>) dispara a la élite (Defensa 6).
- El objetivo está parcialmente cubierto → dificultad, el dado baja a <span class="rpg-token token-d8">k8</span>.
- Tiro <span class="rpg-token token-d8">k8</span> = 6 → impacto, la élite pierde 1 Corazón (le queda 1).

**Ejemplo C — jefe y Golpe de Suerte**
- Adepto (<span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">k12</span>) intenta incapacitar al jefe (Defensa 8) con poder.
- Tiro <span class="rpg-token token-d12">k12</span> = 4 → fracaso. El jugador gasta 1 GS para volver a tirar.
- Re-tiro = 10 → éxito. El jefe pierde 1 Corazón, pero el MJ añade un costo: “el efecto es ruidoso, se activa la alarma.”

---



---

### 5. Poderes (<span class="rpg-token token-stat">P</span>) y Puntos de Poder (PP)

En NDE, "Poder" es una categoría de efectos especiales. Dependiendo del mundo, puede significar:
- magia, psiónica, rituales,
- tecnología avanzada, drones, hacking "en vivo",
- jugadas cinematográficas de los héroes (por ejemplo, "concentración maestra"),
- influencia social en juegos donde la conversación es "poder".

### 5.1 Cuándo gastas <span class="rpg-token token-power">PM</span>

Gastas <span class="rpg-token token-power">PM</span> cuando intentas obtener un efecto **por encima del estándar**.

---

### 5.2 Cómo usar el poder (paso a paso)

1) Describe el efecto que deseas lograr.
2) El DJ establece la Dificultad y el costo de <span class="rpg-token token-power">PM</span>.
3) Gasta <span class="rpg-token token-power">PM</span>.
4) Lanza **<span class="rpg-token token-stat">M</span>** y compáralo con la Dificultad.

**Fracaso:** el efecto no funciona; <span class="rpg-token token-power">PM</span> se pierde; entra una complicación (sobrecarga, rastro, revelación, efecto secundario).

### 5.3 Niveles de efectos (Dificultad / costo)

- **Truco** (truco corto): **D 4 / 0–1 <span class="rpg-token token-power">PM</span>**  
  luz, sonido, pequeña cortina, distracción momentánea.
- **Estándar**: **D 5 / 1 <span class="rpg-token token-power">PM</span>**  
  proyectil, escudo, impulso, salto, refuerzo.
- **Fuerte**: **D 6 / 2 <span class="rpg-token token-power">PM</span>**  
  área, control, curación, parálisis, "hackeo en combate".
- **Grande**: **D 8–12 / 3 <span class="rpg-token token-power">PM</span>**  
  efecto que cambia la escena o tiene consecuencias de campaña.

### 5.4 Éxito excepcional en poder


Si obtienes el máximo en el dado <span class="rpg-token token-stat">M</span>:
- aumenta la escala (área más grande / más tiempo / más fuerte), o
- añade un beneficio adicional (más silencioso, más preciso, más seguro), o
- el DJ puede devolver **1 <span class="rpg-token token-power">PM</span>** (si encaja con la ficción).


### 5.5 Recuperación de <span class="rpg-token token-power">PM</span>

- Después de la escena de conflicto recuperas **1 <span class="rpg-token token-power">PM</span>**.
- Tras un descanso seguro, vuelves a estar al máximo.

### 5.6 Ejemplos de poderes

**Ejemplo A — escudo para correr**
- Jugador: "Coloco una corta cobertura para correr a una mejor posición."
- MJ: **D 5**, costo 1 <span class="rpg-token token-power">PM</span>.
- Tirada <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">d12</span> = 9 → éxito: corres de forma segura.

**Ejemplo B — fracaso con consecuencia**
- Jugador: "Detengo a la élite en su lugar."
- MJ: Fuerte **D 6**, costo 2 <span class="rpg-token token-power">PM</span>.
- Tirada = 1 → fracaso + complicación: pierdes 2 <span class="rpg-token token-power">PM</span>, y el efecto rebota y revela tu posición.



---

### 6.1 0 Corazones

Si caes a 0 Corazones:
- estás **fuera de acción** (herido, aturdido, en shock — dependiendo de la convención),
- un aliado puede sacrificar una acción para levantarte con **1 Corazón**.

### 6.2 Descanso

- Después de una escena de conflicto, si tienen un momento de respiro y las condiciones básicas, pueden volver a tener Corazones plenos.
- En campañas más severas, el MJ puede requerir un descanso seguro para volver a la plenitud.

### 7.3 Descanso
Después de una escena de combate/conflicto, si tienen un momento de descanso seguro (y las condiciones básicas), regresan a la plenitud:
- Corazones,
- Maná.

Esto mantiene el sistema ágil y no requiere un largo proceso de curación.



---

### 7. Desarrollo de personajes

**Cuando creces:** después de una aventura, misión o capítulo importante de la historia (normalmente cada 1–3 sesiones).

Elige **uno**:
- **Aumenta** un atributo en 1 grado de dado (máx. hasta <span class="rpg-token token-d20">k20</span>), o
- **+1 Corazón** (máx. 7), o
- **+1 <span class="rpg-token token-power">PM</span>** (máx. 5), o
- **Nueva Ventaja** (una habilidad específica acordada con el DJ).

> Ejemplo: El especialista aumenta <span class="rpg-token token-stat">Z</span> de <span class="rpg-token token-d12">k12</span> a <span class="rpg-token token-d20">k20</span>, porque la campaña ha entrado en una etapa de persecuciones y tiroteos.

---



---

### 8. Variante solo <span class="rpg-token token-d6">k6</span>: 2k6

Si no quieren usar diferentes dados, jueguen con **2k6**.

### 8.1 Características como modificadores


En lugar de tamaños de dados, separa los modificadores:
- una característica tiene **+2**
- una tiene **+1**
- una tiene **+0**


### 8.2 Prueba


Lanza **2d6 + modificador de característica**.

**Resultado:**
- **6 o menos** – fracaso con consecuencia
- **7–9** – éxito con costo
- **10+** – éxito completo
- **12** – éxito excepcional (beneficio adicional)

### 8.3 Dificultad de la situación


En lugar de cambiar los umbrales, otorga:
- **+1** por ventaja, preparación, buen plan,
- **−1** por dificultades, presión, cobertura, caos.

### 8.4 Suerte en 2d6

Gasta 1 PE para:
- volver a tirar 2d6, o
- añadir **+1** al resultado de la prueba, o
- convertir un fallo en un éxito con coste.

### 8.5 Mapeo rápido (opcional)

Si alguna vez deseas "recalcular" un personaje entre variantes:
- <span class="rpg-token token-d6">k6</span> ≈ +0
- <span class="rpg-token token-d8">k8</span> ≈ +1
- <span class="rpg-token token-d12">k12</span> ≈ +2
- <span class="rpg-token token-d20">k20</span> ≈ +3 (para muy experimentados)

---



---

[ES] Marcador de posición...




---

### 1. Introducción

7.2 Los complementos no son obligatorios, pero a veces facilitan la gestión.

### 9.1 Protección (armadura) como recurso simple


Si deseas que la "protección" tenga un efecto claro:
- la personaje con protección tiene **1 ficha de Armadura por escena**, 
- cuando debería perder 1 Corazón, puede en su lugar gastar una ficha de Armadura.

### 9.2 Presión del tiempo como temporizador


Si la escena tiene un límite de tiempo, el DJ establece un "contador" (por ejemplo, 3 pasos). Cada fallo mueve el contador en 1. Cuando se llega al final, ocurre una consecuencia (alarma, huida del objetivo, colapso del pasaje).

---

### 9.3 Venganza (variante de combate arriesgado)

Si deseas que el combate sea más "agudo" y rápido:
- cuando **atacas cuerpo a cuerpo** y **fallas**, pierdes **1 Corazón**, siempre que el oponente pudiera alcanzarte realmente.
Esta es una variante; en el núcleo de NDE, las consecuencias de los fracasos en combate derivan principalmente de la ficción y las decisiones del DJ.

