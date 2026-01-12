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
generated_at: "2026-01-12T10:14:52.318Z"
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
# Monster Book



---



---

- Same terminology as the Basic Rules and GM books.
- Only players roll. Opponents apply pressure via <span class="rpg-token token-tn">TN</span> and moves; damage usually comes from retaliation or forced tests.




---

> Name — Class, <span class="rpg-token token-tn">TN</span>, Wounds, Role, Move, Special

- Class: Minion | Elite | Boss
- <span class="rpg-token token-tn">TN</span>: the number 4/6/8/12 to hit/outmaneuver the foe.
- Wounds: for Elite and Boss only (default: Elite 2, Boss 3). Minions have no Wounds (they drop on a hit).
- Role: Brute (melee), Skirmisher (mobile), Artillery (ranged), Controller (area/control), Support (buffs/debuffs).
- Move: default 5 squares; change if mobility is defining (e.g., 6 Fast, Flying, Jump 3).
- Special: one or two short capabilities (see Traits and Moves).

Example: “Elite Guard — Elite, <span class="rpg-token token-tn">TN</span> 8, Wounds 2, Brute, Move 5, Special: Heavy Cover; Push.”




---

- Minion: <span class="rpg-token token-tn">TN</span> 6, drops on 1 hit. Pressure by numbers. Retaliation on a miss: −1 Heart.
- Elite: <span class="rpg-token token-tn">TN</span> 8, 2 Wounds. Usually 1 defensive trait or mobility edge. Retaliation on a miss: −1 Heart; sometimes an extra situational effect.
- Boss: <span class="rpg-token token-tn">TN</span> 12, 3 Wounds. Has 2–3 special moves and shapes terrain/tempo. Can force PC tests (evasion, stabilize, etc.).




---

- Brute: presses in melee, pushes from cover.
- Skirmisher: darts in/out, punishes isolated PCs.
- Artillery: fires from cover, forces movement.
- Controller: creates threat zones, smoke/fields, pushes/pulls.
- Support: strengthens allies, shifts <span class="rpg-token token-tn">TN</span> (±1 step) situationally.




---

Add 1–2 to a block. Purely descriptive; only shift <span class="rpg-token token-tn">TN</span> by a step if it makes sense.
- Natural Cover: usually has partial cover at range (attacks against it → <span class="rpg-token token-tn">TN</span> +1 step).
- Light Armor: the first 1‑Heart retaliation on this unit in a scene is ignored.
- Tough: the first success against this unit doesn’t inflict a Wound (only displacement/position) — good for bosses.
- Fast (Move 6): ignores 1 square of difficult terrain each turn.
- Climber/Jumper: treats vertical/obstacle movement as regular; jump 3.
- Flying: ignores ground obstacles (ensure reasonable cover exists).
- Scout: harder to ambush; the first stealth attempt against it is <span class="rpg-token token-tn">TN</span> +1.
- Resistance [type]: the first effect of that type in a scene is reduced (GM defines how: shorter, smaller, weaker).
- Vulnerability [type]: attacks of that type have <span class="rpg-token token-tn">TN</span> −1 step.
- Swarm: when adjacent, retaliation on a miss may affect two PCs within 1 square.




---

Pick 1–2 signature moves. If they threaten PCs, the GM may call for an appropriate PC test (D or M) vs the foe’s <span class="rpg-token token-tn">TN</span>.
- Push (Brute): on a hit, also move the target 1–2 squares.
- Break Cover: when this unit hits, the target’s cover stops working until the end of next round.
- Slip (Skirmisher): entering/leaving melee doesn’t trigger retaliation.
- Volley (Artillery): 3×3 area; all inside test D vs <span class="rpg-token token-tn">TN</span>; failure: −1 Heart and push 1 square.
- Anchor (Controller): a 3×3 zone becomes “sticky” (entering costs the Action) until end of next round.
- Bolster (Support): one ally is 1 step easier to protect/aid until end of round (attackers against it face <span class="rpg-token token-tn">TN</span> +1).
- Summon (Boss): once per fight, brings in 2 minions in free squares.
- Barrier (Boss): until the end of the enemy phase, PCs’ ranged attacks are <span class="rpg-token token-tn">TN</span> +1.
- Shockwave (Boss): all within 2 squares test S vs <span class="rpg-token token-tn">TN</span>; on failure: −1 Heart or knocked down (lose Move this turn).




---

1) Pick class: Minion / Elite (2 Wounds) / Boss (3 Wounds).
2) Set <span class="rpg-token token-tn">TN</span>: 6 / 8 / 12 (rarely 4 for very weak, 10 for tough elites).
3) Choose a role: Brute, Skirmisher, Artillery, Controller, Support.
4) Add 1–2 traits and 1 move (Boss: 2–3 moves).
5) Move: usually 5; change only if it matters.




---

Swap names/colors to fit your world.


### 7.1 Minions
- Guard Minion — Minion, <span class="rpg-token token-tn">TN</span> 6, —, Brute, Move 5, Special: Natural Cover.
- Scout Minion — Minion, <span class="rpg-token token-tn">TN</span> 6, —, Skirmisher, Move 6, Special: Scout.
- Shooter Minion — Minion, <span class="rpg-token token-tn">TN</span> 6, —, Artillery, Move 5, Special: Small Volley (2×2 warning; on failure −1 Heart).
- Controller Minion — Minion, <span class="rpg-token token-tn">TN</span> 6, —, Controller, Move 5, Special: Anchor (one‑shot, 1 round).
- Support Minion — Minion, <span class="rpg-token token-tn">TN</span> 6, —, Support, Move 5, Special: Bolster (once per scene).


### 7.2 Elites
- Elite Guard — Elite, <span class="rpg-token token-tn">TN</span> 8, Wounds 2, Brute, Move 5, Special: Light Armor; Push.
- Elite Stalker — Elite, <span class="rpg-token token-tn">TN</span> 8, Wounds 2, Skirmisher, Move 6, Special: Slip; Vulnerability [observation] (easier to detect).
- Elite Shooter — Elite, <span class="rpg-token token-tn">TN</span> 8, Wounds 2, Artillery, Move 5, Special: Natural Cover; Volley (3×3 after setup).
- Elite Controller — Elite, <span class="rpg-token token-tn">TN</span> 8, Wounds 2, Controller, Move 5, Special: Anchor; Push 1 on critical.
- Elite Medic — Elite, <span class="rpg-token token-tn">TN</span> 8, Wounds 2, Support, Move 5, Special: Bolster; on a hit, removes one ally complication (fictional).


### 7.3 Bosses
- Commander — Boss, <span class="rpg-token token-tn">TN</span> 12, Wounds 3, Support, Move 5, Special: Summon; Bolster; Barrier.
- Colossus — Boss, <span class="rpg-token token-tn">TN</span> 12, Wounds 3, Brute, Move 5, Special: Push (up to 2 squares); Tough; Shockwave.
- Hunter — Boss, <span class="rpg-token token-tn">TN</span> 12, Wounds 3, Skirmisher, Move 6, Special: Slip; Scout; Leaping Volley (after a move).
- Tactician — Boss, <span class="rpg-token token-tn">TN</span> 12, Wounds 3, Controller, Move 5, Special: Anchor (sustain for 1 Mana/round or action); Barrier; Summon (1 minion/round up to 3).




---

Hazards are mindless opponents or environmental effects. They trigger on turns or conditions.
Format: Name — <span class="rpg-token token-tn">TN</span>, Effect, How to Disable
- Turret — <span class="rpg-token token-tn">TN</span> 8, Effect: on the enemy phase each PC in line tests D vs <span class="rpg-token token-tn">TN</span>; failure: −1 Heart; Disable: M or D <span class="rpg-token token-tn">TN</span> 8 at the panel.
- Snap Trap — <span class="rpg-token token-tn">TN</span> 6, Effect: entering the cell forces a D test; failure: restrained or −1 Heart; Disable: D <span class="rpg-token token-tn">TN</span> 6 with tools.
- Repulse Field — <span class="rpg-token token-tn">TN</span> 8, Effect: at start of turn push 2 squares toward edge; Disable: M <span class="rpg-token token-tn">TN</span> 8 (disrupt) or cut power (S <span class="rpg-token token-tn">TN</span> 6).
- Gas/Smoke — <span class="rpg-token token-tn">TN</span> 6, Effect: in a 3×3 area, test M or D; failure: blinded zone/−1 Heart; Disable: vent (S) or seal (D).




---

Pick one from each line (or roll <span class="rpg-token token-d6">d6</span>):
1. Scene goal: cross / retrieve / disable / escort / steal / defend
2. Terrain focus: open / narrow corridors / multi‑level / modular cover / dangerous edges / fog‑smoke
3. Opposition: 6× minion / 4× minion + elite / 2× elite / boss / boss + 2× minion / elite + hazard
4. Enemy edge: cover / height / mobility / time clock / chokepoints / remote support
5. PC edge: surprise / higher ground / tools / short barrier / shortcut / neutral ally




---

Use steps instead of numeric TNs:
- Minion: “Standard” (≈ <span class="rpg-token token-tn">TN</span> 6)
- Elite: “Hard” (+1 step)
- Boss: “Heroic” (+2 steps) and 3 Wounds
Traits and moves stay the same; when a note says “<span class="rpg-token token-tn">TN</span> +1”, raise the step.




---

- If fights end too quickly: add minions in waves (2/round) or raise <span class="rpg-token token-tn">TN</span> by a step for enemies with positional advantage.
- If fights drag: offer more critical opportunities via position, or lower <span class="rpg-token token-tn">TN</span> for weakened foes.
- Two elites ≈ small boss; boss + 4 minions ≈ a two‑hour session finale.




---

- Defensive Guard — Minion, <span class="rpg-token token-tn">TN</span> 6, —, Artillery, Move 5, Special: Natural Cover.
- Mobile Patrol — Minion, <span class="rpg-token token-tn">TN</span> 6, —, Skirmisher, Move 6, Special: Scout.
- Heavy Assault — Elite, <span class="rpg-token token-tn">TN</span> 8, Wounds 2, Brute, Move 5, Special: Light Armor; Push.
- Field Tactician — Elite, <span class="rpg-token token-tn">TN</span> 8, Wounds 2, Controller, Move 5, Special: Anchor; Bolster.
- Field Commander — Boss, <span class="rpg-token token-tn">TN</span> 12, Wounds 3, Support, Move 5, Special: Summon; Barrier; Bolster.
- Terrain Colossus — Boss, <span class="rpg-token token-tn">TN</span> 12, Wounds 3, Brute, Move 5, Special: Tough; Shockwave; Push.

---
This toolkit lets you produce usable foes fast. Set <span class="rpg-token token-tn">TN</span>, choose class and role, add 1–2 traits and a move — and you’re ready for the grid.


