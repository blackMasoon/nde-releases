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
generated_at: "2026-01-15T07:57:22.428Z"
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
# スタート (要約)



---



---

### 1) 1分でヒーロー


* **コンセプト:** あなたは誰で、どのジャンルでプレイしますか（1文）。
* **ロール（1つ選択）:**

  * **アサルト** – プレッシャー、戦闘、障害の突破
  * **スペシャリスト** – スニーク、精度、技術、観察
  * **アデプト** – 力、知識、影響、即興
* **特徴（3つ）:**

  * **力 (<span class="rpg-token token-stat">S</span>)** – 物理的な力、耐久性、近接戦闘
  * **敏捷性 (<span class="rpg-token token-stat">Z</span>)** – 反射神経、スニーク、射撃、操縦
  * **魔力 (<span class="rpg-token token-stat">M</span>)** – 魔法/サイコニクス/テクノロジー/ブラフ/直感（世界による）
* **特徴のサイコロ:** 1つの特徴に**<span class="rpg-token token-d12">k12</span>**、1つに**<span class="rpg-token token-d8">k8</span>**、1つに**<span class="rpg-token token-d6">k6</span>**（ロールに応じて選択）。
* **ハート:** 5. **マジックポイント:** 3（力や「特別なプレイ」に使用）。
以下に「1ページ」スタイルの短いルールのための準備されたセクションがあります（バリアントA）。

**幸運の一撃（動作方法）:** **1幸運ポイント**を消費して、1つを選択:

* **テストの再ロール**（より良い結果を残す）、または
* **その1回のロールでサイコロを1段階上げる**（**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>**）、または
* **失敗を「コストのある成功」に変える** — アクションは成功するが、GMはすぐに代償を追加する（例: 時間を失う、音を立てる、リソースを消費する、悪い位置に終わる、注意を引く、装備を壊す）。

**幸運ポイントの回復:** 次のセッションの開始時に制限に戻ります。GMは大胆なリスク、素晴らしいストーリーの決定、または結果を考慮して**+1幸運ポイント**を与えることができます。

* **装備:** 1つの「キー」ツール（例: 剣、ライフル、ハッキングキット）、1つの防具（アーマー、エネルギーシールド、カモフラージュ）、コンセプトに合った3つの小物。

**例:** スペシャリスト: <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">k6</span>。サイバーパンクでは<span class="rpg-token token-stat">M</span>は「ハッキング/影響」であり、ファンタジーでは<span class="rpg-token token-stat">M</span>は「魔法/意志」です。



---

### 2) アクションの解決方法

1. プレイヤーは**何をするか**と**どのように**（ゲームの世界での説明）を言います。
2. GMは**難易度**と賭け（「失敗した場合に何が起こるか」）を決定します。
3. 特徴のサイコロ（<span class="rpg-token token-stat">S</span>/<span class="rpg-token token-stat">Z</span>/<span class="rpg-token token-stat">M</span>）を振り、難易度と比較します。

**難易度 (T):**

* **3** 簡単、**4** 標準、**5** 難しい、**6** 非常に難しい、**8** 英雄的、**12** 伝説的。

**サイコロの結果:**

* **1** – 失敗と結果（必ず複雑化が発生）。
* **< T** – 失敗（しかしシーンは続行：時間の浪費、騒音、悪化した状況、資源の喪失）。
* **≥ T** – 成功。
* **サイコロの最大値**（例：<span class="rpg-token token-d12">k12</span>で12、<span class="rpg-token token-d20">k20</span>で20） – 特別成功：追加の利点を得る。

**修正なしの修正:**

* **良い状況**: サイコロを1段階上げる（<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>）。
* **悪い状況**: サイコロを1段階下げる（<span class="rpg-token token-d20">k20</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d4">k4</span>）。
* **仲間の助け**（彼のアクションを消費する）: サイコロを1段階上げる。

**例:** アデプトがアラームとストレスの中でポータルを閉じようとする（<span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span>）→悪い状況で<span class="rpg-token token-d6">k6</span>に下がる。T = 5。サイコロの結果6: 成功、しかし「アラーム」は物語のプレッシャーとして背景に残る。



---

### 3) 移動と戦闘 - デフォルトはグリッドなし、オプションとしてグリッド

**デフォルト: マインドシアター（推奨）**

* 距離を次のように説明します: **近い**（手の届く範囲）、**遠くない**（数歩）、**遠い**（舞台の反対側）、**非常に遠い**（スナイパー/車両）。
* ターンでは: **移動 + 1 アクション**。

  * 移動は通常、距離を1「段階」変更します（遠くない→近いなど）。
* **攻撃**: **<span class="rpg-token token-stat">S</span>**（近接）または **<span class="rpg-token token-stat">Z</span>**（遠距離）のロールを目標の**防御**に対して行います。

**敵の防御（目安）:**

* **弱い** 4, **通常** 5, **エリート** 6, **ボス** 8（伝説のボス 12）。

**ヒットの効果（迅速な戦闘）:**

* ヒットは **1 ハート** を与えます。
* 特殊成功は **2 ハート** を与えるか、強力な効果（武装解除、転倒、分散）をもたらします。

**カバーとポジショナルアドバンテージ:**

* 軽いカバー / 不利な角度: 攻撃者のサイコロを1段階下げます。
* 良い位置 / 不意打ち: サイコロを1段階上げます。

**オプション: グリッドでのプレイ**

* 1マス = 1–2 m。ターン中の移動: **最大5マス**。その他のルールは変更なし。

**例:** スペシャリストがカバーから（<span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">d12</span>）エリート（防御6）に向けて射撃します。ターゲットは軽いカバーにいる → <span class="rpg-token token-stat">Z</span>は<span class="rpg-token token-d8">d8</span>に下がります。ロール7: 成功、1ハートのダメージ。



---

### 4) 力、魔法、特殊なプレイ（汎用）

これには魔法、サイコニクス、サイバネティクス、ガジェット、映画のトリックが含まれます - 世界に応じて。

* 標準を**超える**ことをする場合：**パワーポイント**を消費し、**<span class="rpg-token token-stat">M</span>**を振ります。
* 効果のレベルを決定します：

**力のレベル（T / コスト）：**

* **トリック**（短い効果、トリック、「フラッシュ」）：**T 4 / 0–1 <span class="rpg-token token-power">PM</span>**
* **標準**（攻撃、シールド、小さなコントロール）：**T 5 / 1 <span class="rpg-token token-power">PM</span>**
* **強力**（エリア、治療、麻痺、リアルタイムハック）：**T 6 / 2 <span class="rpg-token token-power">PM</span>**
* **大きな**（シーンの変更、強力な介入）：**T 8–12 / 3 <span class="rpg-token token-power">PM</span>**

**失敗：** <span class="rpg-token token-power">PM</span>は失われ、結果は即座に発生します（オーバーロード、デジタルトレース、儀式のひび、望ましくない注意）。

**回復：** 衝突シーンの後に**1 <span class="rpg-token token-power">PM</span>**を回復し、安全な休息の後に完全に回復します。

**例：** スペースオペラでアデプトがドローンの「センサーを曲げる」ことを試みます：標準、T 5、コスト1 <span class="rpg-token token-power">PM</span>。<span class="rpg-token token-stat">M</span>を振る<span class="rpg-token token-d8">k8</span> = 8：特別な成功 - ドローンは信号を失い、道を誤ります。



---

### 5) 落下、リスク、治療

* あなたが **0 ハート** に落ちると、あなたは **行動から除外されます**（負傷、気絶、ショック – コンベンションによる）。
* 同盟者はアクションを消費して、あなたを **1 ハート** に戻すことができます（応急処置、アドレナリン、システムの再起動）。
* シーンの後、少しの休息があれば：あなたは **完全なハート** に戻ります、条件があれば（避難所、包帯、サービス、食事）。
* シーンが特に残酷だったり、敵が優位にある場合、GMは「完全なリセット」が安全な停車を必要とすることを要求することがあります。

**例:** ストームが0に落ちる。スペシャリストは彼を遮蔽の後ろに引きずり、アクションを消費する：ストームは1ハートに戻り、次のターンで行動できます。



---

### 6) キャラクターの成長（テーブルや会計なしのキャンペーン）

冒険の後、**1つ**選んでください：

* **1つの能力を1段階上げる**（最大<span class="rpg-token token-d20">k20</span>まで）、または
* **+1 ハート**（最大7）、または
* **+1 力ポイント**（最大5）、または
* **新しい特技**（GMと合意した短い一文のルール）。

**特技の例（汎用）：**

* **圧力：** シーンごとに、近接攻撃が命中したとき、+1 ハートのダメージを与えます。
* **影：** 隠れて行動する際、サイコロを1段階上げます。
* **火花：** シーンごとに1PMを消費することで、ロールなしで「コストを伴う成功」を自動的に得ることができます。

**例：** アデプトは<span class="rpg-token token-stat">M</span>を<span class="rpg-token token-d8">k8</span>から<span class="rpg-token token-d12">k12</span>に上げます – これで彼の力はT 5–6でより安定して発動します。



---

### 7) バリアント「<span class="rpg-token token-d6">k6</span>のみ」モード**2k6**（迅速かつ非常にプレイしやすい）


もしあなたがサイコロのセットを持っていないか、より「物語的」な結果を望む場合：

* 各テストは：**2k6 + 特徴修正値**を振る。
* **特徴修正値**は開始時に選択：1つの特徴は**+2**、1つは**+1**、1つは**+0**。
* 結果：

  * **6以下** – 失敗と結果
  * **7–9** – コストを伴う成功（妥協、資源の喪失、悪化した状況）
  * **10以上** – 完全な成功
  * **12** – 特別な成功（追加の利益）

**状況の難易度：**しきい値を変更する代わりに、振りに**+1 / -1**を加える（助ける / 妨げる）か、7–9の場合のコストを設定する。

**特徴-サイコロバージョンへのマッピング（互換性が必要な場合）：**

* <span class="rpg-token token-d6">k6</span> ≈ +0, <span class="rpg-token token-d8">k8</span> ≈ +1, <span class="rpg-token token-d12">k12</span> ≈ +2, <span class="rpg-token token-d20">k20</span> ≈ +3（非常に経験豊富なキャラクター用）。

**例:** 専門家が走りながら射撃：<span class="rpg-token token-stat">Z</span> = +2、困難な状況（-1）。2k6を振る = 8、合計9：コストを伴う成功 – 命中するが、露出した位置に終わる。

