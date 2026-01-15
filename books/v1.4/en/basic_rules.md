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
generated_at: "2026-01-15T08:02:46.478Z"
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
# Core Rules



---



---

### Things Needed for Gameplay

- Pencil and character sheet.
- (Optional) map/grid and character tokens (graph paper, mat, VTT).
- Dice: **<span class="rpg-token token-d4">d4</span>, <span class="rpg-token token-d6">d6</span>, <span class="rpg-token token-d8">d8</span>, <span class="rpg-token token-d12">d12</span>, <span class="rpg-token token-d20">d20</span>**.
  - In practice, one of each is sufficient (you roll one die at a time).
  - (Optional) **d100** for random tables or generators.
- If you only have **<span class="rpg-token token-d6">d6</span>**, use the **2d6** variant (at the end).

---



---

### Glossary of Terms

These words appear in the rules — here they are explained "in plain language":

- **GM (Game Master)**: leads the world, describes situations, controls opponents, sets Difficulty and consequences.
- **Player**: describes the actions of their character and makes rolls.
- **Test**: a dice roll that resolves an uncertain outcome.
- **Attributes**: **Strength (<span class="rpg-token token-stat">S</span>)**, **Dexterity (D)**, **Might (<span class="rpg-token token-stat">M</span>)**. They indicate *what die you roll*.
- **Attribute Die**: the size of the die assigned to an attribute (e.g., D = <span class="rpg-token token-d12">d12</span>).
- **Difficulty (D)**: the number that must be met or exceeded for the action to succeed.
- **Success**: result ≥ Difficulty.
- **Exceptional Success**: **maximum result** on the die (e.g., 12 on <span class="rpg-token token-d12">d12</span>, 20 on <span class="rpg-token token-d20">d20</span>) — success + additional benefit.
- **Complication**: an additional problem after failure (noise, loss of time, worse position, loss of resource).
- **Success at a Cost**: the action succeeds, but you pay a price (compromise, loss of resource, exposure, risk).
- **<span class="rpg-token token-luck">Luck</span> Point (LP)**: a limited resource that allows you to salvage scenes (reroll / boost die / turn failure into success at a cost).
- **Hearts**: the "life" of a character (stamina, wounds, condition — depending on the world).
- **<span class="rpg-token token-power">Power</span> Points (PP)**: a resource for powers and "above standard" plays (magic, psionics, gadgets, "cinematic" actions).
- **Defense**: the threshold for hitting an opponent in combat (instead of multiplying rules about armor, armor class, etc.).
- **Cover**: an obstacle between you and the target. Usually hinders ranged attacks or observational actions.



---

### 1. Character


Creating a character is quick. A character is: **concept + role + traits + resources + equipment**.

---

### 1.1 Concept

One sentence: who you are and what genre you are playing.

> Example: "A former corporate agent, now a bounty hunter who operates in the shadows and trusts no one."


### 1.2 Role (choose one)

Roles are deliberately "world-neutral". In fantasy, you might call them something else, in cyberpunk something different, but they function the same way.

- **Assault** — pressure, combat, overcoming obstacles, breaking through the front.
- **Specialist** — stealth, precision, technique, observation, planning.
- **Adept** — powers, influence, knowledge, improvisation (magic/psionics/technology depending on the world).

### 1.3 Attributes and Dice


You have three attributes:

- **Strength (<span class="rpg-token token-stat">S</span>)** — physical <span class="rpg-token token-power">power</span>, endurance, melee combat, forcing.
- **Dexterity (D)** — reflexes, precision, sneaking, shooting, driving.
- **Might (<span class="rpg-token token-stat">M</span>)** — "the special stuff": magic, psionics, advanced technology, social bluffing, intuition — depending on the convention.

**At the start, distribute the dice as follows:**
- one attribute has **<span class="rpg-token token-d12">d12</span>**,
- one has **<span class="rpg-token token-d8">d8</span>**, 
- one has **<span class="rpg-token token-d6">d6</span>**.

**Suggested distribution by role (the simplest):**
- **Assault:** <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d12">d12</span>, D <span class="rpg-token token-d8">d8</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d6">d6</span>
- **Specialist:** D <span class="rpg-token token-d12">d12</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">d8</span>, <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">d6</span>
- **Adept:** <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">d12</span>, D <span class="rpg-token token-d8">d8</span>, <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">d6</span>

> Example: if you have D = <span class="rpg-token token-d12">d12</span>, then when shooting, sneaking, and dodging, you usually roll <span class="rpg-token token-d12">d12</span>.

### 1.4 Resources

- **Hearts:** 5.
- **<span class="rpg-token token-power">Power</span> Points (PP):** 3.
- **<span class="rpg-token token-luck">Luck</span> Point (LP):** at the beginning of each session, you have **2 LP**.

**<span class="rpg-token token-luck">Luck</span> Point (how it works):** spend **1 LP** to choose one:
- **Reroll** your test (keep the better result), or
- **Increase the die by 1 step** for that one roll (**<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>**), or
- **Turn a failure into a 'success at a cost'** — the action succeeds, but the GM immediately adds a price (e.g., noise, loss of time, loss of resource, worse position, attracting attention, damage to equipment).

**Recovering LP:** at the beginning of the next session, you return to the limit. The GM may grant **+1 LP** for bold risks, great narrative decisions, or playing consequences.

### 1.5 Talents (optional, but recommended)

Talents are **2 short phrases** that describe what your character is good at (no lists, no tables).

- Examples: "Mechanic", "Scout", "Negotiator", "Medic", "Hacker", "Veteran", "Explorer".

**How Talents work:** if a Talent genuinely helps in a test, the GM may **increase the die by 1 step** (or neutralize a penalty).
- A Talent does not grant automatic successes.
- Usually, **a maximum of 1 Talent** affects a single test.

### 1.6 Equipment

List:
- 1 "key" tool (weapon / kit / gear without which you cannot do your job),
- 1 protection (armor, shield, camouflage — depending on the world),
- 3 trinkets useful in the adventure.

Equipment in the core rules is mainly **permission** (enables actions), not a numerical bonus.

### 1.7 Example of a Complete Character

- Concept: "Information thief who steals data from systems, not from pockets."
- Role: Specialist
- Attributes: <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">d6</span>, <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">d12</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">d8</span>
- Resources: 5 Hearts, 3 MP, 2 AP
- Talents: "Hacker", "Shadow"
- Equipment: pistol, light armor, lockpicking kit, rope, flashlight

---



---

### 2. Core Rules: Tests

This part is the most important — if you understand it, you understand the system.

### 2.1 When You Make a Test

You make a test when both conditions are met:
1) the outcome is uncertain (it may succeed or fail), and
2) the stakes are real (failure will change something / cost something).

If the action is trivial and without pressure — the GM may say "it succeeded" without a roll.

### 2.2 How to perform a test (step by step)

1) The player states **what they do** and **why**.
2) The GM chooses an attribute: **<span class="rpg-token token-stat">S</span>** or **<span class="rpg-token token-stat">Z</span>** or **<span class="rpg-token token-stat">M</span>**.
3) The GM sets the **Difficulty (D)** and explains what failure means (the stakes).
4) The player rolls the **attribute die**.
5) Compare the result with D and determine the consequences.

### 2.3 Difficulties (T)


We use simple thresholds. If in doubt, choose the lower threshold, and let the "difficulty" show through the consequences.

- **T 3** – easy (almost certain, but sometimes worth checking under pressure)
- **T 4** – standard (typical challenge)
- **T 5** – hard (requires competence or an advantage)
- **T 6** – very hard (risky without an advantage)
- **T 8** – heroic (for the best or with good preparation)
- **T 12** – legendary (rarely "clean"; usually as a campaign goal, plan, ritual, or under great conditions)


### 2.4 Test Results

- **Result ≥ T → Success.** You achieve the intended effect.
- **Result < T → Failure.** You do not achieve the effect, and the situation changes (complication or cost).
- **Rolled 1 → Failure + complication.** A complication definitely occurs.
- **Maximum result on the die → Exceptional success.**
  - In addition to success, you gain an **additional benefit** (faster, quieter, stronger, safer, additional effect).

> Example of success with a cost: "You manage to force the door, but you make noise and someone comes to check."

### 2.5 Advantages and Disadvantages (without counting)

Instead of adding +1/−1 to rolls, we change the **size of the dice**.

- **Better situation** → **upgrade the die by 1 step**  
<span class="rpg-token token-d6">k6</span> → <span class="rpg-token token-d8">k8</span> → <span class="rpg-token token-d12">k12</span> → <span class="rpg-token token-d20">k20</span>
- **Worse situation** → **downgrade the die by 1 step**  
<span class="rpg-token token-d20">k20</span> → <span class="rpg-token token-d12">k12</span> → <span class="rpg-token token-d8">k8</span> → <span class="rpg-token token-d6">k6</span> → <span class="rpg-token token-d4">k4</span>

**Examples of advantages:** preparation, good tools, positional advantage, surprise, support.  
**Examples of disadvantages:** darkness, slippery surfaces, time pressure, noise, distraction, cover.

**Order of rules:** for speed, assume that for one test you usually apply **a maximum of 1 advantage and 1 disadvantage** (they can cancel each other out).

### 2.6 Ally Assistance

An ally can sacrifice their action (or time in a scene outside of combat) to assist.

**Effect:** for this one test, **increase the die by 1 step**.

Assistance must be described sensibly (providing cover, handing over tools, distracting, stabilizing, giving hints).

### 2.7 Repeating Tests

If the test fails, do not repeat it "ad infinitum" without changing the situation.
- Either you do something differently (different attribute / different tools / different approach),
- or you accept the cost (time, alarm, resource),
- or you withdraw.

### 2.8 Examples of Tests (Outside of Combat)

**Example A — Stealthy Passage**
- Player: "I will cross the yard before the spotlight returns."
- GM: Dexterity (D). It’s under time pressure → Difficulty **T 5**.
- The character has the Talent “Shadow” → advantage, die increased by 1 step.
- Roll: D <span class="rpg-token token-d12">d12</span> = 4 → failure. GM: "They don’t notice you right away, but someone hears a rustle and starts checking the area (complication: pressure increases)."

**Example B — Forceful Breach**
- Player: "I will kick down the metal door before the guards reach the corner."
- GM: Strength (<span class="rpg-token token-stat">S</span>), Difficulty **T 6** (very hard without tools).
- Someone helps by holding the lock and wedging the door → die increased by 1 step.
- Roll: <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d12">d12</span> = 12 → exceptional success: the door gives way immediately and you do it quieter than expected.



---

### 3. Movement and Distances (Grid is an Option)

By default, NDE operates without a map: you describe the scene and the positions of the characters.

### 3.1 By Default: Descriptive Distances


Use four zones:
- **Close** — within arm's reach, melee combat.
- **Nearby** — a few steps away, easy to close in.
- **Far** — the other side of the scene, requires clear movement.
- **Very Far** — sniper/vehicle range/"at the edge of the scene".

In a turn, you can usually change the distance by **one zone** (e.g., Far → Nearby).

### 3.2 Option: Grid Play (for Tactics)


If you prefer specifics:
- 1 square = 1–2 m.
- Movement per turn: **up to 5 squares**.
- Diagonals are allowed (count as a regular square).


### 3.3 Cover and Line of Effect

- **Full cover:** it is impossible to interact "in line" (shot, observation, many powers).
- **Partial cover:** makes it difficult — usually **lowers the die by 1 step** for the attacker/watcher.

---



---

### 4. Combat

Combat is a standard scene with tests, only organized in turns.

### 4.1 When Combat Begins

Combat begins when:
- at least one side wants to harm the other, and
- it matters who acts and when.

If the situation is brief and obvious, the GM may resolve it with a single roll.

### 4.2 Turn Order (Simple Version)

Simply put:
- First, all players act (in any order),
- then the opponents act,
- and so on in a loop.

### 4.3 What Do You Do on Your Turn


In your turn, you have:
- **Movement** (changing zones / up to 5 squares in grid variant),
- **1 Action** (attack, test, assist, use <span class="rpg-token token-power">power</span>, equipment, interact with the scene).


### 4.4 Attack: How It Works

1) Choose a target and describe the attack.
2) Choose an attribute:
   - **melee** → roll **Strength (<span class="rpg-token token-stat">S</span>)**,
   - **ranged** → roll **Dexterity (D)**,
   - **powers** → usually roll **Might (<span class="rpg-token token-stat">M</span>)** (see Chapter 5).
3) Determine the target's **Defense**.
4) Roll the dice and compare it to the Defense.

### 4.6 Damage and 'How Much They Can Endure'

- A hit deals **1 Heart**.
- A **Critical Success** deals **2 Hearts** *or* provides a strong effect (disarm, knockdown, push out of cover) — choose one.

Simplest enemy archetypes:
- **Minion:** goes down after 1 hit.
- **Elite:** has **2 Hearts**.
- **Boss:** has **3 Hearts** (or 5 in final scenes).

> Note: 'goes down' does not necessarily mean death. They may be unconscious, fled, surrendered, or taken out of action.

### 4.5 Opponent Defense (Guideline)

- **Weak:** Defense **4**
- **Typical:** Defense **5**
- **Elite:** Defense **6**
- **Boss:** Defense **8** (legendary boss: **12**)

Cover and conditions usually change the size of the attacking dice (easing/difficulty), not the Defense.

### 5.7 Ranges (defaults)
- Melee: adjacent.
- Ranged: any visible target.
  - If you want a limit: treat up to 10 squares as no penalty; beyond that <span class="rpg-token token-<span class="rpg-token token-math">tn</span>"><span class="rpg-token token-math">TN</span></span> +1 step.


### 5.8 Multiple foes in close
If many minions are adjacent to one hero, either:
- raise <span class="rpg-token token-<span class="rpg-token token-math">tn</span>"><span class="rpg-token token-math">TN</span></span> by 1 step (pressure), or
- have failure include an extra complication (lose position).

Keep it fast: one resolution → one outcome.


### 4.7 Examples of Combat

**Example A — melee combat with a lackey**
- The Storm (<span class="rpg-token token-stat">S</span> <span class="rpg-token token-d12">d12</span>) attacks the lackey (Defense 5).
- Conditions are favorable (surprise) → die increases by 1 step, but it is already <span class="rpg-token token-d12">d12</span>, so the increase gives <span class="rpg-token token-d20">d20</span>.
- Roll <span class="rpg-token token-d20">d20</span> = 7 → hit, the lackey is down.

**Example B — shot at the elite from cover**
- The Specialist (<span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">d12</span>) shoots at the elite (Defense 6).
- The target is in partial cover → difficulty, die drops to <span class="rpg-token token-d8">d8</span>.
- Roll <span class="rpg-token token-d8">d8</span> = 6 → hit, the elite loses 1 Heart (leaving them with 1).

**Example C — boss and Stroke of <span class="rpg-token token-luck">Luck</span>**
- The Adept (<span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">d12</span>) tries to incapacitate the boss (Defense 8) with <span class="rpg-token token-power">power</span>.
- Roll <span class="rpg-token token-d12">d12</span> = 4 → failure. The player spends 1 LS for a reroll.
- Reroll = 10 → success. The boss loses 1 Heart, but the GM adds a cost: “the effect is loud, an alarm goes off.”



---

### 5. Powers (<span class="rpg-token token-stat">P</span>) and <span class="rpg-token token-power">Power</span> Points (PP)

In NDE, "<span class="rpg-token token-power">Power</span>" is a category of special effects. Depending on the world, it may mean:
- magic, psionics, rituals,
- advanced technology, drones, live hacking,
- cinematic hero moves (e.g., "masterful concentration"),
- social influence in games where conversation is a "<span class="rpg-token token-power">power</span>."

### 5.1 When You Spend <span class="rpg-token token-power">PM</span>

You spend <span class="rpg-token token-power">PM</span> when you try to achieve an effect **above standard**.

---

### 5.2 How to Use <span class="rpg-token token-power">Power</span> (Step by Step)

1) Describe the effect you want to achieve.
2) The GM determines the Difficulty and the cost in <span class="rpg-token token-power">PM</span>.
3) Spend <span class="rpg-token token-power">PM</span>.
4) Roll **<span class="rpg-token token-stat">M</span>** and compare it to the Difficulty.

**Failure:** the effect does not work; <span class="rpg-token token-power">PM</span> is lost; a complication arises (overload, trace, revelation, side effect).

### 5.3 Levels of Effects (Difficulty / Cost)

- **Trick** (short trick): **T 4 / 0–1 MP**  
  light, sound, minor illusion, momentary distraction.
- **Standard**: **T 5 / 1 MP**  
  projectile, shield, impulse, jump, enhancement.
- **Strong**: **T 6 / 2 MP**  
  area, control, healing, paralysis, "hack during combat."
- **Great**: **T 8–12 / 3 MP**  
  an effect that changes the scene or has campaign consequences.

### 5.4 Exceptional Success in <span class="rpg-token token-power">Power</span>

If you roll a maximum on the <span class="rpg-token token-stat">M</span> dice:
- increase the scale (larger area / longer / stronger), or
- add an additional benefit (quieter, more precisely, safer), or
- the GM may grant **1 MP** (if it fits the fiction).

### 5.5 Recovering MP

- After a conflict scene, you recover **1 MP**.
- After a safe rest, you return to full.

### 5.6 Examples of Powers

**Example A — Shield for a Dash**
- Player: "I set up a short cover to dash to a better position."
- GM: Standard **T 5**, cost 1 <span class="rpg-token token-power">PM</span>.
- Roll <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">d12</span> = 9 → success: you dash safely.

**Example B — Failure with Consequence**
- Player: "I stop the elite in their tracks."
- GM: Strong **T 6**, cost 2 <span class="rpg-token token-power">PM</span>.
- Roll = 1 → failure + complication: you lose 2 <span class="rpg-token token-power">PM</span>, and the effect rebounds, revealing your position.



---

### 6.1 0 Hearts

If you drop to 0 Hearts:
- you are **out of action** (wounded, stunned, in shock — depending on the convention),
- an ally can sacrifice an action to get you back on your feet with **1 Heart**.

### 6.2 Rest

- After a scene of conflict, if you have a moment to catch your breath and the basic conditions, you may return to full Hearts.
- In harsher campaigns, the GM may require a safe resting place to return to full strength.

---

### 7.3 Rest
After a scene of combat/conflict, if you have a moment of safe rest (and basic conditions), you return to full:
- Hearts,
- Mana.

This keeps the system fast and does not require lengthy healing.



---

### 7. Character Development

**When you grow:** after an adventure, mission, or important chapter of the story (usually every 1–3 sessions).

Choose **one**:
- **Increase** one attribute by 1 die step (max. up to <span class="rpg-token token-d20">d20</span>), or
- **+1 Heart** (max. 7), or
- **+1 MP** (max. 5), or
- **New Trait** (a one-sentence, specific ability agreed upon with the GM).

> Example: The Specialist increases Strength from <span class="rpg-token token-d12">d12</span> to <span class="rpg-token token-d20">d20</span>, as the campaign has entered a phase of chases and shootouts.

---



---

### 8. Variant Only <span class="rpg-token token-d6">d6</span>: 2d6

If you do not want to use different dice, play with **2d6**.

### 8.1 Attributes as Modifiers

Instead of die sizes, distribute the modifiers:
- one attribute has **+2**
- one has **+1**
- one has **+0**

### 8.2 Test

Roll **2d6 + ability modifier**.

**Result:**
- **6 or less** – failure with consequence
- **7–9** – success at a cost
- **10+** – full success
- **12** – exceptional success (additional benefit)

### 8.3 Difficulty of the Situation

Instead of changing the thresholds, give:
- **+1** for advantage, preparation, a good plan,
- **−1** for hindrances, pressure, cover, chaos.

### 8.4 <span class="rpg-token token-luck">Luck</span> Roll in 2d6

Spend 1 <span class="rpg-token token-luck">Luck</span> Point to:
- reroll 2d6, or
- add **+1** to the test result, or
- turn a failure into a success at a cost.

### 8.5 Quick Mapping (Optional)

If you ever want to "convert" a character between variants:
- <span class="rpg-token token-d6">d6</span> ≈ +0
- <span class="rpg-token token-d8">d8</span> ≈ +1
- <span class="rpg-token token-d12">d12</span> ≈ +2
- <span class="rpg-token token-d20">d20</span> ≈ +3 (for very experienced)



---

1) What exactly is the player trying to achieve?
2) Which attribute applies: <span class="rpg-token token-stat">S</span>/D/<span class="rpg-token token-stat">M</span>?
3) What’s the <span class="rpg-token token-<span class="rpg-token token-math">tn</span>"><span class="rpg-token token-math">TN</span></span> (4/6/8/12), and does the situation shift it by a step?
4) Any help (bump die)?
5) Roll → success/failure.
6) On failure: which complication (or retaliation in combat)?
7) On critical: which extra benefit?




---

### 1. Introduction

7.2 Additional tools are not required, but they can sometimes facilitate management.

### 9.1 Protection (armor) as a simple resource


If you want "protection" to have a clear effect:
- a character with protection has **1 Armor token per scene**, 
- when they would lose 1 Heart, they can instead expend an Armor token.

### 9.2 Time Pressure as a Timer

If the scene has a time limit, the GM sets a "counter" (e.g., 3 steps). Each failure moves the counter by 1. When it reaches the end — a consequence occurs (alarm, target fleeing, passage collapsing).

---

### 9.3 Retaliation (Risky Combat Variant)

If you want the fight to be more "intense" and fast-paced:
- when you **attack in melee** and **miss**, you lose **1 Heart**, provided the opponent could realistically reach you.
This is a variant — in the core of NDE, the consequences of failures in combat mainly arise from fiction and the GM's decisions.

