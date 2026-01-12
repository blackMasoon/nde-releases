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
generated_at: "2026-01-12T20:14:22.159Z"
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
# Monsterhandbuch

Automatic translation placeholder for de

---



---

### 1. Einleitung

- Wir verwenden dieselben Begriffe wie in den grundlegenden Regeln und im MG-Handbuch.
- **Nur die Spieler würfeln.** Gegner üben Druck durch <span class="rpg-token token-tn">TN</span> und Bewegungen aus; Schäden resultieren normalerweise aus „Vergeltung“ oder Tests, die den Spielern aufgezwungen werden.



---

### 1. Einleitung

> Name — Klasse, <span class="rpg-token token-tn">TN</span>, Wunden, Rolle, Bewegung, Spezial

- **Klasse:** Pachołek | Elite | Boss
- **<span class="rpg-token token-tn">TN</span>:** Zahl 4/6/8/12, die die Schwierigkeit des Treffens/Umgehens des Gegners angibt.
- **Wunden:** nur für Elite und Boss (Elite: 2, Boss: 3 standardmäßig). Pachołek hat keine Wunden (fällt nach einem Treffer).
- **Rolle:** Brute (Nahkampf), Skirmisher (mobil), Artillerie (Fernkampf), Controller (Gebietsbeherrschung), Support (Unterstützung).
- **Bewegung:** standardmäßig 5 Felder. Ändere es, wenn die Mobilität einzigartig ist (z.B. 6 Schnell, Fliegen, Sprung 3).
- **Spezial:** 1–2 kurze beschreibende Fähigkeiten (siehe Abschnitte „Eigenschaften“ und „Bewegungen“).

Beispiel für die Aufzeichnung: „Elite Wächter — Elite, <span class="rpg-token token-tn">TN</span> 8, Wunden 2, Brute, Bewegung 5, Spezial: Schwere Deckung; Druck”.



---

### Pachołek (Minion):

- **Pachołek (Minion):** <span class="rpg-token token-tn">TN</span> 6, fällt nach 1 Treffer. In großer Anzahl erzeugen sie Druck. Vergeltung bei einem Fehlschuss: −1 Herz.
- **Elita:** <span class="rpg-token token-tn">TN</span> 8, 2 Wunden. Hat normalerweise 1 defensive Eigenschaft oder Mobilität. Vergeltung bei einem Fehlschuss: −1 Herz; manchmal zusätzlicher situativer Effekt.
- **Boss:** <span class="rpg-token token-tn">TN</span> 12, 3 Wunden. Hat 2–3 Spezialbewegungen und beeinflusst das Terrain/Tempo. Kann Tests bei den Spielern auslösen (z. B. Ausweichen, Stabilisierung).



---

### Brutale (Nahkampf):

- **Brute (Nahkampf):** drängt im Nahkampf, stößt aus Deckung heraus.
- **Skirmisher (mobil):** geht in Kontakt und verlässt ihn, bestraft Einsamkeit.
- **Artillery (Fernkampf):** schießt aus Deckung, zwingt zur Bewegung.
- **Controller (Kontrolle):** schafft Gefahrenzonen, Rauch, abstoßende Felder.
- **Support (Unterstützung):** stärkt Verbündete, senkt die <span class="rpg-token token-tn">TN</span> von Verbündeten oder hebt situativ die <span class="rpg-token token-tn">TN</span> von Helden um 1 Stufe.



---

### 1. Einleitung

Füge 1–2 zum Statblock hinzu. Sie wirken immer beschreibend; sie ändern die <span class="rpg-token token-tn">TN</span> nur um 1 Grad, wenn es sinnvoll ist.
- **Natürliche Deckung:** In Reichweite hat der Gegner normalerweise eine partielle Deckung (Angriff auf ihn → <span class="rpg-token token-tn">TN</span> +1 Grad).
- **Leichte Rüstung:** Der erste Verlust von 1 Herz durch Vergeltung gegen diese Einheit in der Szene wird ignoriert.
- **Hart:** Der erste Erfolg gegen diese Einheit fügt keinen Schaden zu (nur zurückstoßen/Position) — gut für Bosse.
- **Schnell (Bewegung 6):** Ignoriert 1 Feld schwieriges Terrain pro Runde.
- **Kletterer/Springer:** Bewegt sich vertikal/über Hindernisse wie auf flachem Boden, Sprung von 3 Feldern.
- **Fliegen:** Ignoriert Gelände-Hindernisse (der SL sorgt für sinnvolle Deckungen).
- **Späher:** Es ist schwieriger, ihn zu überraschen; der erste Versuch, sich gegen ihn zu schleichen, hat <span class="rpg-token token-tn">TN</span> +1.
- **Widerstand [Typ]:** Der erste Effekt eines bestimmten Typs in der Szene wird reduziert (der SL erklärt: schwächerer Bereich, kürzere Dauer).
- **Empfindlichkeit [Typ]:** Gegen diesen Typ von Angriffen ist die <span class="rpg-token token-tn">TN</span> um 1 Grad niedriger.
- **Schwärme:** Wenn er neben dem Ziel steht, kann die Vergeltung bei einem Fehlschuss zwei Helden im Bereich von 1 treffen.



---

### 1. Einleitung

Wählen Sie 1–2 charakteristische Bewegungen. Die Bewegungen beschreiben den Effekt; wenn sie den Helden drohen, kann der SL sie auffordern, einen entsprechenden Test (Z oder M) gegen die <span class="rpg-token token-tn">TN</span> des Gegners abzulegen.
- **Druck (Brute):** nach einem Treffer des Helden, zusätzlich um 1–2 Felder verschieben.
- **Durchbrechen der Deckung:** wenn diese Einheit trifft, hört die Deckung des Ziels bis zum Ende der nächsten Runde auf zu wirken.
- **Zerren (Skirmisher):** das Betreten/Verlassen des Nahkampfs provoziert keinen Gegenschlag.
- **Salve (Artillery):** Bereich 3×3; alle im Bereich machen einen Z-Test gegen <span class="rpg-token token-tn">TN</span>; Misserfolg: −1 Herz und werden um 1 Feld zurückgestoßen.
- **Anker (Controller):** das Feld 3×3 wird zu „schlüpfrigem Terrain“ (das Betreten kostet die gesamte Aktion) bis zum Ende der nächsten Runde.
- **Verstärkung (Support):** ein Verbündeter hat bis zum Ende der Runde um 1 Grad erleichtert (Angreifende auf ihn haben <span class="rpg-token token-tn">TN</span> +1).
- **Beschwörung (Boss):** einmal zu Beginn beschwört er 2 Handlanger in freien Feldern.
- **Barriere (Boss):** bis zum Ende der Runde der göttlichen Seite führen die Helden Fernangriffe gegen <span class="rpg-token token-tn">TN</span> +1 aus.
- **Erschütterung (Boss):** alle im Bereich von 2 Feldern machen einen S-Test gegen <span class="rpg-token token-tn">TN</span>; Misserfolg: −1 Herz oder Umwerfen (du verlierst die Bewegung in dieser Runde).



---

### 1. Einleitung

1) **Wähle eine Klasse:** Fußsoldat / Elite (2 Wunden) / Boss (3 Wunden).
2) **Setze <span class="rpg-token token-tn">TN</span>:** 6 / 8 / 12 (ausnahmsweise 4 für sehr schwache oder 10 für harte Eliten).
3) **Verleihe eine Rolle:** Brute, Skirmisher, Artillerie, Controller, Unterstützung.
4) **Füge 1–2 Eigenschaften** und **1 Spezialbewegung** hinzu (Boss: 2–3 Bewegungen).
5) **Bewegung:** normalerweise 5; ändere nur, wenn es entscheidend ist.

Fertig. Dieses Gerüst funktioniert in allen Realitäten.



---

### 1. Einleitung

7.2 Weltfarben und -namen ersetzen

### 7.1 Pachołki
- **Wächter Pachołek — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Brute, Bewegung 5, Spezial: Natürlicher Schutz.**
- **Späher Pachołek — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Skirmisher, Bewegung 6, Spezial: Späher.**
- **Schütze Pachołek — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Artillerie, Bewegung 5, Spezial: Salve (kleines Gebiet 2×2, warnt nur: bei Misserfolg −1 Herz).**
- **Kontrolleur Pachołek — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Controller, Bewegung 5, Spezial: Anker (für 1 Runde, einmalig).**
- **Unterstützung Pachołek — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Support, Bewegung 5, Spezial: Verstärkung (einmal pro Szene).**

### 7.2 Eliten
- **Elitärer Wächter — Elite, <span class="rpg-token token-tn">TN</span> 8, Wunden 2, Brute, Bewegung 5, Spezial: Leichte Rüstung; Druck.**
- **Elitärer Attentäter — Elite, <span class="rpg-token token-tn">TN</span> 8, Wunden 2, Skirmisher, Bewegung 6, Spezial: Zerren; Verwundbarkeit [Beobachtung] (leichter zu entdecken).**
- **Elitärer Scharfschütze — Elite, <span class="rpg-token token-tn">TN</span> 8, Wunden 2, Artillerie, Bewegung 5, Spezial: Natürlicher Schutz; Salve (3×3 nach Vorbereitung).**
- **Elitärer Kontrolleur — Elite, <span class="rpg-token token-tn">TN</span> 8, Wunden 2, Controller, Bewegung 5, Spezial: Anker; 1 Feld zurückstoßen bei außergewöhnlichem Erfolg.**
- **Elitärer Medic — Elite, <span class="rpg-token token-tn">TN</span> 8, Wunden 2, Unterstützung, Bewegung 5, Spezial: Verstärkung; bei einem Treffer wird 1 Komplikation eines Verbündeten zurückgenommen (beschreibend).**

### 7.3 Bosse
- **Anführer — Boss, <span class="rpg-token token-tn">TN</span> 12, Wunden 3, Unterstützung, Bewegung 5, Spezial: Beschwörung; Verstärkung; Barriere.**
- **Koloss — Boss, <span class="rpg-token token-tn">TN</span> 12, Wunden 3, Brute, Bewegung 5, Spezial: Druck (bis zu 2 Felder); Hart; Schlag.**
- **Jäger — Boss, <span class="rpg-token token-tn">TN</span> 12, Wunden 3, Skirmisher, Bewegung 6, Spezial: Zerren; Späher; Salve (Sprung — nach Bewegung).**
- **Taktiker — Boss, <span class="rpg-token token-tn">TN</span> 12, Wunden 3, Controller, Bewegung 5, Spezial: Anker (Halten für 1 Mana/Ressource pro Runde); Barriere; Beschwörung (1 Diener/Runde bis maximal 3).**



---

### 1. Einleitung

Gefahr ist ein „dummes Gegner” oder ein Umwelteffekt. Wirkt rundenweise oder auf Auslöser.
Format: **Name — <span class="rpg-token token-tn">TN</span>, Effekt, Wie man es deaktiviert**
- **Turm — <span class="rpg-token token-tn">TN</span> 8, Effekt: bei der Runde der Gegner jeder in der Schusslinie Test Z vs <span class="rpg-token token-tn">TN</span>, Misserfolg: −1 Herz; Deaktivierung: Test M oder Z <span class="rpg-token token-tn">TN</span> 8 am Panel.**
- **Falle — <span class="rpg-token token-tn">TN</span> 6, Effekt: Betreten des Feldes zwingt zu einem Test Z; Misserfolg: Lähmung oder −1 Herz; Deaktivierung: Z <span class="rpg-token token-tn">TN</span> 6 mit Werkzeugen.**
- **Abstoßfeld — <span class="rpg-token token-tn">TN</span> 8, Effekt: zu Beginn der Runde bewegt sich um 2 Felder in Richtung Rand; Deaktivierung: M <span class="rpg-token token-tn">TN</span> 8 (Streuung) oder Stromabschaltung (S <span class="rpg-token token-tn">TN</span> 6).**
- **Gas/Rauch — <span class="rpg-token token-tn">TN</span> 6, Effekt: im Bereich 3×3 Test M oder Z; Misserfolg: blinder Fleck/−1 Herz; Deaktivierung: Lüften (S) oder Abdichten (Z).**



---

### 1. Einführung

Wähle 1 aus jeder Zeile (oder würfle [token:<span class="rpg-token token-d6">d6</span>]):
1. Ziel der Szene: Übergang / Wiedererlangung / Deaktivierung / Eskorte / Diebstahl / Verteidigung
2. Führendes Terrain: offen / enge Korridore / mehrstöckig / modulare Deckungen / gefährliche Kanten / Nebel-Rauch
3. Gegner: 6× Wache / 4× Wache + Elite / 2× Elite / Boss / Boss + 2× Wache / Elite + Risiko
4. Vorteil des Gegners: Deckung / Höhe / Mobilität / Zeitlimit / Engpässe / Fernunterstützung
5. Vorteil der Spieler: Überraschung / höheres Niveau / Werkzeuge / kurze Barriere / Abkürzung / neutraler Verbündeter



---

### 1. Einleitung

Statt numerischer <span class="rpg-token token-tn">TN</span> verwende Grade:
- **Pion:** „Normal” (entspricht <span class="rpg-token token-tn">TN</span> 6)
- **Elite:** „Schwierig” (+1 Grad)
- **Boss:** „Heldentat” (+2 Grade) und 3 Wunden
Eigenschaften und Bewegungen funktionieren gleich; wenn „<span class="rpg-token token-tn">TN</span> +1” in der Beschreibung steht, erhöhe den Grad.



---

### 7.2 Wenn der Kampf zu kurz dauert

- Wenn der Kampf zu kurz dauert: Füge Wellen von Handlangern hinzu (2 pro Runde) oder erhöhe den Schwierigkeitsgrad um 1 Stufe zugunsten der Gegner, die einen Positionsvorteil haben.
- Wenn der Kampf sich hinzieht: Erlaube außergewöhnlichen Erfolg häufiger, indem du Gelegenheiten schaffst (bessere Position) oder senke den Schwierigkeitsgrad für geschwächte Feinde.
- Zwei Eliten ≈ kleiner Boss; Boss + 4 Handlanger ≈ das finale Duell in einer 2-stündigen Sitzung.



---

### 7.2. Verteidigungstruppe — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Artillerie, Bewegung 5, Spezial: Natürlicher Schutz.

- **Verteidigungstruppe — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Artillerie, Bewegung 5, Spezial: Natürlicher Schutz.**
- **Mobiles Patrouillen — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Scharmützel, Bewegung 6, Spezial: Späher.**
- **Schwerer Sturmangriff — Elite, <span class="rpg-token token-tn">TN</span> 8, Wunden 2, Brut, Bewegung 5, Spezial: Leichte Rüstung; Druck.**
- **Feldtaktiker — Elite, <span class="rpg-token token-tn">TN</span> 8, Wunden 2, Controller, Bewegung 5, Spezial: Anker; Verstärkung.**
- **Feldführer — Boss, <span class="rpg-token token-tn">TN</span> 12, Wunden 3, Unterstützung, Bewegung 5, Spezial: Beschwörung; Barriere; Verstärkung.**
- **Territorialer Koloss — Boss, <span class="rpg-token token-tn">TN</span> 12, Wunden 3, Brut, Bewegung 5, Spezial: Hart; Stoß; Druck.**

---
Dies ist ein Werkzeugset zur schnellen Erstellung von Gegnern. Bestimmen Sie <span class="rpg-token token-tn">TN</span>, wählen Sie Klasse und Rolle, fügen Sie 1–2 Eigenschaften sowie Bewegung hinzu — und Sie haben einen spielbaren Feind, der bereit für das Spielfeld ist.

