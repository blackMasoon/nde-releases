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
generated_at: "2026-01-16T08:50:46.500Z"
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
# Manual de Monstruos

Automatic translation placeholder for es

---



---

### ¿Para qué es este libro?

Este libro es un conjunto de **herramientas** para crear oponentes y amenazas en NDE:
- rápidamente (en 2–5 minutos),
- sin calcular coeficientes,
- de manera coherente con las reglas de **Basic Rules** y **Libro del DM**.

**El supuesto más importante de NDE:** *solo los jugadores lanzan dados.*
Los oponentes no "atacan tirando" — atacan **con presión en la ficción**: ponen obstáculos, fuerzan pruebas, crean amenazas y consecuencias.



---

### 0. Glosario (términos en este libro)

- **Defensa**: umbral de golpe/esquivar del oponente en combate. El jugador tira y compara el resultado con la Defensa.
- **Dificultad (D)**: umbral de prueba contra el entorno, fenómeno, movimiento especial o "truco" del enemigo.
- **Corazones**: cuántos daños puede soportar un ser en esta escena.
- **Peón / Élite / Jefe**: tres niveles de "importancia" del oponente en la escena.
- **Facilidad / Dificultad**: cambio en el tamaño del dado del jugador en 1 grado (**<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>** / hacia abajo).
- **Movimiento especial**: habilidad activa del enemigo que cambia la situación (a menudo obliga a una prueba de F/A/<span class="rpg-token token-stat">M</span> del jugador).
- **Rasgo (pasivo)**: propiedad permanente del enemigo (armadura, vuelo, resistencia, zona de peligro), que usualmente proporciona facilidad/dificultad o cambia la apuesta.



---

### 1. Cómo actúa el oponente en NDE (en resumen)

En NDE el oponente es simple, pero "vivo" gracias a su comportamiento.

1) **El jugador actúa → el jugador lanza los dados.**  
   - Ataque cuerpo a cuerpo: Fuerza (F) vs **Defensa** del objetivo.  
   - Ataque a distancia: Destreza (D) vs **Defensa** del objetivo.  
   - Poderes: Poder (<span class="rpg-token token-stat">P</span>) vs **Dificultad (D)** o vs Defensa (si es un ataque/neutralización).

2) **Si el jugador falla / pierde la prueba**, la escena continúa: aparece un coste o complicación.  
   En combate, el coste puede significar:  
   - pérdida de posición,  
   - pérdida de tiempo,  
   - entrar en el rango de una zona peligrosa,  
   - o **Corazón perdido**, si tiene sentido (por ejemplo, combate cuerpo a cuerpo, fuego cruzado, área de efecto).

3) **El oponente "actúa" sin tirar:**  
   El MG describe lo que hace el enemigo y, si realmente amenaza a los héroes, entonces:  
   - impone una prueba (F/D/<span class="rpg-token token-stat">P</span>) contra **Dificultad (D)**,  
   - o establece una condición ("hasta que no...", "cuando entres en...", "quien esté Cerca..."),  
   - o cambia los dados de los jugadores (facilitación/dificultad).

4) **El combate es comprensible cuando el enemigo tiene una táctica de una frase.**  
   Cada ficha de personaje debe contener: "qué hace este enemigo en la primera ronda" y "qué hace cuando recibe un golpe en la cara".



---

### 2. Bloque de estadísticas — formato y campos

El bloque de estadísticas mínimo tiene solo lo que se necesita en la escena.

> **Nombre — Clase, Defensa, Corazones, Rol, Movilidad, Habilidades, Movimientos, Táctica**

### 2.1 Campos obligatorios

- **Clase:** Peón | Élite | Jefe  
- **Defensa:** número que se debe superar para golpear/esquivar al enemigo.  
- **Corazones:** cuántos impactos puede soportar (en NDE 'impacto' equivale estándarmente a 1 Corazón).  
- **Rol:** qué presión crea en combate (ver capítulo 4).  
- **Movilidad:** cómo se mueve (descripción por zonas; la cuadrícula es opcional).  
- **Habilidades (pasivas):** 1–2 características breves.  
- **Movimientos (activos):** 1 movimiento (Élite) o 2–3 movimientos (Jefe).  
- **Táctica:** 1–3 oraciones para que el DM guíe consistentemente al enemigo.

### 2.2 Campos opcionales (bueno tener, si se ajustan)

- **Alcance:** si el enemigo es a distancia (ej. "Lejos", "Muy lejos").  
- **Zona:** si el enemigo crea un área peligrosa (humo, fuego, campo de fuerza).  
- **Debilidad:** una "palanca" clara para los jugadores (agua, luz UV, interferencia de señal).  
- **Recompensa / Pista:** lo que queda después de derrotar al enemigo (botín, rastro, información).  
- **Variantes:** 1-2 intercambios rápidos (ej. "en lugar de volar, puede saltar"; "en lugar de fuego, tiene ácido").

### 2.3 Ejemplo de bloque de estadísticas (universal)

**Guardia — Esbirro, Defensa 5, Corazones 1, Bruto, Movilidad: Cercano→Próximo, Habilidades: Escudo, Movimientos: Empuje, Táctica: bloquea el paso y empuja fuera de la cobertura.**

- **Escudo (pasivo):** mientras esté **Próximo** a una cobertura o un escudero, quien ataca tiene **desventaja** (el dado desciende 1 grado).
- **Empuje (movimiento):** si el Guardia acierta en combate cuerpo a cuerpo (o si el jugador falla un ataque cuerpo a cuerpo contra él), el MJ puede empujar al personaje 1 zona (Próximo→Cercano) o 1–2 casillas en la variante de cuadrícula.
- **Táctica:** entra en combate cuerpo a cuerpo con el objetivo más débil, defiende el pasillo, no huye.



---

### 3. Clases de enemigos: Esbirro, Élite, Jefe

En NDE, la "dificultad" de un enemigo se compone de dos cosas:
- **qué tan difícil es alcanzarlo** (Defensa),
- **cuánto puede resistir** (Corazones),
- y **qué presión ejerce** (rol + movimientos).

### 3.1 Secuaz (esbirro)

- **Defensa:** normalmente **5** (más fácil: 4, más difícil: 6).
- **Corazones:** **1** (cae al ser golpeado).
- **Movimientos:** por lo general 0–1 (simple, predecible).
- **Propósito:** proporciona ritmo, contexto y sensación de "lucha con el grupo".
- **Cómo manejarlos:** aparecen en grupos de 3–8, caen rápidamente, pero hacen ruido y ocupan espacio.

> Buena regla: el esbirro tiene sobre todo *posición* (cobertura, ventaja numérica, terreno elevado), y no una "mecánica compleja".

### 3.2 La élite

- **Defensa:** generalmente **6** (élite fácil: 5, "élite dura": 8). 
- **Corazones:** **2**.
- **Movimientos:** 1 movimiento característico + 1 cualidad pasiva.
- **Propósito:** actúa como un "mini-jefe" en una escena, obligando a la adaptación.

> La élite debe hacer *una cosa claramente*: "rompe defensas", "crea zonas", "salta por las paredes", "cura a los secuaces".

### 3.3 Jefe

- **Defensa:** usualmente **8** (legendario: 12). 
- **Corazones:** **3** (final: 5). 
- **Movimientos:** 2–3 movimientos + 1–2 características pasivas. 
- **Para qué sirve:** es una escena en sí misma — afecta al terreno y al ritmo.

**Un jefe sin trucos es aburrido.** Para que un jefe sea "jugable", dale al menos uno de los siguientes:
- un movimiento que requiere una prueba a varios héroes,
- una zona (terreno que se debe manejar),
- o una mecánica de "fase" (al perder 1 Corazón cambia su comportamiento).

### 3.4 "Legendario" (nivel opcional)

Si necesitas un oponente de campaña:
- **Defensa 12**, **Corazones 5**, 3-4 movimientos, zonas y fases.
Este es el "jefe para el final del acto" — no lo pongas de manera aleatoria.



---

### 4. Roles de los oponentes (presión clara)

Las funciones están para que el Maestro de Juego sepa de inmediato "cómo jugar con esto". Una función no es una estadística, es un **estilo de amenaza**.

- **Bruto (embate cuerpo a cuerpo):** se aproxima de Cerca, empuja, derriba, rompe el frente.  
  *Pregunta para los jugadores:* "¿quién está al frente y qué arriesga?"

- **Hostigador (móvil):** entra, hace lo suyo y huye; castiga la soledad.  
  *Pregunta:* "¿quién está separado del grupo?"

- **Artillería (distancia):** dispara desde las coberturas; obliga a moverse y cambiar de posición.  
  *Pregunta:* "¿dónde es seguro y dónde está la línea de fuego?"

- **Controlador (control):** áreas, humo, terreno pegajoso, trampas, presión sobre los objetivos.  
  *Pregunta:* "¿cómo evitar la zona en lugar de luchar en ella?"

- **Apoyo:** fortalece, sana, mueve, proporciona coberturas.  
  *Pregunta:* "¿a quién eliminar primero para simplificar la pelea?"




---

### 5. Facilidades/dificultades en los monstruos — regla de dirección

En NDE **no complicamos los números**.  
En lugar de: '+2 para acertar, -1 al daño, bonificación a AC' — hacemos:

- **facilidad:** sube el dado del jugador 1 grado,
- **dificultad:** baja el dado del jugador 1 grado,
- **cambio de enfoque:** el éxito funciona, pero requiere un enfoque diferente (por ejemplo, primero eliminar la cobertura).

### 5.1 Cuando cambiar la Defensa y cuando el dado

- **Cambia más a menudo el dado del jugador** (facilitar/dificultar).
- **Cambia la Defensa raramente**, principalmente cuando:
  - el enemigo tiene "armadura/invisibilidad/campo de fuerza" que *realmente* lo hace más difícil de acertar,
  - o cuando es una mecánica de fase de jefe.

### 5.2 Ejemplos de desventajas "puras"

- "El enemigo está parcialmente cubierto" → el atacante tiene **desventaja**.  
- "El enemigo está aturdido / atado" → el atacante tiene **ventaja**.  
- "El enemigo es rápido y salta por las paredes" → el atacante tiene **desventaja** hasta que lo bloqueen.



---

### 6. Habilidades Pasivas (Características) — Catálogo para Anexar

A continuación tienes características que puedes añadir al bloque de estadísticas. 
Elige **1-2** (jefe: 2-3). Siempre descríbelas en el mundo del juego.

### 6.1 Protección y dureza

- **Armadura Ligera:** el primer golpe en esta escena inflige 1 Corazón menos (o sea, 0) *o* requiere "especificación" (el éxito inflige Corazón solo cuando el ataque bordea la armadura).  
  *Versión más sencilla:* "el primer golpe no inflige Corazón".

- **Armadura Pesada:** mientras no se evite la armadura (flanqueo, explosión, gancho, magia), los ataques tienen **desventaja**.  
  *Nota:* brinda a los jugadores un camino claro para sortearla.

- **Duro:** tras perder 1 Corazón el enemigo no cambia de posición (no se puede empujar/tumbar fácilmente).  
  Bueno para colosos y jefes.

### 6.2 Movilidad

- **Rápido:** una vez por ronda puede cambiar la distancia a una zona adicional (ej. Lejos→Cerca). En la cuadrícula: +1-2 casillas.,- **Saltador / Escalador:** trata los obstáculos verticales como normales. Ofrece accesos cortos razonables a la retaguardia.,- **Vuelo:** ignora los obstáculos del terreno, pero requiere coberturas "desde arriba" o fuerza pruebas de reacción (ej. <span class="rpg-token token-stat">Z</span>, para evitar un bombardeo).

### 6.3 Percepción y sigilo

- **Explorador:** el primer intento de acercarse a él por sorpresa tiene una **dificultad**.
- **Centinelas:** si alguien realiza una acción ruidosa en la escena, el enemigo inmediatamente cambia de posición a una mejor (se pone a cubierto / llama a refuerzos).

### 6.4 Resistencias y debilidades (sencillo)

- **Resistencia [tipo]:** la primera vez en una escena que el enemigo debería recibir un efecto dado (fuego, hielo, psíquico, electricidad), el efecto es **más débil** (área más pequeña / duración más corta / sin pérdida de Corazón).  
- **Debilidad [tipo]:** contra este tipo de ataques, el jugador tiene **facilidades**.

> Principio de transparencia: la resistencia y la debilidad solo tienen sentido si los jugadores pueden descubrirlas y usarlas.

### 6.5 "Enjambre" y presión numérica

- **Enjambre:** si al menos dos de estas criaturas están Cerca de un héroe, el héroe tiene **desventaja** en las pruebas de movimiento/escape hasta que cambie de zona.



---

### 7. Movimientos activos: cómo escribirlos y cómo dirigirlos

Un movimiento activo debe responder a 3 preguntas:
1) **¿Qué hace en la ficción?** (descripción)
2) **¿A quién afecta y cuándo?** (disparador)
3) **¿Cómo se resuelve mecánicamente?** (prueba / efecto / costo)

### 7.1 Formato simple de movimiento

- **Nombre del movimiento:** una sola frase de descripción. - **Desencadenante:** cuándo ocurre esto (por ejemplo, "cuando el héroe está cerca", "cuando alguien dispara desde la cubierta"). - **Prueba:** qué atributo y qué dificultad. - **Consecuencia de fracaso:** lo que pierdes, lo que cambia. - **Consecuencia de éxito:** usualmente evitas la consecuencia o ganas una ventaja.

### 7.2 Cómo determinar la Dificultad del movimiento enemigo (sin tablas)

Si el movimiento es "ofensivo" y se dirige a un único objetivo:
- establece **T movimiento = Defensa del enemigo** (esto es coherente y fácil de recordar).

Si el movimiento es de área o "grande":
- establece T un nivel más alto que el estándar de la escena (usualmente **T 6** o **T 8**).

### 7.3 Movimientos de ejemplo (módulos)

**Empuje (Brute)**  
- **Descripción:** el enemigo entra en combate cuerpo a cuerpo y empuja.  
- **Desencadenante:** cuando el enemigo está Cerca del héroe.  
- **Prueba:** el héroe realiza una prueba de **F o A** contra **D = Defensa del enemigo**.  
- **Fracaso:** el héroe pierde 1 Corazón *o* es empujado 1 zona (el GM elige lo que tiene sentido).  
- **Éxito:** evitas el daño y mantienes la posición.

**Salva (Artillery)**  
- **Descripción:** una serie de disparos / fragmentos en un área.  
- **Desencadenante:** cuando al menos 2 héroes están en la misma zona y no están cubiertos.  
- **Prueba:** cada objetivo prueba **A** contra **D 6** (o D = Defensa del enemigo, si el enemigo es élite).  
- **Fracaso:** −1 Corazón y "debes moverte" (Cerca→Lejos).  
- **Éxito:** te escondes / no recibes daño.

**Ancla (Controller)**  
- **Descripción:** terreno pegajoso, campo de fuerza, telaraña, hielo.  
- **Desencadenante:** el enemigo tiene un momento para establecer la zona.  
- **Prueba:** cuando entras en la zona, pruebas **A o <span class="rpg-token token-stat">M</span>** contra **D 5–6**.  
- **Fracaso:** pierdes el movimiento en este turno y estás "en mala posición" (desventaja en ataques).  
- **Éxito:** pasas o neutralizas la zona.

**Refuerzo (Support)**  
- **Descripción:** el enemigo cubre a un aliado / cura / da ventaja.  
- **Desencadenante:** una vez por ronda, cuando un aliado está en peligro.  
- **Efecto:** el aliado elegido obtiene "escudo" — los atacantes tienen **desventaja** hasta el final de la ronda, o el aliado recupera 1 Corazón (jefe/élite).  
- **Contra de jugadores:** neutraliza el soporte o fuerza una elección (a quién salvar).



---

### 8.1 Por defecto: zonas de distancia

En un combate descriptivo, usa: **Cerca / No muy lejos / Lejos / Muy lejos**.

En la hoja de estadísticas, registra la movilidad como:
- "**Movilidad:** cambia de zona en 1 (estándar)"
- o "**Movilidad:** Rápido (cambia de zona en 2)"
- o "**Movilidad:** Vuela (ignora obstáculos, pero requiere pruebas en ataques aéreos)".

### 8.2 Opción: cuadrícula (si a la mesa le gusta la táctica)

Si juegas en un mapa:
- movimiento estándar = **5 casillas**,
- Rápido = **6-7**,
- Salto = 3 casillas "en vertical" o sobre obstáculos.

**Todas las habilidades descriptivas funcionan igual** — la cuadrícula solo "proporciona una referencia métrica".



---

### 9. Construcción de un oponente en 2 minutos (procedimiento)

1) **Elige una clase**: Esbirro / Élite / Jefe.
2) **Establece Defensa**: 5 / 6 / 8 (legendario: 12).
3) **Establece Corazones**: 1 / 2 / 3 (final: 5).
4) **Elige un rol**: Bruto / Asaltante / Artillería / Controlador / Apoyo.
5) **Añade 1-2 características pasivas** (jefe: 2-3).
6) **Añade movimientos**: Élite 1, Jefe 2-3.
7) **Escribe una táctica en 2 oraciones** (primera ronda + reacción a amenaza).
8) (Opcional) Añade una **debilidad** y **recompensa**.

> Prueba práctica: si puedes dirigir al enemigo sin mirar la tabla, el bloque de estadísticas es bueno.



---

### 10. Plantillas listas (para reskin en cualquier mundo)

Las siguientes entradas están deliberadamente 'sin color'. Cambias el nombre y la descripción, la mecánica se mantiene.

### 10.1 Esbirros

- **Guardia — Esbirro, Defensa 5, Corazones 1, Bruto, Movilidad: estándar, Habilidades: Escudo, Movimientos: Empuje, Táctica: bloquea y empuja.**
- **Explorador — Esbirro, Defensa 5, Corazones 1, Escaramuzador, Movilidad: Rápida, Habilidades: Explorador, Movimientos: Escape, Táctica: se acerca, marca objetivos y desaparece.**
- **Tirador — Esbirro, Defensa 5, Corazones 1, Artillería, Movilidad: estándar, Habilidades: Cobertura, Movimientos: Bombardeo, Táctica: mantiene la Distancia y obliga a correr.**
- **Controlador — Esbirro, Defensa 5, Corazones 1, Controlador, Movilidad: estándar, Habilidades: Zona, Movimientos: Ancla, Táctica: divide al equipo.**
- **Apoyo — Esbirro, Defensa 5, Corazones 1, Apoyo, Movilidad: estándar, Habilidades: <span class="rpg-token token-stat">M</span>édico, Movimientos: Refuerzo, Táctica: protege a la élite.**

**Movimientos rápidos para esbirros:**
- **Escape:** cuando es golpeado (pero aún "no cae" en la ficción, por ejemplo, armadura), se aleja 1 zona.
- **Bombardeo:** si alguien está al descubierto, le da una desventaja en su próxima acción ("balas, esquirlas, miedo").
- **Zona:** una vez por escena coloca una pequeña zona de desventaja (humo, aceite, barro).

### 10.2 Élites

- **Duros — Élite, Defensa 6, Corazones 2, Bruto, Movilidad: estándar, Habilidades: Armadura Ligera, Movimientos: Embestida, Táctica: se acerca y mantiene la línea.**
- **Asesino — Élite, Defensa 6, Corazones 2, Skirmisher, Movilidad: Rápido + Saltador, Habilidades: Explorador, Movimientos: Corte de flanco, Táctica: golpea desde atrás y se retira.**
- **Francotirador — Élite, Defensa 6, Corazones 2, Artillería, Movilidad: Distante, Habilidades: Cobertura, Movimientos: Tiro selectivo, Táctica: fuerza el movimiento y castiga la falta de cobertura.**
- **Manipulador del Terreno — Élite, Defensa 6, Corazones 2, Controlador, Movilidad: estándar, Habilidades: Zona (2×), Movimientos: Ancla, Táctica: corta la ruta de escape.**
- **Comandante — Élite, Defensa 6, Corazones 2, Apoyo, Movilidad: estándar, Habilidades: Centinelas, Movimientos: Refuerzo, Táctica: refuerza a los aliados y los coloca bajo cobertura.**

### 10.3 Jefes

- **Líder — Jefe, Defensa 8, Corazones 3, Soporte, Movilidad: estándar, Habilidades: Vigilante + Escudo, Movimientos: Reforzar + Invocar + Barrera, Táctica: mantiene el apoyo y controla el ritmo.**
- **Coloso — Jefe, Defensa 8, Corazones 3, Bruto, Movilidad: estándar, Habilidades: Resistente + Armadura Pesada, Movimientos: Sacudir + Embate, Táctica: rompe la formación y fuerza pruebas.**
- **Cazador — Jefe, Defensa 8, Corazones 3, Hostigador, Movilidad: Rápido + Saltador, Habilidades: Explorador, Movimientos: Emboscada + Corte + Escape, Táctica: aísla y elimina.**
- **Arquitecto de Zonas — Jefe, Defensa 8, Corazones 3, Controlador, Movilidad: estándar, Habilidades: Zona (2×) + Resistencia [tipo], Movimientos: Anclar + Salva + Desplazar, Táctica: divide al equipo y fuerza decisiones.**



---

### 11. Amenazas Ambientales (Peligros)

Un peligro es un "oponente sin voluntad" o un mecanismo de escena: torreta, fuego, avalancha, alarma.

**Formato: Nombre — Dificultad (T), Cuándo actúa, Efecto, Cómo desactivarlo / evitarlo**

### 11.1 Ejemplos de peligros (universales)

**Torreta / Dron de defensa — T 6**  
- **Cuándo actúa:** al final de la ronda, si alguien está en la línea de visión.  
- **Efecto:** prueba **<span class="rpg-token token-stat">Z</span> vs T 6**; fracaso: −1 Corazón y debes buscar cobertura.  
- **Desactivación:** prueba **<span class="rpg-token token-stat">M</span> o <span class="rpg-token token-stat">Z</span> vs T 6** en el panel / interferencia / corte de energía.

**Trampa / Mina / Cepo — T 5**  
- **Cuándo actúa:** cuando entras en la zona.  
- **Efecto:** prueba **<span class="rpg-token token-stat">Z</span> vs T 5**; fracaso: −1 Corazón o inmovilización (pierdes movimiento).  
- **Desactivación:** herramientas + prueba **<span class="rpg-token token-stat">Z</span> vs T 4–5**.

**Gas / Humo / Contaminación — T 5**  
- **Cuándo actúa:** al inicio del turno, si estás en la zona.  
- **Efecto:** prueba **<span class="rpg-token token-stat">S</span> o <span class="rpg-token token-stat">M</span> vs T 5**; fracaso: −1 Corazón o desventaja en pruebas para salir.  
- **Desactivación:** ventilación, máscaras, sellado.

**Alarma / Temporizador — T (dependiendo de la escena)**  
- **Cuándo actúa:** cuando ocurre una complicación o alguien hace ruido.  
- **Efecto:** aparece una presión de tiempo (próxima ola, cierre de puertas, refuerzos).  
- **Desactivación:** prueba **<span class="rpg-token token-stat">M</span>** (hackeo/ritual) o "físicamente" prueba **<span class="rpg-token token-stat">S</span>/<span class="rpg-token token-stat">Z</span>**.



---

### 12. Generador de escena de combate (rápido, claro)

Elige 1 de cada línea (o lanza <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span>):

1) **Objetivo de la escena:** pasar / recuperar / desactivar / escoltar / robar / defender  
2) **Terreno:** abierto / cuellos de botella / varios niveles / muchas coberturas / bordes / niebla-humo  
3) **Oponentes:** 6× secuaces / 4× secuaces + élite / 2× élite / jefe / jefe + 2× secuaces / élite + riesgo  
4) **Ventaja del enemigo:** cobertura / altura / movilidad / contador de tiempo / emboscada / apoyo a distancia  
5) **Ventaja de los jugadores:** sorpresa / herramientas / atajo / aliado neutral / el terreno ofrece cobertura / información (saben quién es el enemigo)



---

### 13. Equilibrio en la práctica (sin matemáticas)

En NDE, el equilibrio se consigue con *ritmo* y *presión*, no con 'CR'.

### 13.1 Reglas Rápidas para Establecer la Dificultad de la Escena

- **Escena Fácil:** 4-6 esbirros o 1 élite.  
- **Escena Estándar:** 4 esbirros + 1 élite, o 2 élites.  
- **Escena Difícil:** jefe + 2-4 esbirros, o jefe + peligro.  
- **Final:** jefe (Corazones 5) + élite + presión del tiempo.

### 13.2 Si la batalla resulta demasiado corta

- Lanza **una oleada de esbirros** (2–3 por ronda durante 2 rondas). 
- Aumenta la presión del terreno: zona de humo, alarma, falta de cobertura. 
- Cambia de táctica: el enemigo deja de pelear "honestamente" (se retira, toma un rehén, bloquea la salida).

### 13.3 Si la pelea se prolonga

- Dale a los jugadores una "palanca": un tanque expuesto, un panel, un ritual, una debilidad.
- Permite **beneficios por un éxito excepcional**: romper la cobertura, desarmar, dispersar el apoyo.
- Reduce los Corazones del jefe de 5 a 3 si no es el final.



---

### 14. Reskins: cómo adaptar un enemigo para cada ambientación

Tienes un bloque de estadísticas para un "Explorador". Ahora solo cambias la descripción:

- **Fantasía:** arquero explorador goblin (Explorador + Disparo).  
- **Ciencia ficción:** dron de reconocimiento (Explorador + Sensores).  
- **Cyberpunk:** explorador de pandillas en patineta (Rápido + Escape).  
- **Esclavo:** demonio que sigue rastros (Debilidad: hierro; Resistencia: miedo).

La mecánica sigue siendo la misma. Esto permite a la comunidad agregar cientos de entradas sin romper la coherencia del núcleo.

