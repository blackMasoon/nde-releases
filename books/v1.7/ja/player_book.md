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
generated_at: "2026-01-16T10:17:16.306Z"
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
# プレイヤーの書



---



---

### 1) テーブルでのゲームの進め方

- **ゲームマスター (GM)** は状況を説明し、このシーンで何が可能かを伝えます。
- **あなた** は **何をするか** と **どんな効果を望むか** を言います。
- 結果が不確かまたはリスクがある場合、GM は以下を伝えます:
  1) **どの属性**を使うか (<span class="rpg-token token-stat">S</span>/<span class="rpg-token token-stat">Z</span>/<span class="rpg-token token-stat">M</span>)、
  2) **難易度**<span class="rpg-token token-t">T</span> (または目標の**防御**)、
  3) **失敗時の危険** (結果)。

その後、属性のダイスを振り、次に何が起こるかすぐにわかります。

### 最短ルール

**特徴ダイスを振る。結果が<span class="rpg-token token-t">T</span>以上 = 成功。**



---

### 2) あなたのキャラクターにあるもの

あなたのキャラクターには以下があります：
- **コンセプト**（1文：あなたが誰で、どんな世界で活動しているのか）、
- **役割**（ストーム / スペシャリスト / アデプト）、
- 3つの**特性**：力（<span class="rpg-token token-stat">S</span>）、器用さ（<span class="rpg-token token-stat">Z</span>）、力（<span class="rpg-token token-stat">M</span>）、
- **ハート**（耐久度）と **マジックポイント**（MP）、
- **幸運のチャンス**（Ł<span class="rpg-token token-stat">S</span>）、
- （オプションで）**才能**、
- **装備品**。

### 2.1 特徴 (<span class="rpg-token token-stat">S</span>/<span class="rpg-token token-stat">Z</span>/<span class="rpg-token token-stat">M</span>) — 用途

- **力 (<span class="rpg-token token-stat">S</span>)**: 近接戦闘、力仕事、荷物運搬、耐久性。
- **敏捷 (<span class="rpg-token token-stat">Z</span>)**: 射撃、精密さ、隠密、回避、アクロバット、車両運転。
- **力 (<span class="rpg-token token-stat">M</span>)**: ゲーム世界の「特殊効果」: 魔法、サイオニクス、信仰、スーパーテクノロジー、ハッキング、影響、直感 — コンベンションによる。

### 2.2 特性ダイス — その動作原理

各特性にはダイスがあります: <span class="rpg-token token-<span class="rpg-token token-d4">k4</span>"><span class="rpg-token token-d4">k4</span></span>、<span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>、<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>、<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span> または <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>。  
特性を使用する際には、その特性の**一つのダイス**を振ります。

- 大きなダイス = 成功と特別な成功（ダイスの最大値）を出す確率が高くなります。

**例:** あなたは機敏さが <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span> です。射撃、登攀、または隠密行動を行うときは、通常<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span> を振ります。

### 2.3 リソース: ハート、パワーポイント、および運の要素

- **ハート:** 初期値は5。攻撃やプレッシャーがハートを奪う。
- **パワーポイント (PP):** 初期値は3。これを消費して標準を超える力やプレイを行う。
- **運の要素 (WO):** 各セッションの初期値は2。シーンを「救う」ためやドラマ性を強調するために使う。



---

### ステップ1：コンセプトと役割

役割を選ぶ – これはあらゆるユニバースに適した基本的な行動スタイルです。

- **突撃**: リスクを取ってシーンを前進させます。  
  (例: 戦士、海兵隊、警備員、ハンター、野蛮人)
- **専門家**: 正確に計画とツールを使って行動します。  
  (例: 盗賊、スナイパー、斥候、ハッカー、パイロット、トラッカー)
- **達人**: 標準を超えたことを行います – 力、知識、影響力によって。  
  (例: 魔法使い、サイオニック、司祭、錬金術師、テクノマンティ、外交官)

### ステップ 2: 特性のダイスを割り当てる

ダイスを割り当てる: 一つの特性に <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>、一つに <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>、一つに <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>。

クイックヒント:
- **アサルト** は通常、最高に<span class="rpg-token token-stat">S</span>を持っています。
- **スペシャリスト** は通常、最高に<span class="rpg-token token-stat">Z</span>を持っています。
- **エデプト** は通常、最高に<span class="rpg-token token-stat">M</span>を持っています。

### ステップ 3: リソースの記録

- **ハート:** 5  
- **パワーポイント:** 3  
- **フォーチュン:** 2 (セッションの開始時にリフレッシュ)

### ステップ4（オプション）: 2つの才能を選択

才能は、何が得意か（ゲーム内で頻繁に登場するスキル）を表す短いフレーズです。
- 例: 「スカウト」、 「技術者」、 「医者」、 「交渉者」、 「アスリート」、 「アナリスト」、 「ハッカー」、 「儀式師」。

**才能の働き方:** 才能がテストに実際に役立つ場合、GMはそれをより良い状況として扱い、このロールで**ダイスを1段階上げる**ことができます。  
- 通常、1テストにつき1つの才能です。
- 才能は行動の説明を置き換えるものではなく、合理的な計画を強化するものです。

**例:** あなたは「技術者」の才能を持っており、緊急にジェネレーターを始動しようとしています。 GMはそれが助けになると判断し、このテストで<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>を<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>に上げます。

### ステップ5: 装備

記入してください:
- 1つの「重要な」道具（武器または職業用装備）、
- 1つの防護（鎧、盾、カモフラージュ – 世界に依存）、
- 3つの実用的なもの。

装備は通常、**許可**として機能します。何かを持っている場合、適切な行動を試みることができます。良い道具は、意味がある場合、良い状況を作り出す可能性もあります（ダイスプールの増加）。

### キャラクターの例（ユニバーサル）

- 役割: スペシャリスト  
- <span class="rpg-token token-stat">S</span> <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>, <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>  
- ハート 5、MP 3、LS 2  
- 才能: 「スカウト」、「交渉者」  
- 装備: 遠距離武器、ピックツール/ツールセット、ロープ、懐中電灯





---

### 4.1 あなたが判定を行う時

あなたが判定を行う時：
- 何かが**リスクがある**または不確かな場合、
- 失敗が**重大な結果**を伴う場合。

もし何かが明白であり、そしてプレッシャーがないならば、GMは「成功する」と判定を行わずに言うことができます。

### 4.2 難易度 <span class="rpg-token token-t">T</span>

GMは難易度を選択します：

- <span class="rpg-token token-t">T 3</span> 簡単  
- <span class="rpg-token token-t">T 4</span> 標準  
- <span class="rpg-token token-t">T 5</span> 難しい  
- <span class="rpg-token token-t">T 6</span> 非常に難しい  
- <span class="rpg-token token-t">T 8</span> 英雄的  
- <span class="rpg-token token-t">T 12</span> 伝説的

あなたは難易度を「推測」する必要はありません — GMが直接伝えます。

### 4.3 ロールの結果

- **1**: 結果に伴う失敗（合併症が確実に発生します）。
- **結果 < <span class="rpg-token token-t">T</span>**: 失敗（しかし、シーンはそのまま進む）。
- **結果 ≥ <span class="rpg-token token-t">T</span>**: 成功。
- **ダイスの最大値**（例えば、<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>での12、<span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>での20）：特別な成功 + 追加ボーナス。

**追加ボーナス**（例）：より速く、静かに、安全に、大きな効果、より良い位置、あなたにとってプラスの追加ディテール。

### 4.4 良い/悪い状況（ボーナスなし）

修正値を計算する代わりに、状況をプレイしましょう：

- **良い状況** → サイコロを1段階上げる  
  (<span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>)
- **悪い状況** → サイコロを1段階下げる  
  (<span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d4">k4</span>"><span class="rpg-token token-d4">k4</span></span>)

プレイヤーとしてのあなたの役割は: **良い条件を作り出す**、説明や決定を通して（遮蔽、準備、道具、計画、偵察）。

### 4.5 同盟者の支援

同盟者は自分のアクションを使ってあなたを支援することができます。その場合、その1回のロールで:
- ダイスのランクを1段階上げます。

支援にはストーリーにおける意味が必要です（注意をそらす、盾になる、道具を渡す、火力支援、もう一組の手）。

### テストの例（明確で完全）

見張りが来る前にロックされたドアを開けたい。
- マスター: 「これは敏捷です。<span class="rpg-token token-t">T 5</span>です。失敗：大きな音を立て、時間を失います。」
- あなたは敏捷<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>を持っていますが、ピッキングツールを使い、「ロックの専門家」の才能を持っています → より良い状況になり、<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>にアップグレードします。
- ロール<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span> = 6 → 成功: ドアは警報無しで開きます。

---



---

### 5) 幸運の分け前（Ł<span class="rpg-token token-stat">S</span>）— それを使うべき時

各セッションの始めに、あなたは**2 Ł<span class="rpg-token token-stat">S</span>**を持っています。Ł<span class="rpg-token token-stat">S</span>は次のためにあります:
- 重要なシーンを救うために、
- ドラマを追加するために、
- 大胆な決断を報いるために。

**1 Ł<span class="rpg-token token-stat">S</span>**を使って、以下のいずれかを選択してください:
- 自分のテストを**再ロール**する（良い結果を残します）、
- そのロールに対して**ダイスを1段階上げる**、または  
- **失敗を「コストを伴う成功」**に変更する — 行動は成功しますが、GMが即座に代償を加えます。

**Ł<span class="rpg-token token-stat">S</span>の回復:** 次のセッションの始めには、限度額に戻ります。GMは、大胆なリスク、素晴らしいストーリーの決断、または結果を伴うロールプレイングに対して**+1 Ł<span class="rpg-token token-stat">S</span>**を与えることができます。

**例:** 屋根と屋根の間のジャンプでの失敗は、ストリートへの落下を意味します。1 Ł<span class="rpg-token token-stat">S</span>を使って、失敗をコストを伴う成功に変更します: 跳躍に成功しますが、装備を失うか足首をひねります（次のシーンでの不利な状況）。



---

### 6.1 距離 (デフォルト設定、マップなし)

距離を4つの言葉で説明してください：
- **近い**（手が届く範囲）、
- **やや近い**（数歩）、
- **遠い**（シーンの反対側）、
- **非常に遠い**（狙撃レベル / 車両レベル）。

ターンには：**移動 + 1 アクション**があります。  
移動は通常、距離を1段階変更します（やや近い→近い など）。

### 6.2 オプション: グリッド上でのプレイ

もしマップ上でプレイする場合:
- 1 マス = 1–2 m,
- ターンでの移動: **最大5マス**, 
- 対角線は1マスとして数える,
- 他のルールは同じように機能します。

### 6.3 攻撃

- **近接:** 対象の**防御**に対して**力（<span class="rpg-token token-stat">S</span>）**のロール。
- **遠距離:** 対象の**防御**に対して**敏捷性（<span class="rpg-token token-stat">Z</span>）**のロール。

**敵の防御（参考値）：**
- <span class="rpg-token token-t">4</span> 弱い
- <span class="rpg-token token-t">5</span> 一般的
- <span class="rpg-token token-t">6</span> エリート
- <span class="rpg-token token-t">8</span> ボス
- <span class="rpg-token token-t">12</span> 伝説のボス

### 6.4 カバーと位置

- カバー内の目標 / 悪い角度 / 圧力 → より悪い状況 (ダイスを下げる)。
- 良い位置 / 驚き / 数的優位 → より良い状況 (ダイスを上げる)。

### 6.5 命中とダメージ

- 命中は**1ハート**を与えます。
- クリティカルヒットは**2ハート**を与えるか、強力な効果（武装解除、倒す、押しのける、カバーから追い出す）をもたらします。

### 6.6 0 ハート

あなたが **0 ハート** に落ちたとき、行動不能になります（負傷、気絶、衝撃などテーマによる）。
- 味方がアクションを消費して、あなたを **1 ハート** に立ち戻らせることができます。
- プレッシャーが続いている場合、あなたの優先は防御と退避であり、「タンク」ではありません。

### 短いターンの例（グリッドなし）

- あなたは**近く**にエリートがいます。
- 移動: **近く**まで移動し、柱（カバー）の後ろに入ります。
- アクション: 近接攻撃 (<span class="rpg-token token-stat">S</span>)。エリートの防御は<span class="rpg-token token-t">6</span>です。あなたの<span class="rpg-token token-stat">S</span>は<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>です。
  9を振る：成功、エリートはハートを1失います。



---

### 7) 権力と特技（パワーポイント）

「力」と呼ばれるものは世界によって異なります：魔法、サイオニクス、信仰、ガジェット、ハッキング、スーパートリック。

### 7.1 力の使い方

1) 効果を説明する。
2) ゲームマスターが難易度とMPのコストを伝える。
3) MPを消費し、**力 (L)** を振る。

### 7.2 効果レベル (T / コスト)

- **トリック:** 短時間の効果、トリック → <span class="rpg-token token-t">T 4</span>、コスト 0–1 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>
- **スタンダード:** 攻撃、防御、インパルス → <span class="rpg-token token-t">T 5</span>、コスト 1 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>
- **強力:** 範囲、回復、麻痺、ライブハッキング → <span class="rpg-token token-t">T 6</span>、コスト 2 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>
- **大規模:** シーンの変化、強力な干渉 → <span class="rpg-token token-t">T 8–12</span>、コスト 3 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>

### 7.3 失敗と特別な成功

- 失敗: 発行された<span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>は失われ、結果が生じます（過負荷、痕跡、位置の喪失、副作用）。
- ダイスの最大: 特別な成功 + 追加のメリット（より大きな範囲、より長い時間、より強力な効果、または「副作用」の軽減）。

### 7.4 <span class="rpg-token token-power">PM</span>回復

- 戦闘シーンの後、**1 <span class="rpg-token token-power">PM</span>**を回復します。
- 安全な休息の後、完全に回復します（ゲームの世界がそれを許す場合）。

**例（ファンタジー）:** 「ショートジャンプ」 – 標準、<span class="rpg-token token-t">T 5</span>、コスト1 <span class="rpg-token token-power">PM</span>。
**例（SF）:** 「電子ロックオーバーロード」 – 標準、<span class="rpg-token token-t">T 5</span>、コスト1 <span class="rpg-token token-power">PM</span>。



---

### 8) 休息と回復

安全な瞬間がある場合（避難、手当て、サービス、食事）: 
- **ハート**を完全に回復します。
- そして、あなたのセッションの休息ルールに従って**MP**を補充します。

より過酷なキャンペーンでは、GMはすべてを取り戻すために完全な停止を要求することができます。

---



---

### 9) キャラクターの成長（「レベルアップ」するとき）

成長は**冒険の後**に発生します（通常は1～3セッション後、キャンペーンのペースに依存）。  **一つ**を選びます:  - 1つの特性を1段階上げ、ダイスの階級を上げる（最大<span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>まで）、または - +1 ハート（最大7）、または - +1 MP（最大5）、または - 新しい特技 （GM と合意した短い一文のルール）。  **例:** 器用さが<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>から<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>に上がります。今後、全ての<span class="rpg-token token-stat">Z</span>テストは<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>で行います。



---

### 10) 「<span class="rpg-token token-d6">d6</span>のみ」のバリアント: 2d6

もし<span class="rpg-token token-d6">d6</span>のみでプレイしたい場合:
- すべてのテストは**2d6 + 特性修正値**です。
- 初期の特性修正値: 一つの特性**+2**、一つは**+1**、一つは**+0**。

**結果:**
- **6以下** – 結果は失敗し、結果に影響する要素が追加されます  
- **7–9** – 成功しますが、何かしらのコストがあります  
- **10以上** – 完全成功  
- **12** – 卓越した成功

**状況:** 代わりにスロールのしきい値を変更するのではなく、**+1 / -1**をロールに追加します（有利 / 不利）。

**2d6の幸運:** 同じく動作しますが、「サイコロを増やす」ことに代わり、ロールに**+1**を追加します。

---



---

### 11) プレイヤーの良い習慣

- 言う: **何をする + なぜ**。行動の目的がゲームマスターに賭け金を設定するのを助ける。
- 難易度が高い場合: 「ロールを無理にやらない」 — **状況を変える**（準備、道具、カバー、援助、別の道）。
- 協力する: 同盟者の援助は、システム内で最も強力で簡単なレバレッジの1つ。
- 戦闘では位置が勝利を決める: カバー、距離、状況の利点はしばしば統計よりも重要。

