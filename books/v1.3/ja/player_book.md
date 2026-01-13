---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.3
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
generated_at: "2026-01-13T12:23:32.622Z"
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
# プレイヤーの書



---



---

### MGは状況を説明し、何が可能かを言います。
- あなたは、**何をするか**と**どんな結果を望んでいるか**を話します。
- 結果が不確実な場合、MGは言います。

- MGは状況を説明し、何が可能かを述べます。
- あなたは、**何をするか**と**どんな結果を望むか**を言います。
- 結果が不確実な場合、MGは次のことを言います：
  1) どの特性を使用するか（S/Z/M）、
  2) 難易度は何か（<span class="rpg-token token-tn">TN</span>）、
  3) 失敗した場合に何が起こるか。
- あなたは**自分の特性のサイコロを1つ振り**、結果が≥ <span class="rpg-token token-tn">TN</span>かどうかを確認します。

### 最短の原則  
**特性のサイコロを振る。結果 ≥ <span class="rpg-token token-tn">TN</span> = 成功。**



---

### 1. はじめに

あなたのキャラクターは以下の要素を持っています：
- **役割**（戦士 / 盗賊 / 魔法使い）、
- 3つの**特性**：力（S）、敏捷性（Z）、魔法（M）、
- **ライフ**（ハート）と**マナ**、
- 2つの**才能**（オプションですが推奨）、
- 装備。

### 2.1 特徴 (S/Z/M) — 何のために
- **力 (S)**: 近接戦闘、押しのけ、持ち上げ、耐久力。
- **敏捷性 (Z)**: 射撃、精度、隠密、回避、アクロバット。
- **魔法 (M)**: 「特別な」効果（魔法/サイコニクス/テクノロジー — ゲームによって異なる）。

### 2.2 特徴のサイコロ
各特徴にはそのサイコロがあります（例：<span class="rpg-token token-d6">d6</span>、<span class="rpg-token token-d8">d8</span>、<span class="rpg-token token-d10">d10</span>、<span class="rpg-token token-d12">d12</span>、<span class="rpg-token token-d20">d20</span>）。常に**1つの**サイコロを振ります。
- 大きなサイコロ = 高い結果が出る可能性が高くなります。

### 2.3 生命とマナ
- **生命:** 5 ハート（スタート）。
- **マナ:** 3（スタート）。魔法を使用する際に消費します。



---

### ステップ 1: 役割を選択
1 つの役割を選択します。初期の属性ダイスを設定します:
- **戦士:** S <span class="rpg-token token-d10">d10</span>, Z <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d6">d6</span>
- **盗賊:** S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
- **魔法使い:** S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d10">d10</span>

### ステップ2: 資源を記録する
- 生命: 5 ハート
- マナ: 3

### ステップ3: 2つの才能を選択する（オプション）
才能は、あなたが得意なことを説明する短いフレーズです。
- 中立的な例: 「交渉者」、「偵察者」、「メカニック」、「医療者」、「アスリート」、「アナリスト」、「ハッカー」。

**才能の働き:** 才能がテストに実際に役立つ場合、GMは**難易度（<span class="rpg-token token-tn">TN</span>）を1段階下げることができます**。
- 通常、1つのテストにつき1つの才能。
- 才能は行動の説明を置き換えるものではなく、実際に意味がある場合に助けになります。

### ステップ4: 装備
以下をリストアップしてください：
- 1つの戦闘用具（近接または遠距離）、
- 防具（適用される場合）、
- 3つの実用的なアイテム。

このゲームにおける装備は、最も一般的に**「許可」**として機能します：何かを持っているので、特定の行動を試みることができます。

### キャラクターの例
- 役割: ローグ
- S [token:<span class="rpg-token token-d6">d6</span>], Z [token:<span class="rpg-token token-d10">d10</span>], M [token:<span class="rpg-token token-d6">d6</span>]
- 生命 5, マナ 3
- タレント: 「スカウト」、「交渉者」
- 装備: 遠距離武器、ピッキングツール、ロープ、懐中電灯



---

### 4.1 いつ振るか
振るのは以下のときです：
- 何かが**リスクがある**または不確実なとき、
- そして失敗に結果が伴うとき。

もし何かが明白でプレッシャーがない場合、MGは「成功する」と言うことができます。

### 4.2 難易度 (<span class="rpg-token token-tn">TN</span>)
使用される4つのレベル：
- **<span class="rpg-token token-tn">TN</span> 4 — 簡単**
- **<span class="rpg-token token-tn">TN</span> 6 — 普通**
- **<span class="rpg-token token-tn">TN</span> 8 — 難しい**
- **<span class="rpg-token token-tn">TN</span> 12 — 英雄的**

MGが<span class="rpg-token token-tn">TN</span>を選択します。あなたはそれを「推測」する必要はありません — MGが単に難易度を教えてくれます。

### 4.3 投擲結果

**難易度 (<span class="rpg-token token-tn">TN</span>)**: 4 (簡単)、6 (普通)、8 (難しい)。

**ロール結果:**
- **1**: 失敗 + 複雑化。
- **< <span class="rpg-token token-tn">TN</span>**: 失敗。
- **≥ <span class="rpg-token token-tn">TN</span>**: 成功。
- **Max (10/20)**: 成功 + 利益。

### 4.3 投げの結果
- **結果 ≥ <span class="rpg-token token-tn">TN</span>:** 成功。
- **結果 < <span class="rpg-token token-tn">TN</span>:** 失敗。
- **1が出た:** 複雑な失敗。
- **サイコロの最大値**（例: <span class="rpg-token token-d10">d10</span>で10が出た場合）: 特別な成功 + 追加の利益。

**追加の利益**（例）: より速く、より静かに、より安全に、より大きな効果、より良いポジション。

### 4.4 難易度の「1段階」変更
ボーナスを計算する代わりに、GMは時々<span class="rpg-token token-tn">TN</span>を1段階変更します：
- 悪条件 → <span class="rpg-token token-tn">TN</span>が上昇（例：6 → 8）、
- 良条件 → <span class="rpg-token token-tn">TN</span>が下降（例：8 → 6）。

プレイヤーとしてのあなたの役割：**説明や決定を通じて良い条件を作り出す**（遮蔽、準備、道具、計画）。

### 4.5 同盟者の助け
同盟者は自分のアクションを使ってあなたを助けることができます。その場合、その1回のロールで次のことができます：
- サイコロを1サイズ上げる: **<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>**。

助けは説明において意味を持たなければなりません（例：防御、注意をそらす、道具を渡すなど）。

### テストの例
あなたは閉ざされた通路を素早く開けたい。
- MG: 「それは器用さ、<span class="rpg-token token-tn">TN</span> 6です。」
- <span class="rpg-token token-d10">d10</span>を振って7が出る → 成功: 通路が開いた。



---

### 1 短い

- **1 マス** は基本的な距離の単位です。
- ターンでは **最大5マスの移動** が可能です。
- 斜めに移動することもできます（斜め移動も1マスとしてカウントされます）。
- カバーは重要です：もし何かが遠距離攻撃からあなたを隠している場合、通常は命中が難しくなります。



---

### 6.1 ターンの進行
自分のターンでは、次のことができます：
- **移動**（最大5マスまで）、
- **1アクション**。

アクションには、攻撃、装備の使用、特性のテスト、助けること、魔法の使用などがあります。

### 6.2 攻撃

1) 目標を選択します（視界内で、かつ距離内にあるもの）。
2) 武器または魔法を選択します。
3) 使用する特性を確認します（例：近接攻撃の力、遠距離攻撃の敏捷性、魔法の呪文）。
4) **振ります。** 相手の**難易度（<span class="rpg-token token-tn">TN</span>）**と比較します。

### 6.2 攻撃
- **近接:** **力（S）**のロール。
- **遠距離:** **敏捷性（Z）**のロール。
- GMが相手の難易度（<span class="rpg-token token-tn">TN</span>）を言います。

敵のデフォルトの難易度（<span class="rpg-token token-tn">TN</span>）:
- **雑兵:** <span class="rpg-token token-tn">TN</span> 6
- **エリート:** <span class="rpg-token token-tn">TN</span> 8
- **ボス:** <span class="rpg-token token-tn">TN</span> 12

### 6.3 ヒットの意味

- **パチョレク**: 死亡（または戦闘から脱落）。
- **エリート/ボス**: **1 ハート**を失う。
- **プレイヤー**: **1 ハート**を失う（ただし、アーマーを持っている場合は、アーマーが攻撃を吸収するが、消耗する）。

### 6.3 ヒットの意味
- コーンをヒット → 戦闘から退場。
- エリート/ボスをヒット → ダメージを受ける（ボスは通常3回のダメージを受ける）。
- エリート/ボスに対する特別な成功 → 通常は+1のダメージを与える（合計で2）、または状況的な利点を1つ得る（例：遮蔽からの押し出し）。

### 6.4 箱と「報復」

戦闘にはリスクがあります。もし**当たらなかった場合**（結果 < <span class="rpg-token token-tn">TN</span>）や**1**を出した場合：
- 敵が反撃します：**1ハート**を失います。
- または、他の論理的な複雑さが発生します（例：武器を失う、倒される）。

*これは敵のターンではありません — あなたの失敗した攻撃の結果です。*

### 6.4 Pudłoと「報復」
もし**外す**（結果 < <span class="rpg-token token-tn">TN</span>）場合、相手が実際にあなたに届く可能性があった場合、**1ハート**を失います。
- 接近戦ではこれはよくあります。
- 遠距離攻撃では、カバーや状況に大きく依存します。

あなたの戦術的なレッスン：**外したときに報復を受けないように位置を取る**（カバー、距離、計画、助け）。

### 6.5 0 サーク

もし0ハートに落ちた場合：
- あなたは**倒れた**状態です。
- 行動を行うことができません（這うことと、残りの力で話すことだけが可能です）。
- 同盟者があなたを「起こす」ことができます（助けのアクション）、これにより1ハートが回復します。
- 倒れた状態でダメージを受けると、**消滅**します。

### 6.5 0 Serc
0 Sercの状態に落ちた場合：
- あなたは倒れていて行動を行うことができません。
- 同盟者はアクションを消費して、あなたを立たせることができます。**1 Serc**を回復します。

### 短いターンの例
- 移動: 3マス前進して遮蔽に入る。
- アクション: 射撃（Z）。MG: 「難易度6だが、目標は遮蔽の後ろにいる → 難易度8」。<span class="rpg-token token-d10">d10</span>を振る=9 → 命中。



---

### 1. はじめに

7.2 特殊効果の魔法とメカニクス

### 7.1 コストとレベル
- **トリック:** <span class="rpg-token token-tn">TN</span> 4、コスト 0–1
- **スタンダード:** <span class="rpg-token token-tn">TN</span> 6、コスト 1
- **強力な効果:** <span class="rpg-token token-tn">TN</span> 8、コスト 2
- **大きな力:** <span class="rpg-token token-tn">TN</span> 12、コスト 3

### 7.2 マジックの失敗
マジックが失敗した場合：
- 消費したマナを失います。
- 結果が発生します（例：−1 ハート、ポジションの喪失、追加の脅威）。

### 7.3 特殊な成功
魔法のサイコロの最大値は追加の利点を提供します：
- より広い範囲/エリア、
- より長い持続時間、
- より高い効果、
- またはコストの削減（GMは1マナを返すことができます）。

### 魔法の例
5マスの短い「ジャンプ」を行いたいです。
- GM: 「これは標準: <span class="rpg-token token-tn">TN</span> 6、コストは1です。」
- 1マナを支払い、M <span class="rpg-token token-d10">d10</span>=7を振る → 成功: 障害物を越えます。



---

### 1. はじめに

ポコンフリクト後、安全な瞬間と基本的な休息条件があれば：
- 生命とマナが完全に回復します。



---

### 1. はじめに

冒険の後、**1つ**を選択します：
- S/Z/Mのサイズを1つ上げます：<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>、
- または+1 ハート（最大7）、
- または+1 マナ（最大5）。

これは、追加のサイコロを振ることなく成長を意味します。



---

### 1. はじめに

もしテーブルに<span class="rpg-token token-d6">d6</span>しかない場合、サイコロのサイズの代わりに成功の閾値があります：
- マスター 3+, 熟練者 4+, 新人 5+, スキルなし 6。

GMは状況や助けに応じて閾値を1段階上げたり下げたりすることができます。



---

### 常に話す

- いつも言うこと: **何をする** + **なぜ**。 「レバーを引きたい」は良いですが、「通路を閉じるためにレバーを引きたい」はさらに良いです。
- <span class="rpg-token token-tn">TN</span>が高い場合: 「投げを苦しめる」ではなく、状況を変えましょう（カバー、道具、助け、別の道）。
- 協力を確立しましょう: 一人が助け、もう一人がテストを実行します。
- 戦闘ではカバーとポジションを尊重してください — しばしばそれは投げ自体よりも重要です。

---
プレイヤーガイドの終わり。

