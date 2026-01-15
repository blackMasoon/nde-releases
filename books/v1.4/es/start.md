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
generated_at: "2026-01-15T07:57:22.461Z"
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
# Reglas de un vistazo

Automatic translation placeholder for es

---



---

### 1) Héroe en 1 minuto


* **Concepto:** quién eres y en qué género juegas (1 frase).
* **Rol (elige uno):**

  * **Asalto** – presión, combate, superación de obstáculos
  * **Especialista** – sigilo, precisión, técnica, observación
  * **Adept** – poderes, conocimiento, influencia, improvisación
* **Características (3):**

  * **Fuerza (F)** – fuerza física, resistencia, combate cuerpo a cuerpo
  * **Destreza (D)** – reflejos, sigilo, disparo, pilotaje
  * **Poder (<span class="rpg-token token-stat">P</span>)** – magia/psiónica/tecnología/engaño/intuición (dependiendo del mundo)
* **Dados de características:** una característica **<span class="rpg-token token-d12">k12</span>**, una **<span class="rpg-token token-d8">k8</span>**, una **<span class="rpg-token token-d6">k6</span>** (elige según el rol).
* **Corazones:** 5. **Puntos de Poder:** 3 (los gastas en poderes y "jugadas especiales").
A continuación, tienes un fragmento listo para pegar (variante A), en el estilo de reglas breves "1-page".

**Tirada de Suerte (cómo funciona):** gasta **1 TS**, para elegir uno:

* **Repetición** de tu prueba (dejas el mejor resultado), o
* **Aumento del dado en 1 grado** en esa única tirada (**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>**), o
* **Cambio de un fallo a “éxito con costo”** — la acción tiene éxito, pero el DJ inmediatamente impone un costo (por ejemplo, pierdes tiempo, haces ruido, gastas un recurso, terminas en una peor posición, atraes atención, rompes equipo).

**Recuperación de TS:** al comienzo de la siguiente sesión vuelves al límite. El DJ puede otorgar **+1 TS** por un riesgo audaz, una gran decisión narrativa o jugar con las consecuencias.

* **Equipo:** 1 herramienta “clave” (por ejemplo, espada, rifle, kit de hacker), 1 protección (armadura, escudo energético, camuflaje), 3 objetos pequeños que se ajusten al concepto.

**Ejemplo:** Especialista: F <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">P</span> <span class="rpg-token token-d8">k8</span>, D <span class="rpg-token token-d6">k6</span>. En ciberpunk, <span class="rpg-token token-stat">P</span> es “Hackeo/Influencia”; en fantasía, <span class="rpg-token token-stat">P</span> es “Magia/Voluntad”.



---

### 2) Cómo resolver acciones


1. El jugador dice **qué hace** y **cómo** (descripción en el mundo del juego).
2. El director establece la **Dificultad** y la apuesta ("qué sucederá en caso de fracaso").
3. Lanza el dado de atributo (F/D/C) y compara con la Dificultad.

**Dificultad (D):**

* **3** fácil, **4** estándar, **5** difícil, **6** muy difícil, **8** heroico, **12** legendario.

**Resultado de la tirada:**

* **1** – fracaso con consecuencia (la complicación entra seguro).
* **< D** – fracaso (pero la escena continúa: pérdida de tiempo, ruido, peor posición, pérdida de recurso).
* **≥ D** – éxito.
* **<span class="rpg-token token-stat">M</span>áximo en el dado** (por ejemplo, 12 en <span class="rpg-token token-d12">k12</span>, 20 en <span class="rpg-token token-d20">k20</span>) – éxito excepcional: obtienes un beneficio adicional.

**Modificadores sin contar:**

* **Mejor situación**: sube el dado 1 grado (<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>).
* **Peor situación**: baja el dado 1 grado (<span class="rpg-token token-d20">k20</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d4">k4</span>).
* **Ayuda de un aliado** (cuesta su acción): sube el dado 1 grado.

**Ejemplo:** Un adepto intenta cerrar un portal (D <span class="rpg-token token-d8">k8</span>) bajo alarma y estrés → peor situación, baja a <span class="rpg-token token-d6">k6</span>. D = 5. Tirada 6: éxito, pero "alarma" permanece de fondo como presión narrativa.



---

### 3) Movimiento y combate – por defecto sin cuadrícula, cuadrícula como opción

**Por defecto: teatro de la mente (recomendado)**

* Describe las distancias como: **Cerca** (al alcance), **No muy lejos** (unos pasos), **Lejos** (al otro lado del escenario), **Muy lejos** (sniper/vehículo).
* En un turno tienes: **Movimiento + 1 Acción**.

  * El movimiento normalmente cambia la distancia en 1 “grado” (No muy lejos→Cerca, etc.).
* **Ataque**: tira **C** (cuerpo a cuerpo) o **D** (distancia) contra la **Defensa** del objetivo.

**Defensa de los oponentes (aproximadamente):**

* **Débil** 4, **Típico** 5, **Élite** 6, **Jefe** 8 (jefe legendario 12).

**Efectos de un impacto (combate rápido):**

* Un impacto causa **1 Corazón**.
* Un éxito excepcional causa **2 Corazones** o proporciona un efecto fuerte (desarme, derribo, dispersión).

**Cobertura y ventaja posicional:**

* Cobertura ligera / ángulo desfavorable: reduce el dado del atacante en 1 grado.
* Buena posición / sorpresa: aumenta el dado en 1 grado.

**Opción: juego en cuadrícula**

* 1 casilla = 1–2 m. Movimiento en un turno: **hasta 5 casillas**. El resto de las reglas sin cambios.

**Ejemplo:** Un especialista dispara desde cobertura (D <span class="rpg-token token-d12">k12</span>) a una élite (Defensa 6). El objetivo está en cobertura ligera → D baja a <span class="rpg-token token-d8">k8</span>. Tiro 7: éxito, 1 Corazón de daño.



---

### 4) Poderes, "hechizos" y jugadas especiales (universales)


Esto incluye magia, psiónica, cibernética, gadgets, trucos de cine – dependiendo del mundo.

* Cuando haces algo **más allá de lo estándar**: gasta **Punto de Poder** y lanza **<span class="rpg-token token-stat">M</span>**.
* Establece el nivel del efecto:

**Niveles de poder (T / costo):**

* **Truco** (efecto corto, truco, "flash"): **T 4 / 0–1 PP**
* **Estándar** (ataque, escudo, impulso, control menor): **T 5 / 1 PP**
* **Fuerte** (área, curación, parálisis, hackeo "en vivo"): **T 6 / 2 PP**
* **Grande** (cambio de escena, intervención poderosa): **T 8–12 / 3 PP**

**Fallo:** PP se pierde, y la consecuencia es inmediata (sobrecarga, rastro digital, rasguño en el ritual, atención no deseada).

**Recuperación:** después de la escena de conflicto recuperas **1 PP**, después de un descanso seguro – hasta el máximo.

**Ejemplo:** En una ópera espacial, el Adepto intenta "doblar el sensor" de un dron: Estándar, T 5, costo 1 PP. Lanzamiento <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span> = 8: éxito excepcional – el dron pierde la señal y se confunde de pista.



---

### 5) Caída, riesgo y curación

* Cuando caes a **0 Corazones**, estás **fuera de acción** (herido, aturdido, en shock – según la convención).
* Un aliado puede gastar una acción para ponerte en **1 Corazón** (primeros auxilios, adrenalina, reinicio del sistema).
* Después de la escena, si tienen un momento de respiro: regresan a **Corazones completos**, siempre que tengan las condiciones (refugio, vendaje, servicio, comida).
* Si la escena fue especialmente brutal o los enemigos tienen ventaja, el Director puede requerir que un "reinicio completo" necesite una parada segura.

**Ejemplo:** El Asalto cae a 0. El Especialista lo arrastra a cubierto y gasta una acción: El Asalto regresa a 1 Corazón y puede actuar en la siguiente ronda.



---

### 6) Desarrollo de personajes (campaña sin tablas ni contabilidad)


Después de la aventura, elige **una**:

* **Aumenta** una característica en 1 grado (máx. hasta <span class="rpg-token token-d20">k20</span>), o
* **+1 Corazón** (máx. 7), o
* **+1 Punto de Poder** (máx. 5), o
* **Nuevo Rasgo** (una regla corta de una frase acordada con el Director de Juego).

**Ejemplos de rasgos (universales):**

* **Énfasis:** una vez por escena, cuando golpeas en cuerpo a cuerpo, infliges +1 Corazón de daño.
* **Sombra:** cuando actúas desde las sombras, tienes un aumento de dado de 1 grado.
* **Chispa:** una vez por escena puedes gastar 1 PP para obtener automáticamente "éxito con costo" sin tirar.

**Ejemplo:** El Adepto aumenta <span class="rpg-token token-stat">M</span> de <span class="rpg-token token-d8">k8</span> a <span class="rpg-token token-d12">k12</span> – ahora sus poderes se activan de manera más estable con T 5–6.



---

### 7) Variante "solo <span class="rpg-token token-d6">k6</span>" en modo **2k6** (rápido y muy jugable)


Si no tienes un conjunto de dados o quieres grados de resultado más "narrativos":

* Cada prueba es: **lanza 2k6 + modificador de atributo**.
* **Modificadores de atributos** elige al inicio: un atributo **+2**, uno **+1**, uno **+0**.
* Resultado:

  * **6 o menos** – fracaso con consecuencia
  * **7–9** – éxito con costo (compromiso, pérdida de recurso, peor posición)
  * **10+** – éxito total
  * **12** – éxito excepcional (beneficio adicional)

**Dificultad de la situación:** en lugar de cambiar los umbrales, da **+1 / -1** a la tirada (favorece / dificulta) o un costo en caso de 7–9.

**Mapeo a la versión de dados-atributos (si deseas compatibilidad):**

* <span class="rpg-token token-d6">k6</span> ≈ +0, <span class="rpg-token token-d8">k8</span> ≈ +1, <span class="rpg-token token-d12">k12</span> ≈ +2, <span class="rpg-token token-d20">k20</span> ≈ +3 (para personajes muy experimentados).

**Ejemplo:** Un especialista dispara mientras corre: <span class="rpg-token token-stat">Z</span> = +2, situación difícil (-1). Tirada 2k6 = 8, suma 9: éxito con costo – acierta, pero termina en una posición expuesta.

