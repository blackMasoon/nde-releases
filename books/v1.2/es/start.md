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
generated_at: "2026-01-13T06:27:17.022Z"
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

### 1) Héroe en 1 minuto

- Rol (elige uno):
  - Guerrero — maestro de la fuerza y el combate cuerpo a cuerpo
  - Pícaro — maestro de la velocidad, el sigilo y los disparos
  - Mago — maestro de los hechizos y el conocimiento
- Características y dados: Fuerza (F), Destreza (D), Magia (M).
  - Guerrero: F <span class="rpg-token token-d10">d10</span>, D <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d6">d6</span>
  - Pícaro: F <span class="rpg-token token-d6">d6</span>, D <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
  - Mago: F <span class="rpg-token token-d6">d6</span>, D <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d10">d10</span>
- Vida: 5 Corazones. Mana: 3 (usado para hechizos).
- Equipamiento: arma, armadura ligera, 3 objetos adecuados para el rol.
Ejemplo: El Pícaro tiene Destreza <span class="rpg-token token-d10">d10</span>, por lo que usa <span class="rpg-token token-d10">d10</span> para los disparos.



---

### 2) ¿Cómo realizas acciones?

1. Elige la característica adecuada (S/Z/M) y lanza el dado de esa característica.
2. Compara con el nivel de dificultad (<span class="rpg-token token-tn">TN</span>):
   - Fácil 4, Normal 6, Difícil 8, Heroico 12.
3. Resultado:
   - 1 en el dado — fracaso con complicación (ruido, pérdida de tiempo, pequeña herida, etc.).
   - Resultado < <span class="rpg-token token-tn">TN</span> — fracaso.
   - Resultado ≥ <span class="rpg-token token-tn">TN</span> — éxito.
   - Máximo en el dado (por ejemplo, 10 en <span class="rpg-token token-d10">d10</span>, 20 en <span class="rpg-token token-d20">d20</span>) — éxito excepcional con un beneficio adicional.
Mejoras sin contar:
- Mejor/peor situación: baja/aumenta la <span class="rpg-token token-tn">TN</span> en 1 grado (por ejemplo, 6 → 8 por cobertura).
- Ayuda de un aliado (con su acción): para esta tirada "aumenta" el dado en un tamaño (<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>).
Ejemplo: El guerrero fuerza la puerta (Normal 6). Lanza un <span class="rpg-token token-d10">d10</span> y saca 10 — éxito excepcional: la puerta vuela, y el guardia que está detrás de ella se cae.



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

### 4) Magia (prosto)

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

