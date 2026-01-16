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
generated_at: "2026-01-16T08:33:24.382Z"
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
# Guía del Director de Juego

Automatic translation placeholder for es

---



---

### 0) Reglas para dirigir en 30 segundos

- **Comienza con la ficción.** Primero describe la situación y las acciones de los jugadores, luego realiza la prueba.
- **Establece la apuesta antes de lanzar el dado.** Di: *qué está en juego* y *qué sucederá en caso de fallar*.
- **Una decisión → una tirada → un efecto significativo.** No dividas una intención en 3 pruebas.
- **El fracaso impulsa el juego hacia adelante.** No "resetees" la escena, cámbiala con una complicación, costo, o presión.
- **Mantén la consistencia.** Las mismas condiciones → dificultad similar, consecuencias similares.
- **La cuadrícula es opcional.** Por defecto, el juego funciona sin mapa: "Cerca / Lejos / Muy lejos / Muy muy lejos".



---

### 1.1. ¿Cuándo lanzar dados?

El lanzamiento solo tiene sentido cuando al mismo tiempo:
- el resultado **no es obvio**,
- existe una **apuesta real** (algo cambiará),
- ambas partes aceptan que **la mecánica tiene el derecho de decidir**.

**No lances** si:
- la acción es rutinaria y sin presión,
- el fracaso no aporta nada interesante,
- el éxito es seguro y el precio ya está pagado (por ejemplo, los jugadores tienen tiempo, herramientas y seguridad).

**Ejemplo (sin lanzamiento):** Un especialista tiene acceso administrativo y condiciones tranquillas: abrir una puerta estándar en la base no requiere una prueba.
**Ejemplo (con lanzamiento):** Las mismas puertas, pero hay una alarma activa y una patrulla se aproxima en 30 segundos: esto es una prueba, ya que la apuesta es el tiempo y la revelación.

### 1.2. Lista de verificación para la resolución (procedimiento de mesa)

1) El jugador dice: **qué hace** y **qué quiere lograr**.
2) Tú respondes: **qué se interpone** y **cuál es la apuesta**.
3) Eligen una característica: **Fuerza (F)** / **Destreza (D)** / **Poder (<span class="rpg-token token-stat">P</span>)**.
4) Determinas la **Dificultad (D)** o **Defensa** (en combate).
5) Estableces un modificador situacional: **aumentar/reducir los dados** y una posible **ayuda**.
6) Tirada → resultado → consecuencia → actualización de la escena.

Resumido: **Descripción → Apuesta → Característica → D/Defensa → Tirada → Consecuencia**.

---

### 1.3. Dificultad (D): escala y reglas prácticas

Usa una sola escala en todo el juego. Esto construye la confianza de los jugadores en las decisiones del Director del Juego (DJ).

- **D 3 – fácil:** condiciones favorables, sin presión, resistencia mínima.
- **D 4 – estándar:** "trabajo normal" en la aventura.
- **D 5 – difícil:** presión de tiempo, riesgo, oponente, ventana estrecha.
- **D 6 – muy difícil:** clara ventaja del enemigo, alto riesgo, acción compleja bajo estrés.
- **D 8 – heroico:** hazaña por encima del promedio; generalmente requiere ventaja, plan o recurso.
- **D 12 – legendario:** momento de "asombro"; rara vez sin preparación y a menudo con un gran costo.

**Regla práctica:** si no sabes qué establecer, comienza con **D 4** y luego justifica "hacia arriba" o "hacia abajo".

### 1.4. Modificadores sin contar: mejora/reduce el dado

En lugar de sumar bonos y penalizaciones, en NDE cambias el **tamaño del dado** para una tirada.

- **Mejor situación:** mejora el dado en 1 grado  
  <span class="rpg-token token-<span class="rpg-token token-d4">d4</span>"><span class="rpg-token token-d4">d4</span></span>→<span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">d8</span>"><span class="rpg-token token-d8">d8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">d12</span>"><span class="rpg-token token-d12">d12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d20">d20</span>"><span class="rpg-token token-d20">d20</span></span>
- **Peor situación:** reduce el dado en 1 grado (en la dirección opuesta).

**Ayuda de un aliado:** cuesta su acción y proporciona una **mejora del dado en 1 grado** en la tirada.

**Ejemplo:** Cerradura en silencio (T 4) vs cerradura bajo la lluvia y bajo fuego (T 5 + reducción del dado, porque las manos tiemblan y no hay visibilidad).  
Esto generalmente funciona mejor que "T 6 y +2 y -1".

---

### 1.5. Resultados de las pruebas: éxito, fracaso y ritmo del juego

- **1 en el dado:** fracaso + complicación (la complicación entra seguro).  
- **Resultado < T:** fracaso (pero la situación cambia).  
- **Resultado ≥ T:** éxito.  
- **Resultado máximo en el dado:** éxito excepcional (ventaja adicional).

#### ¿Cómo diseñar un fracaso para que no bloquee el juego?

Antes de que el jugador tire, determina 1–2 tipos de coste:
- **tiempo** (alguien llega, algo se cierra),
- **posición** (mala ubicación, expuesto),
- **recurso** (equipo, munición, energía, Punto de Poder),
- **atención** (alarma, sospechas, pista).

**Ejemplo (fail-forward):**  
El jugador quiere forzar una puerta. Un fracaso no significa "no abres".  
El fracaso significa: "abres, pero haces ruido – la patrulla está cerca ahora, y el nivel de alarma aumenta".



---

### 2) Un Golpe de Suerte (Ł<span class="rpg-token token-stat">S</span>): cómo apoyar la dramaturgia sin arruinar el juego

Cada héroe comienza la sesión con **2 Ł<span class="rpg-token token-stat">S</span>**. Esta es una herramienta de los jugadores, pero el Maestro del Juego es responsable de su "economía" en la mesa.

### 2.1. ¿En qué gastan los jugadores los PS?

Gasta 1 PS para:
- realizar un **re-roll** (conservar el mejor),
- **aumentar un dado en 1 grado** para una tirada,
- cambiar un fallo por un **éxito con coste** (el DM añade un precio).

### 2.2. ¿Cuándo otorgar un punto de suerte adicional?

El DJ puede otorgar **+1 punto de suerte** por:
- asumir conscientemente un riesgo que impulsa la escena,
- aceptar las consecuencias sin "negociar",
- encontrar una solución creativa que sea coherente con la convención,
- representar muy bien la relación, motivación o apuesta.

**Regla de higiene:** otorga con moderación (1-2 por sesión por persona en un juego extremadamente generoso). El punto de suerte debe ser una "chispa", no un combustible constante.



---

### 3) Conflicto y combate

NDE debe luchar rápidamente. Si el combate dura 60 minutos, casi siempre significa: demasiados enemigos "con <span class="rpg-token token-heart">HP</span>" o demasiadas tiradas menores.

### 3.1. Por defecto sin mapa: distancias escénicas

Usa cuatro distancias:
- **Cerca** – al alcance de la mano (cuerpo a cuerpo),
- **No muy lejos** – a unos pocos pasos,
- **Lejos** – al otro lado del escenario,
- **Muy lejos** – distancia de francotirador/vehículo.

En un turno, un personaje tiene: **Desplazamiento + 1 Acción**.
El desplazamiento generalmente cambia la distancia en **1 grado** (No muy lejos→Cerca).

**Ejemplo:** El guerrero está No muy lejos. En su turno: se acerca (Cerca) y ataca.

### 3.2. Opción: cuadrícula (grid) - cuando necesitas precisión

Si juegas en una cuadrícula:
- movimiento por turno: **hasta 5 casillas**,
- diagonales permitidas,
- el terreno difícil puede costar "2 casillas por 1 entrada" (opcional).

Todas las demás reglas permanecen idénticas.

### 3.3. Defensa de los enemigos y daño

En combate, en lugar de Dificultad, usas **Defensa** (un "D para la pelea").

**Defensa (orientación):**
- **Débil** 4
- **Típico** 5
- **Élite** 6
- **Jefe** 8 (jefe legendario 12)

**Ataque:** tirada de **Fuerza** (cuerpo a cuerpo) o **Destreza** (a distancia) contra la Defensa.

**Daño (ritmo):**
- un golpe inflige **1 Corazón**,
- un éxito excepcional inflige **2 Corazones** o provoca un efecto fuerte (desarme, derribo, desestabilización, distracción).

**Esbirros y élites (modelo recomendado):**
- **Esbirro:** 1 golpe = sale del combate (derrotado, huye, incapacitado).
- **Élite:** tiene **2 Corazones** (o “2 golpes”), a menudo tiene una ventaja táctica.
- **Jefe:** tiene **3 Corazones** + 1–2 "movimientos de jefe" (ver 3.6).

Esto proporciona enfrentamientos rápidos sin contar puntos.

### 3.4. Cobertura, ventaja y "terreno visible"

En lugar de multiplicar las reglas, usa un solo lenguaje: **dado arriba / dado abajo**.

- Cobertura ligera, humo, ángulo malo: **reduce el dado del atacante** en 1 grado.  
- Buena posición, sorpresa, ventaja de altura: **aumenta el dado** en 1 grado.  
- Cobertura total: el ataque es imposible hasta que la situación cambie.

**Ejemplo:** Un francotirador en la ventana está "Lejos" y tiene ventaja de altura → el atacante recibe una reducción en el dado.  
El equipo cambia de escena: granada de humo, flanqueo, rodeo – y la ventaja desaparece.

### 3.5. Orden en los combates sin contar iniciativa

Esquema recomendado y rápido:
1) **Los jugadores actúan** (en cualquier orden en la mesa).
2) **Los enemigos actúan**.
3) Repetir.

Esto permite a los jugadores planificar combinaciones cortas sin cargar la mesa con la iniciativa.

### 3.6. Cómo dirigir un jefe para que sea interesante (y no solo una 'esponja de daño')

Un jefe en NDE debería tener:
- **Defensa 8** (o 12 en la versión 'final de temporada'),
- **3 Corazones**, 
- **1-2 movimientos únicos** que cambien la escena.

**Ejemplos de movimientos de jefe (universales):**
- **Empujón:** alguien golpeado retrocede una distancia (Cerca→Lejos) y pierde su posición.
- **Rompimiento de cobertura:** el jefe destruye la cobertura o obliga a salir del escondite.
- **Llamada de apoyo:** se unen 2 lacayos o una élite (preferiblemente una vez por pelea).
- **Zona peligrosa:** el área se vuelve peligrosa (fuego, electricidad, runas) – quien permanezca en ella, arriesga una prueba.

**Regla:** el movimiento del jefe debe cambiar el terreno de juego, no solo 'infligir más daño'.

### 3.7. Moral y comportamiento de los enemigos (procedimiento sencillo)

Cuando:
- cae el primer esbirro, o
- la élite pierde su primer Corazón, o
- el jefe pierde su segundo Corazón,

tira un <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span> y decide:
- **1–2:** se retiran / buscan cobertura / negocian,
- **3–4:** mantienen la posición,
- **5–6:** avanzan agresivamente.

Modifica con **+1** si tienen ventaja, **-1** si están aterrorizados o aislados.



---

### 4) Poderes (<span class="rpg-token token-stat">M</span>) del lado del MG: cómo valorarlos y cómo no arruinar el ritmo

En NDE, el 'Poder' abarca magia, psiónica, cibernética, hackeo, carisma 'al nivel de película', dependiendo del mundo.

### 4.1. Escala de poder: Dificultad y coste de Puntos de Poder

- **Truco:** D 4, coste 0–1 PP (efecto pequeño y corto).  
- **Estándar:** D 5, coste 1 PP (objetivo único, salto corto, escudo).  
- **Fuerte:** D 6, coste 2 PP (área, control, curación).  
- **Gran:** D 8–12, coste 3 PP (efecto que cambia la escena).

**Consejo:** si el efecto "cambia las reglas de la escena" (puente de hielo, apagón en el distrito) – es un Gran poder.

### 4.2. Consecuencias del fracaso del poder

El fracaso debe ser concreto e inmediato:
- pérdida de <span class="rpg-token token-power">PM</span> (siempre),
- sobrecarga (pérdida de posición, exposición),
- rastro (digital/astral),
- efecto secundario en el entorno (ruido, destello, olor, eco).

**Ejemplo:** Hack en 'vivo' durante un combate. Fracaso: se pierde <span class="rpg-token token-power">PM</span> y el sistema registra al intruso, activándose el contador de 'contra-ICE'.

### 4.3. Defensa contra el poder

Si la ficción lo justifica, permite una "contra-prueba":
- **Destreza** (esquivar, reflejos) o
- **Poder** (resistencia, contra-ritual, barrera).

La contra-prueba no debe multiplicar las tiradas. Úsala donde haga la escena más interesante (por ejemplo, parálisis, control mental).



---

### 5.1. Construye escenas en 5 pasos

1) **Objetivo de la escena:** qué debe lograr el grupo (específico).  
2) **Obstáculos:** 2-3 tipos diferentes (personas, dispositivos, entorno).  
3) **Amenaza:** enemigos, riesgos, trampas, presión del tiempo.  
4) **Contador (opcional):** 3-5 casillas; los fracasos mueven el contador; al final ocurre un gran efecto.  
5) **Recompensa y consecuencias:** qué cambia con el éxito, qué cambia con el fracaso.

Este es el "motor de escena" mínimo: funciona en fantasía, ciencia ficción y género policial.

### 5.2. Contadores (clocks) – versión simple

El contador tiene de 3 a 5 espacios. Se llena cuando:
- la prueba termina en fracaso,
- alguien hace ruido,
- los enemigos tienen tiempo para reaccionar.

Cuando el contador se llena, se produce un efecto:
- alarma,
- refuerzos,
- cierre del camino,
- pérdida de un recurso,
- escalada del conflicto.

**Ejemplo:** "Alarma 0/4". Un fallo en sigilo = +1. Éxito excepcional = -1 (opcionalmente).
Cuando llegue a 4/4, aparece una patrulla y las puertas se aseguran.

### 5.3. Cómo determinar la "dificultad de la escena" sin hacer todos los cálculos

Para un grupo de 3–5 héroes:

- **Fácil:** 3–5 secuaces o una élite sin ventajas de terreno.  
- **Estándar:** 6–8 secuaces o una élite + 2–4 secuaces, o peligro ambiental.  
- **Difícil:** jefe + 2–4 secuaces, o 2 élites + 3–5 secuaces, o cuenta regresiva 3.  
- **Heroico:** jefe + apoyo + presión ambiental + cuenta regresiva 3–5.

**Lo más importante:** el terreno y las coberturas a menudo importan más que el número de enemigos.



---

### 6.1. Sigilo e infiltración: "Alarma"

1) Establece el contador de **Alarma 0/3 a 0/5**. 
2) Cada fallo = +1 alarma. 
3) Los jugadores pueden reducir la alarma con acciones (por ejemplo, señal falsa, sabotaje) – estas son pruebas normales. 
4) Al alcanzar el máximo entra en efecto: patrulla, bloqueo, cierre total.

**Ejemplo:** El equipo avanza por el pasillo. Un especialista quiere esquivar las cámaras (<span class="rpg-token token-stat">M</span>, D 5). Fallo = +1 alarma. 
Antes de lanzar, sabe lo que arriesga, y eso es clave.

### 6.2. Persecución: "Distancia de la persecución"

Establece la **Distancia** en pasos, por ejemplo, **3** (promedio).  
Cada "turno de persecución":
- el que huye realiza una prueba (<span class="rpg-token token-stat">Z</span> o <span class="rpg-token token-stat">M</span> dependiendo del método),
- el perseguidor realiza una prueba,
- el éxito del que huye aumenta la distancia, el éxito del perseguidor la disminuye,
- cuando la distancia se reduce a **0** – el perseguidor alcanza,
- cuando aumenta a **5** – el que huye escapa.

Agrega obstáculos (giro, multitud, barricada) como descripción + modificador de dados.

### 6.3. Investigación: "Pistas en lugar de muro de pruebas"

Regla: **una pista clave no puede quedar atrapada en una sola prueba**. 
Si la escena de investigación debe continuar, la pista clave está disponible:

- automáticamente (si los jugadores hicieron algo sensato),
- o tras una prueba, pero el fracaso la entrega "con un coste" (tiempo, pista falsa, alarma).

**Ejemplo:** Examinando el cuerpo. Éxito: obtienen la verdad. Fracaso: obtienen la verdad, pero llega la guardia o alguien los nota.

### 6.4. Conflicto social: apuesta, presión, consecuencia

No conviertas la conversación en una 'lucha de tiradas'. Establece:
- qué quiere el PNJ,
- qué quieren los jugadores,
- cuál es la apuesta,
- cuántos 'movimientos' hay hasta el clímax (contador de 3 a 5).

Las pruebas **<span class="rpg-token token-stat">M</span>** (influencia, farol, autoridad) o **<span class="rpg-token token-stat">Z</span>** (leer intenciones) cambian la posición de la conversación.  
El fracaso conlleva un coste (mala impresión, pérdida de recurso, tiempo, hostilidad).



---

### 7.1. Complicaciones en caso de fracaso (lanza <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span>)

1. <span class="rpg-token token-stat">P</span>érdida de tiempo / alguien tuvo tiempo de reaccionar.
2. Revelación de la posición / aumento de la alarma.
3. Daño menor: -1 Corazón o pérdida de un recurso.
4. Mala posición: empujón, caída, exposición.
5. <span class="rpg-token token-stat">P</span>érdida o daño del equipo.
6. Aparece una nueva amenaza en la escena.

### 7.2. Beneficios del éxito excepcional (lanza <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span>)

1. <span class="rpg-token token-stat">M</span>ás rápido (ahorras tiempo o movimiento). 
2. <span class="rpg-token token-stat">M</span>ás silencioso (sin aumento de alarma). 
3. Sin coste (p.ej., sin gastar <span class="rpg-token token-power">PM</span> / sin consecuencias del terreno). 
4. Mayor efecto (mayor alcance, objetivo adicional). 
5. Mejor posición para un aliado (alguien recibe mejora de dados en la siguiente acción). 
6. Pista adicional o ventaja narrativa.

### 7.3. Entrada rápida del oponente (formato para notas)

> **Nombre — Defensa, Corazones, Táctica, Truco/Ventaja**

- **Peón:** Defensa 4–5, 1 golpe = desaparece.
- **Élite:** Defensa 6, 2 Corazones, una ventaja (movilidad/contra/cobertura).
- **Jefe:** Defensa 8 (o 12), 3 Corazones, 1–2 movimientos de jefe.

**Ejemplo (universal):**
> **Guardia — Defensa 5, 1 golpe, mantiene el pasillo, granada de humo (una vez)**



---

### 8) Seguridad y acuerdo en la mesa (mínimo)

Establezcan qué temas no van a jugar (tabúes) y qué se debe "saltar".,Acuerden una señal sencilla para interrumpir una escena (por ejemplo, "stop" o "pausa").,Resuelvan los conflictos en la mesa con una conversación fuera de la ficción, no con "decisiones con enojo".,Esto mejora la calidad del juego más que cualquier mecánica.



---

### 9) Modularidad y desarrollo por la comunidad: cómo mantenerlo bajo control

Si estás construyendo NDE como un "motor", la comunidad encontrará más fácil desarrollarlo a través de paquetes:

- **Paquete de género** (fantasía/cyberpunk/horror): mapeo de Poderes, lista de ventajas, equipo, enemigos, 1-2 procedimientos (por ejemplo, miedo, persecución).  
- **Paquete de enemigos:** 10-20 entradas de secuaz/élite/jefe + tácticas.  
- **Paquete de aventuras:** escenas de 1 página con contadores y apuestas.

**Requisito de calidad para las contribuciones:** cada nueva regla debe tener:
- una frase "para qué es esto" (qué problema resuelve),
- una breve descripción de la regla,
- un ejemplo de 3 a 5 líneas.

De esta manera, los complementos no desestabilizarán el núcleo y serán comprensibles para los nuevos.

