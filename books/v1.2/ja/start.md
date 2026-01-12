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
generated_at: "2026-01-12T20:13:48.826Z"
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

### 1) 1分でヒーロー

- ロール（1つ選択）:
  - 戦士 — 力と近接戦闘の達人
  - 盗賊 — 速度、隠密、射撃の達人
  - 魔法使い — 魔法と知識の達人
- 特徴とサイコロ: 力 (S), 敏捷性 (Z), 魔法 (M)。
  - 戦士: S <span class="rpg-token token-d10">d10</span>, Z <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d6">d6</span>
  - 盗賊: S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
  - 魔法使い: S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d10">d10</span>
- 生命: 5 ハート。マナ: 3（魔法使用時）。
- 装備: 武器、軽鎧、役割に合った3つのアイテム。
例: 盗賊は敏捷性 <span class="rpg-token token-d10">d10</span>を持っているので、射撃には <span class="rpg-token token-d10">d10</span>を使用します。



---

### 2) アクションの実行方法

1. 適切な特性（S/Z/M）を選び、その特性のサイコロを振ります。
2. 難易度（<span class="rpg-token token-tn">TN</span>）と比較します：
   - 簡単 4、普通 6、難しい 8、英雄的 12。
3. 結果：
   - サイコロの出目が1 — 失敗（複雑な状況：騒音、時間の浪費、小さな怪我など）。
   - 出目 < <span class="rpg-token token-tn">TN</span> — 失敗。
   - 出目 ≥ <span class="rpg-token token-tn">TN</span> — 成功。
   - サイコロの最大値（例：<span class="rpg-token token-d10">d10</span>で10、<span class="rpg-token token-d20">d20</span>で20） — 特別な成功と追加の利益。
改善点を数えずに：
- 状況の改善/悪化：<span class="rpg-token token-tn">TN</span>を1段階下げる/上げる（例：6 → 8は防御による）。
- 仲間の助け（自分の行動で）：このロールのために「サイコロを1サイズ上げる」（<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>）。
例：戦士がドアをこじ開ける（普通 6）。<span class="rpg-token token-d10">d10</span>を振って10が出る — 特別な成功：ドアが飛び出し、その後ろにいる兵士が転倒する。



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

### 4) 魔法（簡単に）

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

