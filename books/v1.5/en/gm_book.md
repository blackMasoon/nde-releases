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
generated_at: "2026-01-16T08:33:24.473Z"
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
# Game Master Book



---



---

### 0) Running Rules in 30 Seconds

- **Start with fiction.** First, describe the situation and the players' actions, then roll.
- **Set the stakes before rolling.** Say: *what's at stake* and *what happens on a failure*.
- **One decision → one roll → meaningful result.** Do not split one intent into 3 tests.
- **Failure drives the game forward.** Do not 'reset' the scene – change it with a complication, cost, or pressure.
- **Maintain consistency.** Same circumstances → similar Difficulty, similar consequences.
- **Grid is optional.** By default, the game operates without a map: "Close / Near / Far / Very far."



---

### 1.1. When to Roll?

A roll makes sense only when simultaneously:
- the outcome is **not obvious**,
- there is a **real stake** (something will change),
- both parties agree that **the mechanics have the right to decide**.

**Do not roll** when:
- the action is routine and without pressure,
- failure will not add anything interesting,
- success is certain and the cost has already been paid (e.g., players have time, tools, and security).

**Example (no roll):** The specialist has administrative access and calm conditions – opening standard doors in the base does not require a test.
**Example (with a roll):** The same doors, but the alarm is active, and a patrol is approaching in 30 seconds – this is a test because the stake is time and exposure.

### 1.2. Resolution Checklist (Table Procedure)

1) The player states: **what they do** and **what they want to achieve**.  
2) You respond with: **what stands in the way** and **what the stakes are**.  
3) Choose an attribute: **Strength (<span class="rpg-token token-stat">S</span>)** / **Dexterity (<span class="rpg-token token-stat">Z</span>)** / **<span class="rpg-token token-power">Power</span> (<span class="rpg-token token-stat">M</span>)**.  
4) Determine **Difficulty (T)** or **Defense** (in combat).  
5) Establish the situational modifier: **boost/lower the dice** and possible **assistance**.  
6) Roll → result → consequence → update the scene.

Shortcut: **Description → Stakes → Attribute → T/Defense → Roll → Consequence**.

---

### 1.3. Difficulty (D): Scale and Practical Rules

Use a single scale throughout the game. This builds players' trust in the GM's decisions.

- **D 3 – easy:** favorable conditions, no pressure, minimal resistance.  
- **D 4 – standard:** "normal job" in the adventure.  
- **D 5 – difficult:** time pressure, risk, opponent, narrow window.  
- **D 6 – very difficult:** clear enemy advantage, high risk, complex action under stress.  
- **D 8 – heroic:** above-average achievement; usually requires an advantage, plan, or resource.  
- **D 12 – legendary:** "wow" moment; rarely without preparation and often at a high cost.

**Practical rule:** if you don't know what to set – start at **D 4** and then justify "up" or "down".

### 1.4. Modifiers Without Calculations: Boost/Lower the Die

Instead of adding bonuses and penalties, in NDE you change the **size of the die** for one test.

- **Better situation:** boost the die by 1 step  
  <span class="rpg-token token-<span class="rpg-token token-d4">d4</span>"><span class="rpg-token token-d4">d4</span></span>→<span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">d8</span>"><span class="rpg-token token-d8">d8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">d12</span>"><span class="rpg-token token-d12">d12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d20">d20</span>"><span class="rpg-token token-d20">d20</span></span>
- **Worse situation:** lower the die by 1 step (in the opposite direction).

**Ally's help:** costs their action and provides a **boost of the die by 1 step** for the given test.

**Example:** Lock in silence (D 4) vs. lock in rain and under fire (D 5 + lowering the die, because of trembling hands and lack of visibility).
This usually works better than “D 6 and +2 and -1.”

### 1.5. Test Results: Success, Failure, and Game Pace

- **1 on the die:** failure + complication (complication definitely occurs).  
- **Result < T:** failure (but the situation changes).  
- **Result ≥ T:** success.  
- **Maximum result on the die:** exceptional success (additional benefit).

#### How to design failure so it doesn't block the game?

Before the player rolls, establish 1–2 types of cost:
- **time** (someone gets there, something closes),
- **position** (worse positioning, exposed),
- **resource** (equipment, ammunition, energy, <span class="rpg-token token-power">Power</span> Point),
- **attention** (alarm, suspicion, track).

**Example (fail-forward):**  
The player wants to force open the door. Failure doesn't mean "you don't open it."  
Failure means: "you open it, but make noise – the patrol is now nearby, and the alarm level increases."



---

### 2) A Stroke of <span class="rpg-token token-luck">Luck</span> (Ł<span class="rpg-token token-stat">S</span>): How to Support Drama without Ruining the Game

Each hero starts a session with **2 Ł<span class="rpg-token token-stat">S</span>**. It is a tool for the players, but the GM is responsible for its 'economy' at the table.

### 2.1. What do players spend Ł<span class="rpg-token token-stat">S</span> on?

Spend 1 Ł<span class="rpg-token token-stat">S</span> to:
- perform a **reroll** (keep the better result),
- **upgrade a die by 1 step** for one roll,
- change a failure into a **success with a cost** (the GM adds a price).

### 2.2. When to Award Additional Ł<span class="rpg-token token-stat">S</span>?

The GM can award **+1 Ł<span class="rpg-token token-stat">S</span>** for:
- consciously taking risks that drive the scene,
- accepting consequences without "negotiating",
- creative solutions consistent with the convention,
- very good role-playing of relationships, motivation, or stakes.

**Hygiene rule:** award sparingly (1-2 per session per person in extremely generous games). Ł<span class="rpg-token token-stat">S</span> should be a "spark," not a constant fuel.



---

### 3) Conflict and Combat

NDE should fight quickly. If a battle lasts 60 minutes, it almost always means: too many enemies 'on <span class="rpg-token token-heart">HP</span>' or too many small rolls.

### 3.1. Default Without a Map: Stage Distances

Use four distances:
- **Close** – within arm's reach (melee),
- **Nearby** – a few steps away,
- **Far** – the other side of the stage,
- **Very Far** – sniper/vehicle range.

In a turn, a character has: **Movement + 1 Action**.  
Movement typically changes the distance by **1 degree** (Nearby→Close).

**Example:** A warrior is Nearby. In the turn: they run up (Close) and attack.

### 3.2. Option: grid – when you need precision

If you are playing on a grid:
- movement per turn: **up to 5 squares**,
- diagonals allowed,
- difficult terrain may cost "2 squares per entry" (optional).

All other rules remain identical.

### 3.3. Opponent Defense and Damage

In combat, instead of Difficulty, you use **Defense** (a kind of "D for combat").

**Defense (approximately):**
- **Weak** 4
- **Typical** 5
- **Elite** 6
- **Boss** 8 (legendary boss 12)

**Attack:** roll **Strength** (melee) or **Dexterity** (ranged) against Defense.

**Damage (pace):**
- a hit deals **1 Heart**,
- an extraordinary success deals **2 Hearts** or provides a strong effect (disarm, knockdown, disruption, distract).

**Minions and elites (recommended model):**
- **Minion:** 1 hit = removed from battle (defeated, flees, incapacitated).
- **Elite:** has **2 Hearts** (or "2 hits"), often has one tactical advantage.
- **Boss:** has **3 Hearts** + 1–2 "boss moves" (see 3.6).

This allows for quick encounters without counting points.

### 3.4. Cover, Advantage, and “Clear Terrain”

Instead of multiplying rules, use a single language: **boost the die / lower the die**.

- Light cover, smoke, poor angle: **lower the attacker's die** by 1 step. 
- Good position, surprise, height advantage: **boost the die** by 1 step. 
- Full cover: attack is impossible until the situation changes.

**Example:** A sniper in a window is 'Far' and has a height advantage → the attacker gets a die reduction.
The team changes the scene: smoke grenade, flanking, circumventing – and the advantage disappears.

### 3.5. Order in Combat Without Counting Initiative

Recommended quick scheme:
1) **Players take actions** (in any order around the table).
2) **Opponents take actions**.
3) Repeat.

This allows players to plan short combinations without burdening the table with initiative.

### 3.6. How to Make a Boss Interesting (and Not Just a 'Damage Sponge')

A boss in NDE should have:
- **Defense 8** (or 12 in the 'season finale' version),
- **3 Hearts**,
- **1–2 unique moves** that change the scene.

**Example Boss Moves (Universal):**
- **Push Back:** anyone hit moves back by 1 distance (Close→Far) and loses position.
- **Shield Break:** the boss destroys a shield or forces someone out of hiding.
- **Call for Reinforcements:** 2 minions or one elite join the fray (best used once per fight).
- **Danger Zone:** an area becomes hazardous (fire, electricity, runes) – anyone who stays risks a test.

**Rule:** a boss's move should change the game field, not just 'deal more damage.'


### 3.7. Morale and Enemy Behavior (Light Procedure)

When:
- the first minion falls, or
- an elite loses the first Heart, or
- a boss loses the second Heart,

roll a <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span> and decide:
- **1–2:** they retreat / seek cover / negotiate,
- **3–4:** they hold their ground,
- **5–6:** they charge aggressively.

Modify by **+1** if they have the advantage, **-1** if they are frightened or cut off.

---



---

### 4) Powers (<span class="rpg-token token-stat">M</span>) from the GM's Side: How to Price Them and How Not to Ruin the Pace

In NDE, '<span class="rpg-token token-power">Power</span>' encompasses magic, psionics, cybernetics, hacking, 'movie-level' charisma – depending on the world.

### 4.1. <span class="rpg-token token-power">Power</span> Scale: Difficulty and <span class="rpg-token token-power">Power</span> Points Cost

- **Trick:** T 4, cost 0–1 PP (small, short effect).
- **Standard:** T 5, cost 1 PP (single target, short jump, shield).
- **Strong:** T 6, cost 2 PP (area, control, healing).
- **Great:** T 8–12, cost 3 PP (scene-changing effect).

**Tip:** if the effect is to "change the rules of the scene" (ice bridge, blackout in a district) - it is a Great <span class="rpg-token token-power">power</span>.

### 4.2. Consequences of <span class="rpg-token token-power">Power</span> Failure

Failure should be specific and immediate:
- loss of <span class="rpg-token token-power">PM</span> (always),
- overload (loss of position, exposure),
- trace (digital/astral),
- side effect in the environment (noise, flash, smell, echo).

**Example:** A live hack during combat. Failure: <span class="rpg-token token-power">PM</span> is lost, and the system logs the intruder – the 'counter-ICE' timer starts.

### 4.3. Defense Against <span class="rpg-token token-power">Power</span>

If the fiction justifies it, allow a "counter-roll":
- **Dexterity** (dodge, reflex) or
- **<span class="rpg-token token-power">Power</span>** (resistance, counter-ritual, barrier).

A counter-roll should not multiply rolls. Use it where it makes the scene more interesting (e.g., paralysis, mind control).



---

### 5.1. Build Scenes in 5 Steps

1) **Scene Objective:** what the team is supposed to achieve (specific goal).  
2) **Obstacles:** 2–3 different types (people, devices, environment).  
3) **Threats:** opponents, hazards, traps, time pressure.  
4) **Counter (optional):** 3–5 spaces; failures move the counter; a major consequence occurs at the end.  
5) **Reward and Consequences:** what changes with success, what changes with failure. 

This is the minimal 'scene engine'—it works in fantasy, sci-fi, and crime genres.

### 5.2. Clocks – Simple Version

A clock consists of 3–5 segments. It fills up when:
- a test ends in failure,
- someone makes noise,
- enemies have time to react.

When the clock fills up, a consequence occurs:
- alarm,
- reinforcements,
- path closure,
- resource loss,
- conflict escalation.

**Example:** "Alarm 0/4". Failure in stealth = +1. Exceptional success = -1 (optional).  
When it reaches 4/4 – a patrol shows up and the doors lock.

### 5.3. How to Determine the 'Scene Difficulty' Without Counting Everything

For a team of 3–5 heroes:

- **Easy:** 3–5 minions or one elite without terrain advantages.  
- **Standard:** 6–8 minions or an elite + 2–4 minions, or environmental hazard.  
- **Difficult:** boss + 2–4 minions, or 2 elites + 3–5 minions, or countdown of 3.  
- **Heroic:** boss + support + terrain pressure + countdown of 3–5.

**Most Important:** terrain and cover often mean more than the number of enemies.



---

### 6.1. Sneaking and Infiltration: "Alarm"

1) Set the counter **Alarm 0/3 to 0/5**. 
2) Each failure = +1 alarm.
3) Players can decrease the alarm through actions (e.g., false signal, sabotage) – these are normal tests.
4) When the maximum is reached, an effect occurs: patrol, locking, lockdown.

**Example:** The team is walking down a corridor. The specialist wants to bypass the cameras (<span class="rpg-token token-stat">M</span>, T 5). Failure = +1 alarm.
Before they roll, they know what they are risking – and that's the key.

### 6.2. Chase: "Chase Distance"

Determine the **Distance** in steps, e.g. **3** (average).  
Each "chase turn":
- the escapee makes a test (based on <span class="rpg-token token-stat">Z</span> or <span class="rpg-token token-stat">M</span> depending on the method),
- the pursuer makes a test,
- a successful escapee increases the distance, a successful pursuer decreases it,
- when the distance drops to **0** – the pursuer catches up,
- when it increases to **5** – the escapee gets away.

Add obstacles (turns, crowds, barricades) as description + dice modifier.

### 6.3. Investigation: "Clues Instead of Test Walls"

Rule: **a key clue cannot be stuck behind a single test**.  
If the investigative scene is to progress, the key clue is available:  
- automatically (if players do something reasonable),  
- or after a test, but failure gives it "with a cost" (time, false lead, alarm).

**Example:** Examining a body. Success: they get the truth. Failure: they get the truth, but the authorities arrive or someone notices them.

### 6.4. Social Conflict: Stakes, Pressure, Consequence

Do not turn the conversation into a 'dice-rolling battle.' Determine: 
- what the NPC wants, 
- what the players want, 
- what the stakes are, 
- how many 'moves' there are until the tipping point (counter 3-5). 

**<span class="rpg-token token-stat">M</span>** tests (influence, bluff, authority) or **<span class="rpg-token token-stat">Z</span>** tests (reading intentions) change the conversation's position. 
Failure incurs a cost (bad impression, loss of resource, time, hostility).



---

### 7.1. Complications on Failure (roll <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span>)

1. Loss of time / someone managed to react.
2. Exposure of position / increased alarm.
3. Minor damage: -1 Heart or resource loss.
4. Bad position: push, fall, exposure.
5. Loss or damage of equipment.
6. A new threat emerges in the scene.

### 7.2. Benefits on Exceptional Success (roll <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span>)

1. Faster (save time or movement).
2. Quieter (no increase in alert level).
3. No cost (e.g., no MP expenditure / no terrain consequences).
4. Greater effect (increased range, additional target).
5. Better ally position (someone gets a dice boost in the next action).
6. Additional clue or narrative advantage.

### 7.3. Quick Enemy Entry (Note Format)

> **Name — Defense, Hearts, Tactics, Trick/Advantage**

- **Minion:** Defense 4–5, 1 hit = disappears.  
- **Elite:** Defense 6, 2 Hearts, one advantage (mobility/counter/cover).  
- **Boss:** Defense 8 (or 12), 3 Hearts, 1–2 boss moves.

**Example (universal):**  
> **Guard — Defense 5, 1 hit, holds the corridor, smoke grenade (once)**

---



---

### 8) Safety and Table Agreement (Minimum)

- Establish what you are not playing (taboo topics) and what you will 'skip over'.
- Agree on a simple signal to interrupt a scene (e.g., 'stop' or 'pause').
- Resolve table conflicts through discussion outside of fiction, not 'rulings in anger'.

This improves the quality of the game more than any mechanics.



---

### 9) Modularity and Community Development: How to Keep It in Check

If you are building an NDE as an 'engine,' the easiest way for the community to develop it is through packages:

- **Genre Package** (fantasy/cyberpunk/horror): mapping of Powers, list of feats, equipment, adversaries, 1–2 procedures (e.g., fear, chase).  
- **Adversary Package:** 10–20 entries for minion/elite/boss + tactics.  
- **Adventure Package:** 1-page scenes with counters and stakes.

**Requirement for Quality Contribution:** each new rule should have:
- a sentence "what is this for" (what issue it solves),
- a short rule description,
- an example of 3–5 lines.

This way, the supplements will not disrupt the core and will be approachable for newcomers.

