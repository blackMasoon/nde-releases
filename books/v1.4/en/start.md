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
generated_at: "2026-01-15T07:57:22.479Z"
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
# Start (Rules in a Nutshell)



---



---

### 1) Hero in 1 Minute


* **Concept:** who you are and what genre you are playing (1 sentence).
* **Role (choose one):**

  * **Assault** – pressure, combat, overcoming obstacles
  * **Specialist** – sneaking, precision, technique, observation
  * **Adept** – powers, knowledge, influence, improvisation
* **Attributes (3):**

  * **Strength (<span class="rpg-token token-stat">S</span>)** – physical strength, endurance, melee combat
  * **Agility (A)** – reflexes, sneaking, shooting, piloting
  * **Might (<span class="rpg-token token-stat">M</span>)** – magic/psionics/technology/bluff/intuition (depending on the world)
* **Attribute Dice:** one attribute **<span class="rpg-token token-d12">d12</span>**, one **<span class="rpg-token token-d8">d8</span>**, one **<span class="rpg-token token-d6">d6</span>** (choose according to your role).
* **Hearts:** 5. **<span class="rpg-token token-power">Power</span> Points:** 3 (spend on powers and "special moves").
Below you have a ready-made snippet to paste (variant A), in the style of short rules "1-page".

**<span class="rpg-token token-luck">Luck</span> Roll (how it works):** spend **1 <span class="rpg-token token-luck">Luck</span> Point**, to choose one:

* **Reroll** your test (keep the better result), or
* **Increase the die by 1 step** for this one roll (**<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>**), or
* **Turn a failure into a "success at a cost"** — the action succeeds, but the GM immediately adds a price (e.g., you lose time, make noise, expend a resource, end up in a worse position, attract attention, damage equipment).

**Recovering <span class="rpg-token token-luck">Luck</span> Points:** at the beginning of the next session, you return to the limit. The GM may grant **+1 <span class="rpg-token token-luck">Luck</span> Point** for bold risks, great narrative decisions, or playing consequences.

* **Equipment:** 1 "key" tool (e.g., sword, rifle, hacking kit), 1 protection (armor, energy shield, camouflage), 3 trinkets fitting the concept.

**Example:** Specialist: <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d12">d12</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">d8</span>, A <span class="rpg-token token-d6">d6</span>. In cyberpunk, <span class="rpg-token token-stat">M</span> is "Hacking/Influence"; in fantasy, <span class="rpg-token token-stat">M</span> is "Magic/Will".



---

### 2) How to Resolve Actions

1. The player states **what they do** and **how** (description in the game world).
2. The Game Master determines the **Difficulty** and the stakes ("what happens on failure").
3. Roll the attribute die (<span class="rpg-token token-stat">S</span>/<span class="rpg-token token-stat">Z</span>/<span class="rpg-token token-stat">M</span>) and compare it to the Difficulty.

**Difficulty (D):**

* **3** easy, **4** standard, **5** hard, **6** very hard, **8** heroic, **12** legendary.

**Roll Result:**

* **1** – failure with consequence (a complication definitely arises).
* **< D** – failure (but the scene continues: loss of time, noise, worse position, loss of resource).
* **≥ D** – success.
* **Max on the die** (e.g., 12 on a <span class="rpg-token token-d12">d12</span>, 20 on a <span class="rpg-token token-d20">d20</span>) – exceptional success: you gain an additional benefit.

**Modifiers without counting:**

* **Better situation**: increase the die by 1 step (<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>).
* **Worse situation**: decrease the die by 1 step (<span class="rpg-token token-d20">d20</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d4">d4</span>).
* **Ally's help** (costs their action): increase the die by 1 step.

**Example:** The Adept tries to close the portal (<span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">d8</span>) under alarm and stress → worse situation, drops to <span class="rpg-token token-d6">d6</span>. D = 5. Roll 6: success, but the "alarm" remains in the background as narrative pressure.



---

### 3) Movement and Combat – Default without Grid, Grid as an Option

**Default: theatre of mind (recommended)**

* Describe distances as: **Close** (within reach), **Nearby** (a few steps), **Far** (the other side of the stage), **Very Far** (sniper/vehicle).
* In a turn, you have: **Movement + 1 Action**.

  * Movement usually changes the distance by 1 "degree" (Nearby→Close, etc.).
* **Attack**: roll **<span class="rpg-token token-stat">M</span>** (melee) or **R** (ranged) against the target's **Defense**.

**Defense of opponents (approximate):**

* **Weak** 4, **Typical** 5, **Elite** 6, **Boss** 8 (legendary boss 12).

**Effects of a Hit (quick combat):**

* A hit deals **1 Heart**.
* A critical success deals **2 Hearts** or provides a strong effect (disarm, knockdown, distraction).

**Cover and Positional Advantage:**

* Light cover / poor angle: lower the attacker's die by 1 degree.
* Good position / surprise: raise the die by 1 degree.

**Option: play on a grid**

* 1 square = 1–2 m. Movement in a turn: **up to 5 squares**. The rest of the rules remain unchanged.

**Example:** A specialist shoots from cover (R <span class="rpg-token token-d12">d12</span>) at an elite (Defense 6). The target is in light cover → R drops to <span class="rpg-token token-d8">d8</span>. Roll 7: success, 1 Heart of damage.



---

### 4) Powers, 'Spells' and Special Maneuvers (Universal)

This includes magic, psionics, cybernetics, gadgets, film tricks – depending on the world.

* When you do something **above standard**: spend **<span class="rpg-token token-power">Power</span> Point** and roll **<span class="rpg-token token-stat">M</span>**.
* Determine the level of effect:

**<span class="rpg-token token-power">Power</span> Levels (T / cost):**

* **Trick** (short effect, trick, "flash"): **T 4 / 0–1 PP**
* **Standard** (attack, shield, impulse, minor control): **T 5 / 1 PP**
* **Strong** (area, healing, paralysis, live hack): **T 6 / 2 PP**
* **Great** (scene change, powerful intervention): **T 8–12 / 3 PP**

**Failure:** PP is lost, and the consequence is immediate (overload, digital trace, crack in the ritual, unwanted attention).

**Recovery:** after the conflict scene, you regain **1 PP**, after a safe rest – to full.

**Example:** In a space opera, the Adept tries to "bend the sensor" of a drone: Standard, T 5, cost 1 PP. Roll <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span> = 8: exceptional success – the drone loses signal and goes off track.



---

### 5) Fall, Risk, and Healing

* When you fall to **0 Hearts**, you are **out of action** (injured, stunned, in shock – according to the convention).
* An ally can spend an action to bring you back to **1 Heart** (first aid, adrenaline, system reboot).
* After the scene, if you have a moment to catch your breath: you return to **full Hearts**, provided you have the conditions (shelter, bandage, service, meal).
* If the scene was particularly brutal or the enemies have the upper hand, the Game Master may require that a "full reset" necessitates a safe stop.

**Example:** Storm falls to 0. The specialist pulls him behind cover and spends an action: Storm returns to 1 Heart and can act in the next turn.



---

### 6) Character Development (campaign without tables and bookkeeping)


After the adventure, choose **one**:

* **Increase** one attribute by 1 step (max. to <span class="rpg-token token-d20">d20</span>), or
* **+1 Heart** (max. 7), or
* **+1 <span class="rpg-token token-power">Power</span> Point** (max. 5), or
* **New Trait** (a short, one-sentence rule agreed upon with the Game Master).

**Examples of traits (universal):**

* **Pressure:** once per scene, when you hit in melee, you deal +1 Heart of damage.
* **Shadow:** when you act from hiding, you have a die increase of 1 step.
* **Spark:** once per scene, you can spend 1 PP to automatically achieve a "success at a cost" without rolling.

**Example:** The Adept increases <span class="rpg-token token-stat">M</span> from <span class="rpg-token token-d8">d8</span> to <span class="rpg-token token-d12">d12</span> – now his powers stabilize better at T 5–6.



---

### 7) The "only <span class="rpg-token token-d6">d6</span>" variant in **2d6** mode (fast and highly playable)


If you don't have a set of dice or want more "narrative" degrees of success:

* Each test is: **roll 2d6 + ability modifier**.
* **Ability modifiers** are chosen at the start: one ability **+2**, one **+1**, one **+0**.
* Result:

  * **6 or less** – failure with consequence
  * **7–9** – success at a cost (compromise, loss of resource, worse position)
  * **10+** – full success
  * **12** – exceptional success (additional benefit)

**Difficulty of the situation:** instead of changing thresholds, give **+1 / -1** to the roll (helps / hinders) or a cost in case of 7–9.

**Mapping to the dice-ability version (if you want compatibility):**

* <span class="rpg-token token-d6">d6</span> ≈ +0, <span class="rpg-token token-d8">d8</span> ≈ +1, <span class="rpg-token token-d12">d12</span> ≈ +2, <span class="rpg-token token-d20">d20</span> ≈ +3 (for very experienced characters).

**Example:** A specialist shoots while running: <span class="rpg-token token-stat">Z</span> = +2, difficult situation (-1). Roll 2d6 = 8, total 9: success at a cost – hits, but ends up in an exposed position.

