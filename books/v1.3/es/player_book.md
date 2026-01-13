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
generated_at: "2026-01-13T12:23:32.729Z"
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
# Manual del Jugador

Automatic translation placeholder for es

---



---

### MG describe la situación y dice lo que es posible.
- Tú dices, **qué haces** y **qué efecto deseas**.
- Si el resultado es incierto, MG dice.

- MG describe la situación y dice qué es posible.
- Tú dices **qué haces** y **qué efecto deseas**.
- Si el resultado es incierto, el MG dice:
  1) qué rasgo usas (S/Z/M),
  2) cuál es la dificultad (<span class="rpg-token token-tn">TN</span>),
  3) qué puede suceder en caso de fracaso.
- Tú lanzas **un dado** de tu rasgo y miras si el resultado ≥ <span class="rpg-token token-tn">TN</span>.

### La regla más corta



---

### 1. Introducción

Tu personaje tiene:
- **Rol** (Guerrero / Pícaro / Mago),
- 3 **atributos**: Fuerza (F), Destreza (D), Magia (M),
- **Vida** (Corazones) y **Maná**,
- 2 **Talentos** (opcional, pero recomendado),
- equipo.

### 2.1 Características (S/Z/M) — para qué sirven
- **Fuerza (S)**: combate cuerpo a cuerpo, forzar, levantar, resistencia.
- **Destreza (Z)**: disparos, precisión, sigilo, esquivar, acrobacias.
- **Magia (M)**: efectos "especiales" (hechizos/psiónica/tecnología — dependiendo del juego).

### 2.2 Huesos de características
Cada característica tiene su propio hueso (por ejemplo, <span class="rpg-token token-d6">d6</span>, <span class="rpg-token token-d8">d8</span>, <span class="rpg-token token-d10">d10</span>, <span class="rpg-token token-d12">d12</span>, <span class="rpg-token token-d20">d20</span>). Siempre lanzas **un** hueso.
- Hueso más grande = mayor probabilidad de obtener resultados altos.

### 2.3 Vida y Maná
- **Vida:** 5 Corazones (inicio).
- **Maná:** 3 (inicio). La gastas cuando usas Magia.



---

### Paso 1: Elige un rol
Elige un rol. Establece los dados de características iniciales:
- **Guerrero:** F <span class="rpg-token token-d10">d10</span>, D <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d6">d6</span>
- **Pícaro:** F <span class="rpg-token token-d6">d6</span>, D <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
- **Mago:** F <span class="rpg-token token-d6">d6</span>, D <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d10">d10</span>

### Paso 2: Registra los recursos

### Paso 3: Elige 2 Talentos (opcionalmente)
Los talentos son frases cortas que describen en qué eres bueno.
- Ejemplos neutrales: "Negociador", "Explorador", "Mecánico", "Médico", "Atleta", "Analista", "Hacker".

**Cómo funcionan los Talentos:** si un Talento realmente ayuda en la prueba, el MG puede **reducir la dificultad (<span class="rpg-token token-tn">TN</span>) en 1 grado**.
- Normalmente 1 Talento por prueba.
- El Talento no reemplaza la descripción de la acción — ayuda cuando realmente tiene sentido.

### Paso 4: Equipo
Enumera:
- 1 herramienta de combate (cuerpo a cuerpo o a distancia),
- protección (si aplica),
- 3 objetos útiles.

El equipo en este juego generalmente funciona como **"permiso"**: tienes algo, así que puedes intentar realizar ciertas acciones.

### Ejemplo de personaje
- Rol: Pícaro
- S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
- Vida 5, Maná 3
- Talentos: “Explorador”, “Negociador”
- Equipo: herramienta a distancia, ganzúas, cuerda, linterna



---

### 4.1 Cuándo tiras
Tiras cuando:
- algo es **arriesgado** o incierto,
- y el fracaso tiene consecuencias.

Si algo es obvio y sin presión, el MG puede decir "tiene éxito" sin tirar.

### 4.2 Dificultades (<span class="rpg-token token-tn">TN</span>)
Se utilizan 4 niveles:
- **<span class="rpg-token token-tn">TN</span> 4 — Fácil**
- **<span class="rpg-token token-tn">TN</span> 6 — Normal**
- **<span class="rpg-token token-tn">TN</span> 8 — Difícil**
- **<span class="rpg-token token-tn">TN</span> 12 — Heroico**

El MG elige la <span class="rpg-token token-tn">TN</span>. No necesitas "adivinarla" — el MG simplemente dice cuál es la dificultad.

### 4.3 Resultados del lanzamiento

**Nivel de Dificultad (<span class="rpg-token token-tn">TN</span>)**: 4 (Fácil), 6 (Normal), 8 (Difícil).

**Resultado de la Tirada:**
- **1**: Fracaso + Complicación.
- **< <span class="rpg-token token-tn">TN</span>**: Fracaso.
- **≥ <span class="rpg-token token-tn">TN</span>**: Éxito.
- **Max (10/20)**: Éxito + Beneficio.

### 4.3 Resultados del lanzamiento
- **Resultado ≥ <span class="rpg-token token-tn">TN</span>:** éxito.
- **Resultado < <span class="rpg-token token-tn">TN</span>:** fracaso.
- **Resultado 1:** fracaso con complicación.
- **Máximo en los dados** (por ejemplo, 10 en un <span class="rpg-token token-d10">d10</span>): éxito excepcional + beneficio adicional.

**Beneficio adicional** (ejemplos): más rápido, más silencioso, más seguro, mayor efecto, mejor posición.

### 4.4 Cambios en la dificultad "por grado"
En lugar de contar bonificaciones, el GM a veces cambia la <span class="rpg-token token-tn">TN</span> por 1 grado:
- peores condiciones → <span class="rpg-token token-tn">TN</span> más alta (por ejemplo, 6 → 8),
- mejores condiciones → <span class="rpg-token token-tn">TN</span> más baja (por ejemplo, 8 → 6).

Tu papel como jugador: **crea mejores condiciones** a través de la descripción y decisiones (cobertura, preparación, herramientas, plan).

### 4.5 Ayuda de un aliado
Un aliado puede usar su Acción para ayudarte. Entonces, en esa única tirada puedes:
- aumentar el dado en 1 tamaño: **<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>**.

La ayuda debe tener sentido en la descripción (por ejemplo, cubrir, distraer, proporcionar herramientas).

### Ejemplo de prueba
Quieres abrir rápidamente un paso bloqueado.
- MJ: "Es Destreza, <span class="rpg-token token-tn">TN</span> 6."
- Tiras [token:<span class="rpg-token token-d10">d10</span>] y sale 7 → éxito: paso abierto.



---

### 1. Kratka

- **1 casilla** es la unidad básica de distancia.
- En tu turno tienes **movimiento de hasta 5 casillas**.
- Puedes moverte en diagonal (la diagonal cuenta como 1 casilla).
- La cobertura es importante: si algo te cubre de un ataque a distancia, generalmente es más difícil acertar.



---

### 6.1 Cómo se ve un turno
En tu turno tienes:
- **Movimiento** (hasta 5 casillas),
- **1 Acción**.

La acción puede ser: atacar, usar equipo, realizar una prueba de habilidad, ayudar, usar Magia.

### 6.2 Ataque

1) Elige un objetivo (dentro del alcance y a la vista).
2) Elige un arma/hechizo.
3) Verifica qué Atributo se utiliza (por ejemplo, Fuerza en cuerpo a cuerpo, Destreza a distancia, Magia para el hechizo).
4) **Lanza.** Compara con la **<span class="rpg-token token-tn">TN</span>** del oponente.

### 6.2 Ataque
- **Cuerpo a cuerpo:** tirada de **Fuerza (F)**.
- **Distancia:** tirada de **Destreza (D)**.
- El GM indica la <span class="rpg-token token-tn">TN</span> del oponente.

<span class="rpg-token token-tn">TN</span> predeterminadas de los oponentes:
- **Esbirro:** <span class="rpg-token token-tn">TN</span> 6
- **Élite:** <span class="rpg-token token-tn">TN</span> 8
- **Jefe:** <span class="rpg-token token-tn">TN</span> 12

### 6.3 ¿Qué significa un golpe?

- **Esbirro**: Muere (o queda fuera de combate).
- **Élite/Jefe**: Pierde **1 Corazón**.
- **Jugador**: Pierde **1 Corazón** (a menos que tenga Armadura — entonces la Armadura absorbe el golpe, pero se desgasta).

### 6.3 ¿Qué significa un impacto?
- Golpeas a un esbirro → sale de la pelea.
- Golpeas a una élite/jefe → recibe una Herida (el jefe tiene 3 Heridas por defecto).
- Éxito excepcional contra una élite/jefe → normalmente infliges +1 Herida (un total de 2), o ganas una ventaja situacional (por ejemplo, empujar fuera de cobertura).

### 6.4 Fallo y "Venganza"

El combate tiene riesgos. Si **no aciertas** (resultado < <span class="rpg-token token-tn">TN</span>) o sacas un **1**:
- El enemigo contraataca: pierdes **1 Corazón**.
- O sucede otra complicación lógica (ej. pierdes el arma, eres derribado).

*No es el turno del enemigo, es el efecto de tu ataque fallido.*

### 6.4 Fallo y "Venganza"
Si **fallas** (resultado < <span class="rpg-token token-tn">TN</span>) y el enemigo podía alcanzarte realmente, pierdes **1 Corazón**.
- En cuerpo a cuerpo es común.
- En ataques a distancia depende mucho de la cobertura y la situación.

Tu lección táctica: **posiciciónate para no recibir venganza al fallar** (cobertura, distancia, plan, ayuda).

### 6.5 0 Serc

Si caes a 0 Corazones:
- Estás **Derribado**.
- No puedes realizar acciones (solo arrastrarte y hablar con las pocas fuerzas que te quedan).
- Un aliado puede "levantarte" (acción de Ayuda), restaurando 1 Corazón.
- Si recibes daño estando Derribado — **Mueren**.

### 6.5 0 Corazones
Cuando caes a 0 Corazones:
- estás derribado y no realizas acciones,
- un aliado puede gastar una Acción para levantarte con **1 Corazón**.

### Ejemplo de un turno corto
- Movimiento: corres 3 casillas hacia la cobertura.
- Acción: disparas (Z). MJ: "<span class="rpg-token token-tn">TN</span> 6, pero el objetivo está detrás de la cobertura → <span class="rpg-token token-tn">TN</span> 8". Tiras <span class="rpg-token token-d10">d10</span>=9 → impacto.



---

### 1. Introducción

Magia a mecánica de "efectos especiales". Tú describes el efecto, el MG establece la <span class="rpg-token token-tn">TN</span> y el costo de Maná.

### 7.1 Costos y niveles
- **Truco:** <span class="rpg-token token-tn">TN</span> 4, costo 0–1
- **Estándar:** <span class="rpg-token token-tn">TN</span> 6, costo 1
- **Efecto fuerte:** <span class="rpg-token token-tn">TN</span> 8, costo 2
- **Gran poder:** <span class="rpg-token token-tn">TN</span> 12, costo 3

### 7.2 Fracaso en la Magia
Cuando la Magia falla:
- pierdes la Mana gastada,
- aparece una consecuencia (por ejemplo, -1 Corazón, pérdida de posición, amenaza adicional).

### 7.3 Éxito excepcional
El máximo en los dados de Magia otorga un beneficio adicional:
- mayor alcance/área,
- mayor duración,
- mayor efectividad,
- o un menor costo (el MJ puede devolver 1 Mana).

### Ejemplo de Magia
Quieres realizar un breve "salto" de 5 casillas.
- MG: "Es Estándar: <span class="rpg-token token-tn">TN</span> 6, costo 1."
- Pagas 1 Mana, tiras M <span class="rpg-token token-d10">d10</span>=7 → éxito: saltas detrás de la cobertura.



---

### 1. Introducción

Después del conflicto, si tienen un momento seguro y las condiciones básicas para descansar:
- La Vida y el Maná regresan a su máximo.



---

### 1. Introducción

Después de la aventura eliges **uno**:
- aumentar S/Z/M en 1 tamaño de dado: <span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>,
- o +1 Corazón (máx 7),
- o +1 Maná (máx 5).

Esto significa desarrollo sin añadir más dados a las tiradas.



---

### 1. Introducción

Si en la mesa solo hay un <span class="rpg-token token-d6">d6</span>, en lugar del tamaño del dado tienes un umbral de éxito:
- Maestro 3+, Entrenado 4+, Novato 5+, Sin habilidad 6.

El GM puede aumentar/disminuir el umbral en 1 grado por situación o ayuda.



---

### Siempre di

- Siempre di: **qué haces** + **para qué**. "Quiero presionar la palanca" está bien, pero "quiero presionar la palanca para cerrar el paso" es aún mejor.
- Si el <span class="rpg-token token-tn">TN</span> es alto: no "agobies el lanzamiento" — cambia la situación (cubierta, herramientas, ayuda, otro camino).
- Establezcan colaboración: una persona ayuda, la otra realiza la prueba.
- En combate, respeta la cobertura y la posición — a menudo son más importantes que el propio lanzamiento.

---
Fin del libro del jugador.

