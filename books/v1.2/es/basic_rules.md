---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.2
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
generated_at: "2026-01-12T20:13:55.918Z"
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
# Libro de Reglas Básicas



---



---

[ES] Marcador de posición...




---

[ES] Marcador de posición...




---

[ES] Marcador de posición...


### 3.1 Cuándo tirar
[ES] Marcador de posición...


### 3.2 Cómo tirar
[ES] Marcador de posición...


### 3.3 Escala de dificultad (<span class="rpg-token token-tn">TN</span>)
[ES] Marcador de posición...


### 3.4 Resultados
[ES] Marcador de posición...


### 3.5 Ajustar dificultad
[ES] Marcador de posición...


### 3.6 Ayuda
[ES] Marcador de posición...




---

[ES] Marcador de posición...


### 4.1 Casillas
[ES] Marcador de posición...


### 4.2 Movimiento
[ES] Marcador de posición...


### 4.3 Cobertura
[ES] Marcador de posición...


### Wyniki Testu

> **Nivel de Dificultad (<span class="rpg-token token-tn">TN</span>)**: 4 (Fácil), 6 (Normal), 8 (Difícil).
> 
> **Resultado de la Tirada:**
> - **1**: Fracaso + Complicación.
> - **< <span class="rpg-token token-tn">TN</span>**: Fracaso.
> - **≥ <span class="rpg-token token-tn">TN</span>**: Éxito.
> - **Max (10/20)**: Éxito + Beneficio.

---

### 3.4 Resultados de la prueba
- **Resultado ≥ <span class="rpg-token token-tn">TN</span> → Éxito.** La figura logra el efecto deseado.
- **Resultado < <span class="rpg-token token-tn">TN</span> → Fracaso.** El efecto no se produce.
- **Resultado de 1 → Fracaso + complicación.** (Incluso si <span class="rpg-token token-tn">TN</span> es bajo.)
- **Resultado máximo en los dados → Éxito excepcional.**
  - Además del éxito, obtienes **un beneficio adicional**.
  - El beneficio adicional debe derivarse de la situación (más efecto, menos riesgo, más rápido, más silencioso, etc.).

### 3.5 Modificación de la dificultad "sin contar"
En lugar de añadir +1/−1 a las tiradas, cambiamos la <span class="rpg-token token-tn">TN</span> en **un grado**.

- **Condiciones peores** → <span class="rpg-token token-tn">TN</span> +1 grado (por ejemplo, 6→8):
  - cobertura del objetivo, oscuridad, resbaladizo, presión del tiempo, ruido, distracción.
- **Condiciones mejores** → <span class="rpg-token token-tn">TN</span> −1 grado (por ejemplo, 8→6):
  - preparación, buenas herramientas, ventaja de posición, sorpresa, concentración total.

Si algo es "extremadamente" difícil/fácil, el MJ puede moverlo **2 grados**.

**Límites:**
- Si después de las reducciones la <span class="rpg-token token-tn">TN</span> cae por debajo de 4, considéralo "casi seguro" (normalmente sin tirada).
- Si después de las aumentos la <span class="rpg-token token-tn">TN</span> supera 12, considéralo "casi imposible" (normalmente requiere un plan u otro enfoque).

### 3.6 Ayuda de un aliado
Un aliado puede en su turno (o en una escena fuera de combate) dedicar una Acción para ayudar.

**Efecto de la ayuda (núcleo):** en esta única prueba, aumenta el tamaño del dado en 1:
- <span class="rpg-token token-d6">d6</span> → <span class="rpg-token token-d8">d8</span> → <span class="rpg-token token-d10">d10</span> → <span class="rpg-token token-d12">d12</span> → <span class="rpg-token token-d20">d20</span>

Reglas de orden:
- Normalmente, **una persona** puede ofrecer ayuda en una única prueba (para evitar crear una "torre de ayuda").
- La ayuda debe ser descrita de manera sensata: cubrir, proporcionar herramientas, distraer, estabilizar, dar pistas.

### 3.7 Repetición de pruebas
Si la prueba falla, no la repitas "una y otra vez" sin cambiar la situación.
- O haces algo diferente (otra característica / otras herramientas / otro enfoque),
- o aceptas la complicación (por ejemplo, el consumo de tiempo, una alarma),
- o te retiras.

### 3.8 Ejemplos de pruebas (fuera de combate)
**Ejemplo A — paso silencioso:**
- Jugador: “Quiero atravesar el espacio abierto sin ser visto”.
- MJ: Agilidad (A). Hay penumbra y obstáculos → <span class="rpg-token token-tn">TN</span> 6 (Normal).
- Tiro <span class="rpg-token token-d10">d10</span>=5 → fracaso. MJ: “No te notan de inmediato, pero alguien escucha un sonido y comienza a revisar el área (complicación: presión de tiempo)”.

**Ejemplo B — trabajo con herramientas:**
- Jugador: “Quiero activar el mecanismo rápidamente”.
- MJ: Fuerza, si es puramente físico, o Magia, si es un efecto especial; aquí: Fuerza (F). <span class="rpg-token token-tn">TN</span> 6.
- Un aliado ayuda (aumenta el dado). Tiro <span class="rpg-token token-d12">d12</span>=12 → éxito excepcional: funciona de inmediato y además no hace ruido.



---

[ES] Marcador de posición...


### 5.1 Inicio del combate
[ES] Marcador de posición...


### 5.2 Orden de turno
[ES] Marcador de posición...


### 5.3 Acciones
[ES] Marcador de posición...




---

[ES] Marcador de posición...


### 6.1 Maná
[ES] Marcador de posición...


### 6.2 Resolución
[ES] Marcador de posición...


### 6.3 Niveles de efecto
[ES] Marcador de posición...


### Atak

> 1) Elige un objetivo (dentro del alcance y a la vista).
> 2) Elige un arma/hechizo.
> 3) Verifica qué Atributo se utiliza (por ejemplo, Fuerza en cuerpo a cuerpo, Destreza a distancia, Magia para el hechizo).
> 4) **Lanza.** Compara con la **<span class="rpg-token token-tn">TN</span>** del oponente.

---

### 6.4 Magia crítica
[ES] Marcador de posición...


### Trafienie

> - **Pachołek**: Muere (o queda fuera de la lucha).
> - **Élite/Jefe**: Pierde **1 Corazón**.
> - **Jugador**: Pierde **1 Corazón** (a menos que tenga Armadura — entonces la Armadura absorbe el impacto, pero se desgasta).

---

### 6.5 Ejemplos de magia
[ES] Marcador de posición...


### Pudło i Odwet

> Walka ma ryzyko. Jeśli **no aciertas** (resultado < <span class="rpg-token token-tn">TN</span>) o sacas **1**:
> - El oponente contraataca: pierdes **1 Corazón**.
> - O sucede otra complicación lógica (por ejemplo, pierdes un arma, te derriban).
> 
> *No es el turno del oponente — es el efecto de tu ataque fallido.*

---

### 5.6 Pudło y “Venganza”
La lucha conlleva riesgos. Cuando atacas y fallas, el oponente a menudo “responde”.

**Regla de venganza (núcleo):** si el resultado del ataque < <span class="rpg-token token-tn">TN</span> y el oponente podría alcanzarte realmente, pierdes **1 Corazón**.

Cómo entender “podría alcanzarte” (sin complicaciones):
- si atacas cuerpo a cuerpo (estás al lado) — casi siempre sí,
- si atacas a distancia, y estás en un espacio abierto y el oponente tiene la posibilidad de contraatacar — generalmente sí,
- si tienes cobertura total o estás fuera del alcance real del peligro — generalmente no.

**Sacar un 1 en combate:** fracaso + complicación. Esto generalmente significa: pierdes 1 Corazón y además algo empeora (por ejemplo, te caes, pierdes el arma, eres empujado fuera de la cobertura).

### 5.7 Rango de ataques (predeterminado)
Para no multiplicar números, utiliza reglas simples:
- A quemarropa: objetivo en la casilla adyacente.
- Distancia: objetivo en "rango de visión" en el tablero.
  - Si el MJ desea limitaciones: acepta **hasta 10 casillas** sin penalización; más de 10 casillas <span class="rpg-token token-tn">TN</span> +1 grado.

### 5.8 Varios oponentes a la vez
Si varios matones están "en combate" con un personaje, el MJ puede:
- aumentar la <span class="rpg-token token-tn">TN</span> en 1 grado (presión), o
- considerar que un fallo significa una complicación adicional (por ejemplo, pierdes la posición).

La regla debe ser rápida: **una resolución → un efecto**.

### 5.9 Ejemplos de combate (paso a paso)
**Ejemplo A — intercambio simple en combate cuerpo a cuerpo:**
- El guerrero (S <span class="rpg-token token-d10">d10</span>) está al lado de un peón (<span class="rpg-token token-tn">TN</span> 6).
- Tiro <span class="rpg-token token-d10">d10</span>=4 → fallo. Dado que es combate cuerpo a cuerpo, se aplica la represalia → El guerrero pierde 1 Corazón.

**Ejemplo B — jefe y éxito excepcional:**
- El pícaro (Z <span class="rpg-token token-d10">d10</span>) dispara al Jefe (<span class="rpg-token token-tn">TN</span> 12). El MJ dice: “Sin preparación, es difícil”.
- Un aliado ayuda (<span class="rpg-token token-d12">d12</span>) y el pícaro tiene una buena posición (<span class="rpg-token token-tn">TN</span> 12 → 8).
- Tiro <span class="rpg-token token-d12">d12</span>=12 → éxito excepcional: El Jefe recibe 2 Heridas.



---

En esta mecánica, "Magia" es una categoría de efectos especiales. Dependiendo del mundo, puede significar:
- hechizos, psiónica,
- equipo/tecnología,
- habilidades sobrehumanas,
- cualquier otro "recurso especial" del personaje.

### 6.1 Maná
- Al inicio tienes **3 Manás**.
- El maná se gasta cuando intentas obtener un efecto "más allá de las capacidades normales".

### 6.2 Cómo funciona el uso de la Magia
1) Describe el efecto que deseas lograr.
2) El GM asigna la <span class="rpg-token token-tn">TN</span> y el costo de Maná.
3) Gasta Maná.
4) Lanza el dado de Magia (M) y compáralo con la <span class="rpg-token token-tn">TN</span>.

**Fallo:** el efecto no funciona; el Maná se pierde; se produce una pequeña consecuencia.

### 6.3 Niveles de efectos (<span class="rpg-token token-tn">TN</span> y costo)
- **Truco:** <span class="rpg-token token-tn">TN</span> 4, costo 0–1
  - pequeño efecto: luz, sonido, cortina de humo, distracción momentánea.
- **Estándar:** <span class="rpg-token token-tn">TN</span> 6, costo 1
  - proyectil, barrera, salto de 5 casillas, refuerzo corto.
- **Fuerte:** <span class="rpg-token token-tn">TN</span> 8, costo 2
  - área, control, curación +2 Corazones, inmovilización.
- **Gran poder:** <span class="rpg-token token-tn">TN</span> 12, costo 3
  - efecto grande y escénico que cambia la situación.

### 6.4 Éxito excepcional en Magia
Si sacas el máximo en los dados de Magia:
- aumenta la escala del efecto (por ejemplo, mayor área / más tiempo / más fuerte), o
- reduce el costo (el MJ puede devolver 1 Mana), o
- añade un beneficio adicional (por ejemplo, el efecto es silencioso, preciso, seguro para los aliados).

### 6.5 Ejemplos de Magia
**Ejemplo A — defensa:**
- Jugador: "Quiero crear una corta barrera para correr de forma segura 5 casillas".
- MJ: <span class="rpg-token token-tn">TN</span> estándar 6, costo 1.
- Tiro M <span class="rpg-token token-d10">d10</span>=9 → éxito: corres, la situación es más segura.

**Ejemplo B — fracaso y consecuencia:**
- Jugador: "Quiero inmovilizar a la élite" (<span class="rpg-token token-tn">TN</span> 8, costo 2).
- Tiro=3 → fracaso: el efecto no funciona, pierdes 2 Manas y aparece una complicación (por ejemplo, te expones).



---

### 7.1 Corazón (vida)
- Estándarmente tienes **5 Corazones**.
- La pérdida de un Corazón significa daño real o agotamiento — dependiendo del mundo.

### 0 Serc

> Si caes a 0 Corazones:
> - Estás **Derribado**.
> - No puedes realizar acciones (solo arrastrarte y hablar con las pocas fuerzas que te quedan).
> - Un aliado puede "levantarte" (acción de Ayuda), restaurando 1 Corazón.
> - Si recibes daño estando Derribado — **Mueren**.

---

### 7.2 0 Corazones
Si caes a 0 Corazones:
- estás **derribado** y no realizas acciones,
- un aliado puede sacrificar una Acción para levantarte con **1 Corazón**.

### 7.3 Descanso
Después de una escena de combate/conflicto, si tienen un momento de descanso seguro (y las condiciones básicas), regresan a la plenitud:
- Corazones,
- Maná.

Esto mantiene el sistema ágil y no requiere un largo proceso de curación.



---

[ES] Marcador de posición...




---

[ES] Marcador de posición...


### 9.1 Zamiast rozmiarów kości — progi
Cada característica tiene un umbral de éxito en <span class="rpg-token token-d6">d6</span>:
- **Maestro:** éxito en 3+
- **Entrenado:** éxito en 4+
- **Novato:** éxito en 5+
- **Sin habilidad:** éxito solo en 6

### 9.2 Dificultades y situación
En lugar de <span class="rpg-token token-tn">TN</span> 4/6/8/12, utiliza "grados de dificultad" mediante el cambio de umbral:
- normalmente tiras contra tu umbral,
- más difícil en 1 grado → umbral +1,
- más fácil en 1 grado → umbral −1,
- (mínimo 2+, máximo 6).

### 9.3 Ayuda

### 9.4 Lucha en solo-<span class="rpg-token token-d6">d6</span>
Puedes dejar las mismas categorías de oponentes, pero en lugar de <span class="rpg-token token-tn">TN</span> usa "grados":
- Peón: "Normal" (sin cambio en el umbral),
- Élite: "Difícil" (+1 al umbral),
- Jefe: "Heroico" (+2 al umbral) y 3 Heridas.

### 9.5 Desarrollo
Desarrollo en solo-<span class="rpg-token token-d6">d6</span>:
- eleva el nivel de una característica (por ejemplo, Novato→Entrenado),
- o +1 Corazón/Mana.



---

[ES] Marcador de posición...




---

### 1. Introducción

7.2 Los complementos no son obligatorios, pero a veces facilitan la gestión.

### 11.1 Protección (armadura) como recurso simple
Si deseas que la "protección" tenga un significado mecánico:
- Un personaje con protección tiene 1 ficha de **Armadura** por escena.
- Cuando debería perder 1 Corazón (venganza/golpe), puede en su lugar gastar la Armadura.

### 11.2 Presión del tiempo como cronómetro
Si la escena tiene un límite de tiempo, el MJ establece un "contador" (por ejemplo, 3 pasos). Cada fracaso mueve el contador en 1. Cuando llegue al final, ocurrirá una consecuencia (alarma, huida del objetivo, colapso del pasaje).

---
Fin del libro de reglas básicas.

