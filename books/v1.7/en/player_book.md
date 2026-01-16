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
generated_at: "2026-01-16T10:17:16.355Z"
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
# Player Book



---



---

### 1) What Gameplay at the Table Looks Like

- **Game Master (GM)** describes the situation and says what is possible in this scene. - **You** say: **what you do** and **what effect you want**. - If the outcome is uncertain or risky, the GM says: 1) **which attribute** you use (<span class="rpg-token token-stat">P</span>/C/<span class="rpg-token token-stat">M</span>), 2) **what is the Difficulty** <span class="rpg-token token-t">D</span> (or **Defense** of the target), 3) **what is at stake upon failure** (consequence). Then you roll the attribute die and immediately know what happens next.

### The Shortest Rule

**Roll an attribute die. Result ≥ <span class="rpg-token token-t">T</span> = success.**



---

### 2) What Your Character Has

Your character has:
- **Concept** (1 sentence: who you are, in which world you operate),
- **Role** (Assault / Specialist / Adept),
- 3 **traits**: Strength (<span class="rpg-token token-stat">S</span>), Dexterity (<span class="rpg-token token-stat">Z</span>), <span class="rpg-token token-power">Power</span> (<span class="rpg-token token-stat">M</span>),
- **Hearts** (endurance) and **<span class="rpg-token token-power">Power</span> Points** (PP),
- **Stroke of <span class="rpg-token token-luck">Luck</span>** (SoL),
- (optionally) **Talents**,
- **equipment**.

### 2.1 Attributes (<span class="rpg-token token-stat">S</span>/A/<span class="rpg-token token-stat">P</span>) — what they are for

- **Strength (<span class="rpg-token token-stat">S</span>)**: melee combat, forcing, carrying, endurance.
- **Agility (A)**: shooting, precision, sneaking, dodging, acrobatics, driving vehicles.
- **<span class="rpg-token token-power">Power</span> (<span class="rpg-token token-stat">P</span>)**: "special effects" of the game world: magic, psionics, faith, supertechnology, hacking, influence, intuition — depending on the convention.

### 2.2 Attribute Dice — How They Work

Each attribute has a die: <span class="rpg-token token-<span class="rpg-token token-d4">k4</span>"><span class="rpg-token token-d4">d4</span></span>, <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">d6</span></span>, <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span>, <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span>, or <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">d20</span></span>.  
When you use an attribute, you roll **one die** of that attribute.

- A larger die = a greater chance of success and a critical success (max on the die).

**Example:** You have Dexterity <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span>. When you shoot, climb, or sneak, you typically roll <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span>.

### 2.3 Resources: Hearts, <span class="rpg-token token-power">Power</span> Points, and Stroke of <span class="rpg-token token-luck">Luck</span>

- **Hearts:** 5 at the start. Hits and pressure take away Hearts. 
- **<span class="rpg-token token-power">Power</span> Points (PP):** 3 at the start. You spend them on powers and actions beyond the standard. 
- **Stroke of <span class="rpg-token token-luck">Luck</span> (SoL):** 2 at the start of each session. This is your "scene saving" and enhancing the drama.



---

### Step 1: Concept and Role

Choose a role – this is the general style of action (fits any universe).

- **Assault**: you take risks and push scenes forward.  
  (e.g. warrior, marines, security guard, hunter, barbarian)
- **Specialist**: you act precisely, with a plan and tools.  
  (e.g. rogue, sniper, scout, hacker, pilot, tracker)
- **Adept**: you do things "beyond the standard" – with <span class="rpg-token token-power">power</span>, knowledge, influence.  
  (e.g. mage, psionic, cleric, alchemist, technomancer, diplomat)

### Step 2: Allocate Attribute Dice

Allocate dice: one attribute <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span>, one <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span>, one <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">d6</span></span>.

Quick tips:
- **Assault** usually has <span class="rpg-token token-stat">S</span> the highest.
- **Specialist** usually has <span class="rpg-token token-stat">Z</span> the highest.
- **Adept** usually has <span class="rpg-token token-stat">M</span> the highest.

### Step 3: Record Resources

- **Hearts:** 5  
- **<span class="rpg-token token-power">Power</span> Points:** 3  
- **<span class="rpg-token token-luck">Luck</span>:** 2 (refreshed at the beginning of the session)

### Step 4 (optional): Choose 2 Talents

Talents are short phrases describing what you are good at (skills that frequently come up in the game). 
- Examples: "Scout", "Mechanic", "Medic", "Negotiator", "Athlete", "Analyst", "Hacker", "Ritualist".

**How Talents work:** if a Talent genuinely helps in a test, the GM considers this a better situation, and you can **upgrade your die by 1 step** for this roll.  
- Usually 1 Talent per 1 test.
- A Talent does not replace the description of the action – it is meant to enhance a reasonable plan.

**Example:** You have the Talent "Mechanic" and try to start the generator in an emergency. The GM decides it helps: you upgrade <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span> to <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span> for this test.

### Step 5: Equipment

List:
- 1 'key' tool (weapon or professional equipment),
- 1 protection (armor, shield, camouflage - depending on the world),
- 3 utility items.

Equipment usually acts as a **permission**: if you have something, you can attempt the appropriate actions. A good tool can also create a better situation (dice boost) if it makes sense.

### Character Example (Universal)

- Role: Specialist  
- <span class="rpg-token token-stat">S</span> <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">d6</span></span>, A <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span>  
- Hearts 5, MP 3, RL 2  
- Talents: “Scout”, “Negotiator”  
- Equipment: ranged weapon, lockpicks/toolkit, rope, flashlight



---

### 4.1 When You Roll

You roll when:
- something is **risky** or uncertain,
- failure has **significant consequences**.

If something is obvious and without pressure, the GM may say "it succeeds" without a roll.

### 4.2 Difficulty <span class="rpg-token token-t">T</span>

The GM chooses the Difficulty:

- <span class="rpg-token token-t">T 3</span> easy  
- <span class="rpg-token token-t">T 4</span> standard  
- <span class="rpg-token token-t">T 5</span> hard  
- <span class="rpg-token token-t">T 6</span> very hard  
- <span class="rpg-token token-t">T 8</span> heroic  
- <span class="rpg-token token-t">T 12</span> legendary

You do not have to "guess" the Difficulty — the GM states it outright.

### 4.3 Results of the Roll

- **1**: failure with a consequence (complication definitely occurs).
- **Result < <span class="rpg-token token-t">T</span>**: failure (but the scene continues).
- **Result ≥ <span class="rpg-token token-t">T</span>**: success.
- **Max on the die** (e.g., 12 on <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>, 20 on <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>): exceptional success + additional benefit.

**Additional benefit** (examples): faster, quieter, safer, greater effect, better position, additional detail in your favor.

### 4.4 Better/Worse Situation (Without Bonuses)

Instead of counting modifiers, play the situation:

- **Better situation** → upgrade the die by 1 step  
  (<span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">d6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">d20</span></span>)
- **Worse situation** → downgrade the die by 1 step  
  (<span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">d20</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">d6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d4">k4</span>"><span class="rpg-token token-d4">d4</span></span>)

Your role as a player: **create better conditions** through description and decisions (cover, preparation, tools, plan, reconnaissance).

### 4.5 Ally Assistance

An ally can use their Action to assist you. In that case, for that one roll:
- you increase the die by 1 rank.

The assistance must make sense in the description (distraction, cover, providing tools, fire support, an extra pair of hands).

### Test Example (Clear and Complete)

You want to unlock the locked door before the guards arrive.
- GM: “This is Dexterity. <span class="rpg-token token-t">T 5</span>. Failure: you make noise and lose time.”
- You have D <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span>, but you're using lockpicks and have the Talent “Lock Specialist” → better situation, bump up to <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span>.
- Roll <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span> = 6 → success: the door opens without an alarm.



---

### 5) Stroke of <span class="rpg-token token-luck">Luck</span> (SL) — when to use it

At the beginning of each session, you have **2 SL**. SL is used to:
- save important scenes,
- add drama,
- reward bold decisions.

Spend **1 SL** to choose one:
- **Re-roll** your test (keep the better result), or  
- **Boost a die by 1 step** for that single roll, or  
- **Turn a failure into a "success with a cost"** — the action succeeds, but the GM immediately adds a price.

**Regain SL:** at the start of the next session you reset to the limit. The GM may grant **+1 SL** for taking bold risks, making great narrative decisions, or playing with consequences.

**Example:** A failure while jumping between rooftops would mean falling to the street. You spend 1 SL to turn failure into success with a cost: you make the leap, but either lose equipment or twist an ankle (a worse situation in the next scene).



---

### 6.1 Distances (default, without map)

Describe distance with four words:
- **Close** (within arm's reach),
- **Nearby** (a few steps),
- **Far** (the other side of the scene),
- **Very far** (sniper/vehicle range).

In a turn, you have: **Movement + 1 Action**.  
Movement usually changes the distance by 1 degree (Nearby→Close, etc.).

### 6.2 Option: Grid-Based Play

If you are playing on a map:
- 1 square = 1–2 meters,
- movement per turn: **up to 5 squares**,
- diagonals count as 1 square,
- the rest of the rules work the same.

### 6.3 Attack

- **Melee:** roll **Strength (<span class="rpg-token token-stat">S</span>)** against the target's **Defense**.  
- **Ranged:** roll **Dexterity (<span class="rpg-token token-stat">Z</span>)** against the target's **Defense**.

**Opponents' Defense (approximate):**
- <span class="rpg-token token-t">4</span> Weak  
- <span class="rpg-token token-t">5</span> Typical  
- <span class="rpg-token token-t">6</span> Elite  
- <span class="rpg-token token-t">8</span> Boss  
- <span class="rpg-token token-t">12</span> Legendary Boss

### 6.4 Cover and Position

- Target in cover / bad angle / pressure → worse situation (lower the die).
- Good position / surprise / numerical advantage → better situation (raise the die).

### 6.5 Hit and Damage

- A hit deals **1 Heart**.
- An exceptional success deals **2 Hearts** or provides a strong effect (disarming, knocking over, pushing back, forcing out of cover).

### 6.6 0 Hearts

When you fall to **0 Hearts**, you are out of action (wounded, stunned, in shock – according to the convention).
- An ally can use an Action to set you to **1 Heart**.
- If the pressure continues, your priority is cover and evacuation, not "tanking."

### Example of a Short Turn (without Grid)

- You are **Nearby** the elite.
- Movement: you move **Close** behind a pillar (cover).
- Action: melee attack (<span class="rpg-token token-stat">S</span>). The elite's defense is <span class="rpg-token token-t">6</span>. You have <span class="rpg-token token-stat">S</span> <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>.  
  Roll 9: success, the elite loses 1 Heart.

---



---

### 7) Powers and Moves Beyond Standard (<span class="rpg-token token-power">Power</span> Points)

What we call "<span class="rpg-token token-power">power</span>" depends on the world: spells, psionics, faith, gadgets, hacking, super tricks.

### 7.1 How You Use <span class="rpg-token token-power">Power</span>

1) Describe the effect.
2) The GM tells you the Difficulty and cost in MP.
3) Spend MP and roll **<span class="rpg-token token-power">Power</span> (<span class="rpg-token token-stat">P</span>)**.

### 7.2 Effect Levels (T / cost)

- **Trick:** short effect, trick → <span class="rpg-token token-t">T 4</span>, cost 0–1 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>
- **Standard:** attack, shield, impulse → <span class="rpg-token token-t">T 5</span>, cost 1 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>
- **Strong:** area, healing, paralysis, live hack → <span class="rpg-token token-t">T 6</span>, cost 2 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>
- **Great:** scene change, powerful interference → <span class="rpg-token token-t">T 8–12</span>, cost 3 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>

### 7.3 Exceptional Failure and Success

- Failure: expended <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span> is lost, and a consequence applies (overload, trace, loss of position, side effect).
- Max on the die: exceptional success + additional benefit (greater range, longer duration, stronger effect, or fewer "side effects").

### 7.4 Recover MP

- After a scene of conflict, you recover **1 MP**.
- After a safe rest – full recovery (as long as the game world allows it).

**Example (fantasy):** "Short Jump" – Standard, <span class="rpg-token token-t">T 5</span>, cost 1 MP.  
**Example (sci-fi):** "Overload the electronic lock" – Standard, <span class="rpg-token token-t">T 5</span>, cost 1 MP.





---

### 8) Rest and Recovery

If you have a safe moment (shelter, dressing, service, meal):
- you return to full **Hearts**,
- and replenish **MP** according to the rest rule in your convention.

In more stringent campaigns, the GM may require a complete halt to recover everything.



---

### 9) Character Development (when you "level up")

Development occurs **after the adventure** (usually after 1–3 sessions, depending on the campaign's pace).  
You choose **one**: 
- increase one attribute by 1 die level (up to a maximum of <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">d20</span></span>), or 
- +1 Heart (maximum 7), or 
- +1 MP (maximum 5), or 
- a new Feat (a short, one-sentence rule agreed upon with the GM). 

**Example:** Dexterity rises from <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span> to <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span>. From now on, you perform all Dexterity tests with <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span>.



---

### 10) "Only <span class="rpg-token token-d6">d6</span>" Variant: 2d6

If you want to play using only <span class="rpg-token token-d6">d6</span>:
- Each test is **2d6 + attribute modifier**.
- Starting attribute modifiers: one attribute **+2**, one **+1**, one **+0**.

**Result:**
- **6 or less** – failure with consequence  
- **7–9** – success with a cost  
- **10+** – full success  
- **12** – exceptional success

**Situation:** give **+1 / -1** to the roll (helps/hinders), instead of changing thresholds.

**<span class="rpg-token token-luck">Luck</span> in 2d6:** works the same way, only "boosting the dice" changes to **+1 to the roll**.

---



---

### 11) Good Player Habits

- Say: **what you do + why**. The purpose of the actions helps the GM set the stakes. - If Difficulty is high: don't "force the roll" — **change the situation** (preparation, tool, cover, help, another path). - Cooperate: an ally's help is one of the strongest, simplest levers in the system. - In combat, position wins: cover, distance, and situational advantage are often more important than statistics.

