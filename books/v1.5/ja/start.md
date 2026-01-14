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
generated_at: "2026-01-14T12:06:55.666Z"
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
# スタート (要約)



---



---

### [ERROR] 1) Bohater w 1 minutę

[Translation Failed] * **Koncept:** kim jesteś i w jakim gatunku grasz (1 zdanie).
* **Rola (wybierz jedną):**

  * **Szturm** – presja, walka, przełamywanie przeszkód
  * **Specjalista** – skradanie, precyzja, technika, obserwacja
  * **Adept** – moce, wiedza, wpływ, improwizacja
* **Cechy (3):**

  * **Siła (S)** – siła fizyczna, wytrzymałość, walka wręcz
  * **Zręczność (Z)** – refleks, skradanie, strzelanie, pilotowanie
  * **Moc (M)** – magia/psionika/technologia/blef/intuicja (zależnie od świata)
* **Kości cech:** jedna cecha **<span class="rpg-token token-d12">k12</span>**, jedna **<span class="rpg-token token-d8">k8</span>**, jedna **<span class="rpg-token token-d6">k6</span>** (wybierz zgodnie z rolą).
* **Serca:** 5. **Punkty Mocy:** 3 (wydajesz na moce i „zagrania specjalne”).
Poniżej masz gotowy fragment do wklejenia (wariant A), w stylistyce krótkich zasad „1-page”.

**Łut Szczęścia (jak działa):** wydaj **1 ŁS**, aby wybrać jedno:

* **Przerzut** swojego testu (zostawiasz lepszy wynik), albo
* **Podbicie kości o 1 stopień** na ten jeden rzut (**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>**), albo
* **Zamiana porażki na „sukces z kosztem”** — akcja się udaje, ale MG natychmiast dokłada cenę (np. tracisz czas, robisz hałas, zużywasz zasób, kończysz w gorszej pozycji, przyciągasz uwagę, psujesz sprzęt).

**Odzysk ŁS:** na początku kolejnej sesji wracasz do limitu. MG może przyznać **+1 ŁS** za odważne ryzyko, świetną decyzję fabularną lub granie konsekwencjami.

* **Ekwipunek:** 1 narzędzie „kluczowe” (np. miecz, karabin, zestaw hakerski), 1 ochrona (pancerz, tarcza energetyczna, kamuflaż), 3 drobiazgi pasujące do konceptu.

**Przykład:** Specjalista: Z <span class="rpg-token token-d12">k12</span>, M <span class="rpg-token token-d8">k8</span>, S <span class="rpg-token token-d6">k6</span>. W cyberpunku M to „Hacking/Influence”; w fantasy M to „Magia/Wola”.



---

### [ERROR] 2) Jak rozstrzygać akcje

[Translation Failed] 1. Gracz mówi **co robi** i **jak** (opis w świecie gry).
2. Prowadzący ustala **Trudność** i stawkę („co się stanie przy porażce”).
3. Rzuć kością cechy (S/Z/M) i porównaj z Trudnością.

**Trudność (T):**

* **3** łatwe, **4** standard, **5** trudne, **6** bardzo trudne, **8** heroiczne, **12** legendarne.

**Wynik rzutu:**

* **1** – porażka z konsekwencją (komplikacja wchodzi na pewno).
* **< T** – porażka (ale scena idzie dalej: strata czasu, hałas, gorsza pozycja, utrata zasobu).
* **≥ T** – sukces.
* **Maks na kości** (np. 12 na <span class="rpg-token token-d12">k12</span>, 20 na <span class="rpg-token token-d20">k20</span>) – sukces wyjątkowy: dostajesz dodatkową korzyść.

**Modyfikatory bez liczenia:**

* **Lepsza sytuacja**: podbij kość o 1 stopień (<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>).
* **Gorsza sytuacja**: obniż kość o 1 stopień (<span class="rpg-token token-d20">k20</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d4">k4</span>).
* **Pomoc sojusznika** (kosztuje jego akcję): podbij kość o 1 stopień.

**Przykład:** Adept próbuje zamknąć portal (M <span class="rpg-token token-d8">k8</span>) przy alarmie i stresie → gorsza sytuacja, spada na <span class="rpg-token token-d6">k6</span>. T = 5. Rzut 6: sukces, ale „alarm” zostaje w tle jako presja fabularna.



---

### 3) ボード上の動きと戦い

- 移動: 5マスまで（対角移動可）。
- あなたのターン: 移動 + 1アクション（例: 攻撃、魔法、探索、レバーを引く）。
- 攻撃:
  - 近接 (S): 敵の<span class="rpg-token token-tn">TN</span>に対するロール。
  - 遠距離 (Z): 対象の防御が<span class="rpg-token token-tn">TN</span>を1段階上げる。
- 敵の<span class="rpg-token token-tn">TN</span>: 兵士 6、エリート 8、ボス 12。
- 命中の結果: 兵士 — 命中で倒れる; エリート — GMが有利な条件を要求する場合がある; ボス — 3ダメージ（命中 = 1ダメージ）。ボスに対する特別な成功 = 2ダメージ。
- 反撃: 近接攻撃や反撃範囲で外した場合、1ハートを失う（完全防御がない限り）。
例: 魔法使い (Z <span class="rpg-token token-d6">d6</span>) が箱の後ろにいる兵士にスリングで攻撃する: <span class="rpg-token token-tn">TN</span> 6 + 防御 → 8。魔法使いは盗賊に助けを求め（サイコロを<span class="rpg-token token-d8">d8</span>に上げる）て、より良い位置に移動する（<span class="rpg-token token-tn">TN</span>が6に下がる）。<span class="rpg-token token-d8">d8</span>=7 — 命中。



---

### 4) 魔法

- 呪文を唱える: 効果を説明し、マナを消費し、魔法を発動する (M)。
  - トリック (炎、轟音、霧) — <span class="rpg-token token-tn">TN</span> 4、コスト 0–1 マナ。
  - 弾丸/シールド/ジャンプ 5マス — <span class="rpg-token token-tn">TN</span> 6、コスト 1 マナ。
  - エリア/治療 +2 ハート/麻痺 — <span class="rpg-token token-tn">TN</span> 8、コスト 2 マナ。
  - 大魔法 (氷の橋、火の嵐) — <span class="rpg-token token-tn">TN</span> 12、コスト 3 マナ。
- 失敗: マナが無駄になる; 小さな結果が生じる (息切れ −1 ハート または 敵の不本意な注意を引く)。
- 戦闘後の休息: 全てのマナを回復する; 安全な休息はハートも回復する。
例: 「閃光」 (短距離テレポート 5マス): <span class="rpg-token token-tn">TN</span> 6、コスト 1 マナ。魔法使い <span class="rpg-token token-d10">d10</span> を振って 7 — シールドの後ろに成功したジャンプ。



---

### 5) 堕落と治療

- 0 ハート: 倒れている（動けない）。味方はアクションを使ってあなたを1ハートに回復させることができます。
- 戦闘後、短い休憩と食事を取ることで、あなたはハートとマナを完全に回復します。
例: ローグが0に倒れる。戦士が彼を立ち上がらせる — ローグは1ハートに戻ります。



---

### 6) キャラクターの成長

冒険の後に、次のいずれかを選択してください：
- 1つの属性をサイコロのサイズで上げる：<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>、
- または +1 ハート（最大7）、
- または +1 マナ（最大5）。
例：戦士が力を<span class="rpg-token token-d10">d10</span>から<span class="rpg-token token-d12">d12</span>に上げる — <span class="rpg-token token-tn">TN</span> 12に当てやすくなる。



---

### 7) ダブル・<span class="rpg-token token-d6">d6</span>バリアント

ダイス<span class="rpg-token token-d6">d6</span>が1つだけの場合：
- 各特性には成功の閾値があり、ダイスのサイズの代わりになります：
  - マスター 3+, 熟練者 4+, 初心者 5+, スキルなし 6。
- 難易度（<span class="rpg-token token-tn">TN</span>）は状況を1段階変化させます（簡単/難しい）。
- 助け：閾値を1下げる（例：このロールで4+から3+に）。
- 成長：1つの特性のレベルを上げる（例：熟練者4+ → マスター3+）または+1 ハート/マナ。
例：軽い防御を持つターゲットに対する盗賊の射撃（熟練者4+）は、難易度が1段階上がるため5+が必要です。<span class="rpg-token token-d6">d6</span>のロール=5 — ヒット。

