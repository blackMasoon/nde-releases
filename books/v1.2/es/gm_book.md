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
generated_at: "2026-01-13T06:26:36.965Z"
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
# Guía del Director de Juego

Automatic translation placeholder for es

---



---

### 7.2 Comunica claramente la tarifa.

- **Comunica claramente la dificultad.** Antes de hacer la tirada, di: característica, <span class="rpg-token token-tn">TN</span>, consecuencia del fallo, oportunidad de ayuda.
- **Descripción → mecánica → resultado.** Siempre comienza con la ficción, solo después haz la tirada.
- **Escenas rápidas.** Mantén el ritmo: una prueba = un efecto razonable.
- **El fallo impulsa la acción.** La complicación cambia la situación, no "reinicia" la escena.
- **Coherencia.** Las mismas circunstancias → las mismas <span class="rpg-token token-tn">TN</span> y consecuencias.



---

### 1. Introducción

1) El jugador dice qué hace y qué quiere lograr.  
2) Elige una característica: **S** (fuerza), **Z** (precisión/rápido), **M** (efectos especiales).  
3) Establece **<span class="rpg-token token-tn">TN</span>**: 4 fácil, 6 normal, 8 difícil, 12 heroico.  
4) Diga qué riesgos hay en caso de fracaso y si alguien puede **ayudar** (aumentar el dado en 1 tamaño).  
5) El jugador lanza el dado de la característica y compara con la <span class="rpg-token token-tn">TN</span>.  
6) Resuelve el resultado y actualiza la situación.  

Resumen para la mesa: “Características/<span class="rpg-token token-tn">TN</span>/Lanzamiento/Efecto”.



---

### 4 (fácil):

- **4 (fácil):** las condiciones son favorables, el objetivo no ofrece resistencia.
- **6 (normal):** estándar en la aventura sin ventaja.
- **8 (difícil):** presión del tiempo, mala posición, cobertura, herramientas complejas.
- **12 (heroico):** desafío excepcional; generalmente requiere preparación o un dado alto.

Modificación situacional: ajusta la <span class="rpg-token token-tn">TN</span> **en 1 grado** (máx. 2 en extremos).
- Peor: oscuro, resbaladizo, cobertura, alarma → <span class="rpg-token token-tn">TN</span> +1.
- Mejor: tiempo, herramientas, ventaja de posición, sorpresa → <span class="rpg-token token-tn">TN</span> −1.

Intuiciones rápidas sobre efectividad (aproximaciones):
- <span class="rpg-token token-d6">d6</span> vs TN6 ≈ 17%; <span class="rpg-token token-d8">d8</span> vs 6 ≈ 38%; <span class="rpg-token token-d10">d10</span> vs 6 ≈ 50%; <span class="rpg-token token-d12">d12</span> vs 6 ≈ 58%.
- <span class="rpg-token token-d10">d10</span> vs TN8 ≈ 30%; <span class="rpg-token token-d12">d12</span> vs 8 ≈ 42%; <span class="rpg-token token-d20">d20</span> vs 12 ≈ 45%.
Usa estos números como referencia, no cuentes en tiempo real.

Cuándo no lanzar:
- Cuando el resultado es obvio y no hay apuestas.
- Cuando la tirada no cambiará nada (mejor pasar al siguiente desafío).



---

### 1 en los huesos

- **1 en los dados**: fracaso + complicación. Ejemplos: ruido, pérdida de tiempo, pista falsa, herida leve (−1 Corazón), recurso perdido, peor posición.
- **Fracaso (resultado < <span class="rpg-token token-tn">TN</span>)**: falta de efecto y posible "represalia" (en combate) o avance de la amenaza (fuera de combate).
- **Éxito excepcional (máximo en los dados)**: éxito + beneficio adicional: más rápido/silencioso/sin costo/mayor efecto.

Lista de verificación para crear complicaciones:
1) Golpea un recurso (tiempo, posición, corazones, maná, equipo).
2) Cambia la disposición en el tablero (nuevos obstáculos, caminos cortados, escudos reforzados).
3) Aumenta la presión (contador, alarma, refuerzo de enemigos).



---

### Ruch:

- **Movimiento:** hasta 5 casillas por turno; se permite diagonalmente.
- **Cobertura:** parcial → ataques a distancia <span class="rpg-token token-tn">TN</span> +1; total → sin línea de visión.
- **Terreno difícil (opcional):** entrar en una casilla cuesta 2 de 5 puntos de movimiento.
- **Empujar/mover:** prueba de S vs <span class="rpg-token token-tn">TN</span> 6 (modificar según la situación). Éxito: mueve el objetivo 1-2 casillas; excepcional: +1 casilla.
- **Alcances:** considera hasta 10 casillas como "sin penalización"; más allá → <span class="rpg-token token-tn">TN</span> +1. 
La velocidad es más importante que el conteo minucioso — mantén las reglas ligeras.



---

### Kolejność:

- **Orden:** jugadores → oponentes → repetir.
- **Ataque:** cuerpo a cuerpo = S, distancia = Z; <span class="rpg-token token-tn">TN</span> del oponente: matón 6, élite 8, jefe 12.
- **Impacto:** matón cae; élite/jefe recibe 1 Herida (el jefe tiene 3). Éxito excepcional = normalmente 2 Heridas.
- **Fallo:** si el oponente podía alcanzar → el héroe pierde 1 Corazón (venganza). En cobertura/lejos — normalmente sin venganza.

Escalado de presión:
- Muchos matones "en combate" → <span class="rpg-token token-tn">TN</span> +1 o complicación adicional en caso de fallo.
- Cambia el terreno cada turno: aparecen obstáculos, cuellos de botella, oportunidades para ventaja.



---

### 1. Introducción

Construye escenas en 5 pasos:
1) **Objetivo**: para qué sirve la escena (por ejemplo, un paso, conseguir un objeto, desactivar una amenaza).
2) **Obstáculos**: 2-3 tipos diferentes (guardias, cerraduras, alarmas, terrenos peligrosos).
3) **Amenaza**: secuaces/elites/jefe, peligros, trampas.
4) **Contador (opcional)**: 3-5 pasos; los fracasos lo mueven; al final, una consecuencia negativa.
5) **Recompensa/Consecuencia**: qué se obtiene con el éxito, qué cambia con el fracaso.

Umbrales de tamaño de enfrentamiento (para 3-5 héroes):
- **Fácil:** 3-5 secuaces o elite sin apoyo.
- **Estándar:** 6-8 secuaces o elite + 2-4 secuaces.
- **Difícil:** jefe + 2-4 secuaces o 2 elites + 3-5 secuaces.
- **Heroico:** jefe + 4-6 secuaces y/o elite.
Ajusta a la mesa: el terreno y las coberturas tienen un gran impacto.



---

### 1. Introducción

Formato (ejemplo, sin clima):
> **Nombre — <span class="rpg-token token-tn">TN</span>, Heridas, Táctica, Especial**
- **Peón:** <span class="rpg-token token-tn">TN</span> 6, sin Heridas; táctica simple.
- **Élite:** <span class="rpg-token token-tn">TN</span> 8, 2 Heridas; tiene una clara ventaja (por ejemplo, movilidad, cobertura, control del campo).
- **Jefe:** <span class="rpg-token token-tn">TN</span> 12, 3 Heridas; 1–2 movimientos únicos (por ejemplo, empujar, invocar apoyo).

Reacción y moral (sistema ligero):
- Cuando caiga el primer peón o la élite reciba una Herida, tira **<span class="rpg-token token-d6">d6</span>**:
  - 1–2: retirada/emboscada; 3–4: mantienen la posición; 5–6: atacan.
- Modifica ±1 por ventaja/miedo/jefe cerca.



---

### 1. Introducción

Magia es "efectos especiales". Asigna <span class="rpg-token token-tn">TN</span> y costo de Maná según la escala:
- **Truco:** <span class="rpg-token token-tn">TN</span> 4, costo 0–1 (efecto corto, pequeño).
- **Estándar:** <span class="rpg-token token-tn">TN</span> 6, costo 1 (objetivo único, salto corto, barrera).
- **Fuerte:** <span class="rpg-token token-tn">TN</span> 8, costo 2 (área, control, curación +2 Corazones).
- **Gran poder:** <span class="rpg-token token-tn">TN</span> 12, costo 3 (efecto escénico).

Reglas auxiliares:
- **Múltiples objetivos:** o +1 costo de Maná, o <span class="rpg-token token-tn">TN</span> +1 grado.
- **Mantenimiento del efecto:** paga 1 Maná cada turno o ocupa una Acción.
- **Contraataque/esquivar hechizo:** permite realizar la prueba correspondiente del héroe (Z o M) contra la misma <span class="rpg-token token-tn">TN</span>, para reducir o evitar el efecto (dependiendo de la ficción).



---

### 7.2 Asesinato encubierto/silencio: establece el "nivel de alarma" como **contador 3-5

- **Asesinato/sustracción:** establece el "nivel de alarma" como **contador 3–5**; los fracasos lo aumentan; al alcanzar el máximo, aparece una patrulla, la cerradura se asegura, etc.
- **Persecución:** determina la distancia en "pasos de persecución" (por ejemplo, 3). Cada turno: ambas partes hacen una prueba; el éxito del perseguidor acorta la distancia, el del fugitivo la alarga. Cuando llegue a 0 → captura; al llegar a 5 → escape.
- **Obstáculos ambientales:** comunica claramente el costo del riesgo (por ejemplo, caída = −1 Corazón y peor posición), el <span class="rpg-token token-tn">TN</span> depende de las descripciones.



---

### Desarrollo:

- **Desarrollo:** después de la aventura, cada uno elige una opción: aumentar el tamaño de la característica de la habilidad, +1 Corazón (máx 7) o +1 Mana (máx 5).
- **Recompensas materiales:** otorgan "permisos" (nuevas acciones) o ventajas únicas ("una vez por escena, reduce la <span class="rpg-token token-tn">TN</span> en 1"). Evita modificadores permanentes.
- **Economía (opcional):** umbrales simples: barato/estándar/caro — resuelve con una prueba de recursos en lugar de contar moneda.



---

### 1. Introducción

- Establece con los jugadores el rango de contenido (qué está bien, qué evitamos).
- Acuerda una señal simple de "alto"/"rebobinar" para situaciones incómodas.
- Resuelve los conflictos en la ficción, no en la mesa.



---

### 1. Introducción

1) **Hak:** un problema en una sola frase.
2) **3 lugares** con características tácticas (cubiertas, alturas, pasajes estrechos).
3) **3 obstáculos:** castillo, guardia, amenaza ambiental.
4) **Recursos en juego:** tiempo, ruido, atención del oponente.
5) **Lista de complicaciones** (5 unidades) y **contador** para la escena.
6) **Oponentes:** entradas de 1 línea (peones/elites/jefe) + táctica simple.



---

### 1. Introducción

Komplikaciones — <span class="rpg-token token-d6">d6</span> (universales):
1. Pérdida de tiempo / ventaja del oponente.
2. Revelación de la posición / aumento de la alarma.
3. Daño menor: −1 Corazón o recurso.
4. Mala posición: empujón/atasco.
5. Pérdida/atrapamiento de equipo.
6. Una nueva amenaza aparece en la escena.

Beneficios por éxito excepcional — <span class="rpg-token token-d6">d6</span>:
1. Más rápido.
2. Más silencioso.
3. Sin costo (por ejemplo, sin Maná/sin represalias).
4. Mayor efecto (área/rango).
5. Mejor posición de los aliados.
6. Pista/información adicional.



---

### Cel de los jugadores

- Objetivo de los jugadores: pasar a través de la entrada asegurada.
- MJ: cerradura (<span class="rpg-token token-tn">TN</span> 6), patrulla (contador 3), pasaje estrecho (cubiertas).
1) Jugador A: "Abro la cerradura" (Z, <span class="rpg-token token-tn">TN</span> 6). Fallo = +1 al contador. Tirada 5 → fallo, contador 1/3.
2) Jugador B ayuda (aumenta el dado). A: nuevamente (nuevas herramientas, mejor posición), tirada <span class="rpg-token token-d12">d12</span>=9 → éxito.
3) La patrulla se acerca (contador 2/3). Jugador C cubre la salida (S, <span class="rpg-token token-tn">TN</span> 6). Éxito excepcional → ventaja de posición para el grupo.
Escena resuelta rápidamente, con apuestas claras.

---
Esto es todo lo que necesitas para dirigir. El resto (mundo, monstruos, tesoros) es modular y debe adaptarse al universo elegido.

