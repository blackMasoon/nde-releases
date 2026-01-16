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
generated_at: "2026-01-16T10:17:16.406Z"
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
# Manual del Jugador

Automatic translation placeholder for es

---



---

### 1) Cómo es el juego en la mesa

- **El Director de Juego (DJ)** describe la situación y dice qué es posible en esta escena.
- **Tú** dices: **qué haces** y **qué efecto deseas**.
- Si el resultado es incierto o arriesgado, el DJ dice:
  1) **qué atributo** usas (F/D/<span class="rpg-token token-stat">P</span>),
  2) **cuál es la Dificultad** <span class="rpg-token token-t">T</span> (o **Defensa** del objetivo),
  3) **qué amenaza en caso de fracaso** (consecuencia).

Luego lanzas el dado del atributo y de inmediato saben qué sucede a continuación.

### La regla más corta

**Lanza el dado de característica. Resultado ≥ <span class="rpg-token token-t">T</span> = éxito.**



---

### 2) Qué tiene tu personaje

Tu personaje tiene:
- **Concepto** (1 oración: quién eres, en qué mundo actúas),
- **Rol** (Asalto / Especialista / Adepto),
- 3 **atributos**: Fuerza (F), Destreza (D), Poder (<span class="rpg-token token-stat">P</span>),
- **Corazones** (resistencia) y **Puntos de Poder** (PP),
- **Giro de Suerte** (GS),
- (opcionalmente) **Talentos**,
- **equipo**.

### 2.1 Características (<span class="rpg-token token-stat">S</span>/<span class="rpg-token token-stat">Z</span>/<span class="rpg-token token-stat">M</span>) — para qué son

- **Fuerza (<span class="rpg-token token-stat">S</span>)**: combate cuerpo a cuerpo, forzar, cargar, resistencia. - **Destreza (<span class="rpg-token token-stat">Z</span>)**: disparar, precisión, sigilo, esquivar, acrobacias, conducción de vehículos. - **Poder (<span class="rpg-token token-stat">M</span>)**: "efectos especiales" del mundo del juego: magia, psiónica, fe, supertecnología, hacking, influencia, intuición — dependiendo de la convención.

### 2.2 Dados de características — cómo funcionan

Cada característica tiene un dado: <span class="rpg-token token-<span class="rpg-token token-d4">k4</span>"><span class="rpg-token token-d4">k4</span></span>, <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>, <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>, <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span> o <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>.
Cuando usas una característica, lanzas **un dado** de esa característica.

- Dado más grande = mayor probabilidad de éxito y de éxito excepcional (máx en el dado).

**Ejemplo:** Tienes Destreza <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>. Cuando disparas, escalas o te deslizas, normalmente lanzas <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>.

### 2.3 Recursos: Corazones, Puntos de Poder y Golpe de Suerte

- **Corazones:** 5 al inicio. Los golpes y la presión quitan Corazones.
- **Puntos de Poder (PP):** 3 al inicio. Los usas para poderes y movimientos más allá del estándar.
- **Golpe de Suerte (GS):** 2 al inicio de cada sesión. Es tu "salvar escenas" y aumentar la dramaturgia.




---

### Paso 1: Concepto y rol

Elige un rol: este es el estilo de actuación general (se adapta a cualquier universo).

- **Asalto**: te arriesgas y empujas las escenas hacia adelante.  
  (ej. guerrero, marines, guardaespaldas, cazador, bárbaro)
- **Especialista**: actúas con precisión, con un plan y herramientas.  
  (ej. pícaro, francotirador, explorador, hacker, piloto, rastreador)
- **Adept**: haces cosas "más allá del estándar" - con poder, conocimiento, influencia.  
  (ej. mago, psiónico, sacerdote, alquimista, tecnomante, diplomático)

### Paso 2: Distribuir los dados de características

Distribuir los dados: una característica <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>, una <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>, una <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>.

Consejos rápidos:
- **Asalto** normalmente tiene <span class="rpg-token token-stat">S</span> más alto.
- **Especialista** normalmente tiene <span class="rpg-token token-stat">Z</span> más alto.
- **Experto** normalmente tiene <span class="rpg-token token-stat">M</span> más alto.

### Paso 3: Guarda los recursos

- **Corazones:** 5  
- **Puntos de Poder:** 3  
- **Suerte:** 2 (se actualiza al comienzo de la sesión)

### Paso 4 (opcional): Elige 2 Talentos

Los talentos son frases cortas que describen en qué eres bueno (competencias que a menudo regresan en el juego). - Ejemplos: "Explorador", "Mecánico", "<span class="rpg-token token-stat">M</span>édico", "Negociador", "Atleta", "Analista", "Hacker", "Ritualista".

**Cómo funcionan los Talentos:** si un Talento realmente ayuda en una prueba, el DM lo trata como una situación mejor y puedes **mejorar el dado en 1 grado** para esa tirada. - Normalmente 1 Talento por 1 prueba. - Un Talento no reemplaza la descripción de la acción – debe fortalecer un plan sensato.

**Ejemplo:** Tienes el Talento "Mecánico" e intentas poner en marcha de emergencia un generador. El DM decide que esto ayuda: mejoras el <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span> a <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span> para esta prueba.

### Paso 5: Equipo

Enumera:
- 1 herramienta "clave" (arma o equipo profesional),
- 1 protección (armadura, escudo, camuflaje, dependiendo del mundo),
- 3 objetos útiles.

El equipo suele funcionar como **permiso**: si tienes algo, puedes intentar las acciones correspondientes. Una buena herramienta también puede crear una mejor situación (aumentar los dados) si tiene sentido.

### Ejemplo de personaje (universal)

- Rol: Especialista  
- F <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">d6</span></span>, A <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span>, I <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span>  
- Corazones 5, <span class="rpg-token token-power">PM</span> 3, HS 2  
- Talentos: "Explorador", "Negociador"  
- Equipamiento: arma a distancia, ganzúas / kit de herramientas, cuerda, linterna



---

### 4.1 Cuando lanzas

Lanzas cuando:
- algo es **arriesgado** o incierto,
- el fracaso tiene una **consecuencia significativa**.

Si algo es obvio y sin presión, el GM puede decir “tienes éxito” sin lanzar.

### 4.2 Dificultad <span class="rpg-token token-t">T</span>

El DM elige la Dificultad:

- <span class="rpg-token token-t">T 3</span> fácil  
- <span class="rpg-token token-t">T 4</span> estándar  
- <span class="rpg-token token-t">T 5</span> difícil  
- <span class="rpg-token token-t">T 6</span> muy difícil  
- <span class="rpg-token token-t">T 8</span> heroico  
- <span class="rpg-token token-t">T 12</span> legendario

No necesitas "adivinar" la Dificultad — el DM la dice directamente.

### 4.3 Resultados del lanzamiento

- **1**: fallo con consecuencia (la complicación es segura).
- **Resultado < <span class="rpg-token token-t">T</span>**: fallo (pero la escena continúa).
- **Resultado ≥ <span class="rpg-token token-t">T</span>**: éxito.
- **<span class="rpg-token token-stat">M</span>áximo en el dado** (por ejemplo, 12 en <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>, 20 en <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>): éxito excepcional + beneficio adicional.

**Beneficio adicional** (ejemplos): más rápido, más silencioso, más seguro, mayor efecto, mejor posición, detalle adicional a tu favor.

### 4.4 Situación mejor/peor (sin bonificaciones)

En lugar de contar modificadores, juegas según la situación:

- **Situación mejor** → aumenta el dado en 1 nivel  
  (<span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>)
- **Situación peor** → reduce el dado en 1 nivel  
  (<span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d4">k4</span>"><span class="rpg-token token-d4">k4</span></span>)

Tu papel como jugador: **crea mejores condiciones** a través de la descripción y decisiones (cobertura, preparación, herramientas, plan, reconocimiento).

### 4.5 Ayuda del aliado

El aliado puede usar su Acción para ayudarte. Entonces, para ese único lanzamiento:
- subes el dado 1 grado.

La ayuda debe tener sentido en la descripción (distraer, cubrir, pasar herramientas, apoyo de fuego, un par de manos adicional).

### Ejemplo de prueba (claro y completo)

Quieres abrir una puerta bloqueada antes de que lleguen los guardias.
- MJ: "Es Destreza. <span class="rpg-token token-t">T 5</span>. Fracaso: haces ruido y pierdes tiempo."
- Tienes D <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>, pero usas ganzúas y tienes el Talento "Especialista en cerraduras" → mejor situación, subes a <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>.
- Tirada <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span> = 6 → éxito: la puerta se abre sin alarma.



---

### 5) Golpe de Suerte (GS) — cuándo vale la pena usarlo

Al comienzo de cada sesión tienes **2 GS**. GS existe para:
- salvar escenas importantes,
- añadir dramatismo,
- recompensar decisiones valientes.

Gasta **1 GS** para elegir una:
- **Repetir** tu prueba (te quedas con el mejor resultado), o
- **Aumentar el dado en 1 grado** en ese único lanzamiento, o
- **Cambiar el fallo por un "éxito con costo"** — la acción tiene éxito, pero el GM inmediatamente añade un precio.

**Recuperación de GS:** al comienzo de la siguiente sesión vuelves al límite. El GM puede otorgar **+1 GS** por riesgo valiente, una gran decisión narrativa o jugar con las consecuencias.

**Ejemplo:** Un fallo al saltar entre tejados significaría caer a la calle. Gastas 1 GS y cambias el fallo por éxito con costo: llegas al otro lado, pero pierdes el equipo o te tuerces el tobillo (una peor situación en la siguiente escena).




---

### 6.1 Distancias (predeterminadas, sin mapa)

Describe la distancia con cuatro palabras: - **Cerca** (al alcance de la mano), - **No muy lejos** (unos pocos pasos), - **Lejos** (al otro lado de la escena), - **Muy lejos** (a distancia de francotirador / vehicular).

En un turno tienes: **Desplazamiento + 1 Acción**.
Desplazarse generalmente cambia la distancia en 1 grado (No muy lejos→Cerca, etc.).

### 6.2 Opción: juego en la cuadrícula

Si juegas en un mapa:
- 1 casilla = 1–2 m,
- movimiento por turno: **hasta 5 casillas**,
- las diagonales cuentan como 1 casilla,
- el resto de las reglas funciona de manera idéntica.

### 6.3 Ataque

- **Cuerpo a cuerpo:** tirada de **Fuerza (F)** contra la **Defensa** del objetivo.  
- **A distancia:** tirada de **Destreza (D)** contra la **Defensa** del objetivo.

**Defensa de los oponentes (aproximadamente):**
- <span class="rpg-token token-t">4</span> Débil  
- <span class="rpg-token token-t">5</span> Típico  
- <span class="rpg-token token-t">6</span> Élite  
- <span class="rpg-token token-t">8</span> Jefe  
- <span class="rpg-token token-t">12</span> Jefe legendario

### 6.4 Cobertura y posición

- Objetivo en cobertura / mal ángulo / presión → peor situación (reduce el dado). 
- Buena posición / sorpresa / superioridad numérica → mejor situación (sube el dado).

### 6.5 Golpear y daño

- Un golpe inflige **1 Corazón**. - Un éxito crítico inflige **2 Corazones** o produce un efecto fuerte (desarme, derribo, empujón, eliminar cobertura).

### 6.6 0 Corazones

Cuando caes a **0 Corazones**, estás fuera de combate (herido, aturdido, en shock, según la convención).
- Un aliado puede usar una Acción para ponerte en **1 Corazón**.
- Si la presión continúa, tu prioridad es la cobertura y evacuación, no el "tanqueo".

### Ejemplo de un turno corto (sin cuadrícula)

- Estás **Cerca** de la élite.
- Movimiento: te desplazas **Cerca** detrás de la columna (cobertura).
- Acción: ataque cuerpo a cuerpo (<span class="rpg-token token-stat">S</span>). La defensa de la élite es <span class="rpg-token token-t">6</span>. Tienes <span class="rpg-token token-stat">S</span> <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>.
  Tirada 9: éxito, la élite pierde 1 Corazón.

---



---

### 7) Poderes y jugadas por encima del estándar (Puntos de Poder)

Lo que llamamos "poder" depende del mundo: hechizos, psiónica, fe, gadgets, hacking, supertrucos.

### 7.1 Cómo usas el poder

1) Describe el efecto.  
2) El GM dice la Dificultad y el costo en <span class="rpg-token token-power">PM</span>.  
3) Gasta <span class="rpg-token token-power">PM</span> y lanza **Poder (<span class="rpg-token token-stat">P</span>)**.

### 7.2 Niveles de efecto (T / costo)

- **Truco:** efecto breve, truco → <span class="rpg-token token-t">T 4</span>, costo 0–1 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>
- **Estándar:** ataque, escudo, impulso → <span class="rpg-token token-t">T 5</span>, costo 1 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>
- **Fuerte:** área, curación, parálisis, hackeo "en vivo" → <span class="rpg-token token-t">T 6</span>, costo 2 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>
- **Grande:** cambio de escena, intervención poderosa → <span class="rpg-token token-t">T 8–12</span>, costo 3 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>

### 7.3 Fracaso y Éxito Excepcional

- Fracaso: los <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span> gastados se pierden, y se aplica la consecuencia (sobrecarga, rastro, pérdida de posición, efecto secundario).
- <span class="rpg-token token-stat">M</span>áximo en el dado: éxito excepcional + beneficio adicional (mayor alcance, mayor duración, efecto más fuerte, o menos "efectos secundarios").

### 7.4 Recuperación <span class="rpg-token token-power">PM</span>

- Después de una escena de conflicto, recuperas **1 <span class="rpg-token token-power">PM</span>**.
- Después de un descanso seguro - hasta el máximo (si el mundo del juego lo permite).

**Ejemplo (fantasía):** "Salto corto" – Estándar, <span class="rpg-token token-t">T 5</span>, costo 1 <span class="rpg-token token-power">PM</span>.  
**Ejemplo (ciencia ficción):** "Sobrecargo el cerrojo electrónico" – Estándar, <span class="rpg-token token-t">T 5</span>, costo 1 <span class="rpg-token token-power">PM</span>.




---

### 8) Descanso y recuperación

Si tenéis un momento seguro (refugio, vendaje, servicio, comida):
- vuelven a tener **Corazones** completos,
- y reponen **<span class="rpg-token token-power">PM</span>** de acuerdo con la regla de descanso en vuestra convención.

En campañas más rigurosas, el MG puede requerir una parada completa para recuperar todo.



---

### 9) Desarrollo de personajes (cuando "subes de nivel")

El desarrollo ocurre **después de la aventura** (usualmente después de 1–3 sesiones, dependiendo del ritmo de la campaña).  
Eliges **uno**:
- sube una característica en 1 grado de dado (máx. hasta <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">d20</span></span>), o
- +1 Corazón (máx. 7), o
- +1 <span class="rpg-token token-power">PM</span> (máx. 5), o
- nuevo Rasgo (una regla breve, de una oración, acordada con el MG).

**Ejemplo:** La Destreza sube de <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span> a <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span>. A partir de ahora, todos los tests de D lo haces en <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span>.

---



---

### 10) Variante "solo <span class="rpg-token token-d6">d6</span>": 2d6

Si deseas jugar solo con <span class="rpg-token token-d6">d6</span>:
- Cada prueba es **2d6 + modificador de característica**.
- Modificadores de características al inicio: una característica **+2**, una **+1**, una **+0**.

**Resultado:**
- **6 o menos** – fracaso con consecuencia  
- **7–9** – éxito con costo  
- **10+** – éxito completo  
- **12** – éxito excepcional

**Situación:** da **+1 / -1** al tiro (favorece / dificulta), en lugar de cambiar los umbrales.

**Golpe de Suerte en 2d6:** funciona de la misma manera, solo que "mejorar los dados" se cambia por **+1 al tiro**.

---



---

### 11) Buenos hábitos del jugador

- Habla: **qué haces + para qué**. El objetivo de las acciones facilita al MG establecer la apuesta. - Si la Dificultad es alta: no "forces la tirada" — **cambia la situación** (preparación, herramienta, cobertura, ayuda, otro camino). - Colabora: la ayuda de un aliado es una de las palancas más fuertes y simples del sistema. - En combate, ganar la posición: la cobertura, la distancia y la ventaja situacional son a menudo más importantes que la estadística.

