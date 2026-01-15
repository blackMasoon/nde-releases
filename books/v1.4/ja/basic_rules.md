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
generated_at: "2026-01-15T08:02:46.355Z"
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
# 基本ルールブック



---



---

### ゲームに必要なもの

- 鉛筆とキャラクターシート。
- （オプション）マップ/グリッドとキャラクターマーカー（方眼紙、マット、VTT）。
- サイコロ: **<span class="rpg-token token-d4">k4</span>, <span class="rpg-token token-d6">k6</span>, <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-d20">k20</span>**。
  - 実際には、**各サイコロを1つずつ**用意すれば十分です（1回に1つのサイコロを振ります）。
  - （オプション）ランダムテーブルやジェネレーター用の**k100**。
- もし**<span class="rpg-token token-d6">k6</span>**しか持っていない場合は、**2k6**のバリアントを使用してください（最後に）。

---



---

### 用語集


これらの言葉はルールに登場します — ここでは「人間的に」説明されています：

- **GM (ゲームマスター)**: 世界を導き、状況を説明し、敵を操り、難易度と結果を決定します。
- **プレイヤー**: 自分のキャラクターの行動を説明し、サイコロを振ります。
- **テスト**: 不確実な結果を決定するためのサイコロの振り。
- **特性**: **力 (<span class="rpg-token token-stat">S</span>)**、**敏捷性 (<span class="rpg-token token-stat">Z</span>)**、**魔力 (<span class="rpg-token token-stat">M</span>)**。これらは、*どのサイコロを振るか*を示します。
- **特性のサイコロ**: 特性に割り当てられたサイコロのサイズ（例: <span class="rpg-token token-stat">Z</span> = <span class="rpg-token token-d12">d12</span>）。
- **難易度 (T)**: 行動が成功するために達成または超えなければならない数値。
- **成功**: 結果 ≥ 難易度。
- **特別な成功**: サイコロの**最大結果**（例: <span class="rpg-token token-d12">d12</span>で12、<span class="rpg-token token-d20">d20</span>で20） — 成功 + 追加の利益。
- **複雑さ**: 失敗後の追加の問題（騒音、時間の損失、不利な位置、資源の喪失）。
- **コストを伴う成功**: 行動は成功するが、代償を支払う（妥協、資源の喪失、暴露、リスク）。
- **幸運の一撃 (Ł<span class="rpg-token token-stat">S</span>)**: シーンを救うための限られたリソース（再ロール / サイコロの上昇 / 失敗をコストを伴う成功に変える）。
- **ハート**: キャラクターの「命」（耐久力、傷、コンディション — 世界によって異なる）。
- **マジックポイント (<span class="rpg-token token-power">PM</span>)**: 標準を超えた力や行動のためのリソース（魔法、サイコニクス、ガジェット、「映画的」アクション）。
- **防御**: 戦闘における敵の命中閾値（防具や防御クラスなどのルールを掛け算する代わりに）。
- **遮蔽**: あなたとターゲットの間の障害物。通常、遠距離攻撃や観察行動を困難にします。

---



---

### 1. キャラクター


キャラクターの作成は短いです。キャラクターとは: **コンセプト + 役割 + 特徴 + 資源 + 装備**。

---

### 1.1 コンセプト

一文で: あなたは誰で、どのジャンルでプレイしていますか。

> 例: 「かつての企業エージェント、今は静かに行動し、誰にも信頼を置かない賞金稼ぎ。」

### 1.2 役割 (1つ選択)

役割は意図的に「世界に中立」です。ファンタジーでは別の名前を付けることができ、サイバーパンクでは別の名前を付けることができますが、同じように機能します。

- **突撃** — プレッシャー、戦闘、障害物の突破、前線の突破。
- **スペシャリスト** — ステルス、精度、技術、観察、計画。
- **アデプト** — 力、影響、知識、即興（魔法/サイオニクス/テクノロジーは世界によって異なる）。

### 1.3 特徴とサイコロ


あなたには三つの特徴があります:

- **力 (<span class="rpg-token token-stat">S</span>)** — 物理的な力、耐久力、近接戦闘、押しのけ。
- **敏捷性 (<span class="rpg-token token-stat">Z</span>)** — 反射、精度、隠密、射撃、操縦。
- **魔力 (<span class="rpg-token token-stat">M</span>)** — 「特別なもの」：魔法、サイオニクス、高度な技術、社会的なブラフ、直感 — コンベンションに応じて。

**最初にサイコロを次のように分配します:**
- 一つの特徴に **<span class="rpg-token token-d12">k12</span>**、
- 一つに **<span class="rpg-token token-d8">k8</span>**、
- 一つに **<span class="rpg-token token-d6">k6</span>**。

**役割に応じた推奨の分配（最も簡単な方法）:**
- **突撃:** <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d6">k6</span>
- **専門家:** <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">k6</span>
- **見習い:** <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">k6</span>

> 例: もしあなたの <span class="rpg-token token-stat">Z</span> = <span class="rpg-token token-d12">k12</span> であれば、射撃、隠密、回避の際には通常 <span class="rpg-token token-d12">k12</span> を振ります。

### 1.4 リソース

- **ハート:** 5.
- **マジックポイント (MP):** 3.
- **ラッキー・ポイント (LP):** 各セッションの開始時に **2 LP** を持っています。

**ラッキー・ポイント（効果）:** **1 LP** を消費して、次のいずれかを選択します:
- **テストの再ロール**（より良い結果を残す）、または
- **その1回のロールのサイコロを1段階上げる**（**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>**）、または
- **失敗を「コストを伴う成功」に変える** — 行動は成功しますが、GMはすぐに代償を追加します（例: 音、時間の損失、リソースの損失、悪い位置、注意を引く、装備の損傷）。

**LPの回復:** 次のセッションの開始時に制限に戻ります。GMは大胆なリスク、素晴らしいストーリーの決定、または結果を考慮したプレイに対して **+1 LP** を与えることがあります。

### 1.5 タレント（オプショナルだが推奨）

タレントは、あなたのキャラクターが得意とすることを説明する**2つの短いフレーズ**です（リストや表なし）。

- 例： 「メカニック」、「スカウト」、「交渉者」、「メディック」、「ハッカー」、「ベテラン」、「探検家」。

**タレントの働き方：**タレントがテストに実際に役立つ場合、GMは**サイコロを1段階上げる**ことができます（または難易度を中和することができます）。
- タレントは自動的な成功を与えません。
- 通常、**最大1つのタレント**が1つのテストに影響を与えます。

### 1.6 装備

リストアップしてください:
- 1つの「キー」ツール（武器 / セット / あなたの仕事に必要な装備）、
- 1つの防具（鎧、盾、カモフラージュ — 世界によって異なる）、
- 冒険に役立つ小物を3つ。

ルールのコアにおける装備は主に**許可**（アクションを可能にする）であり、数値的なボーナスではありません。

### 1.7 完全なキャラクターの例

- コンセプト: 「情報を盗む盗賊、ポケットからではなくシステムからデータを盗む。」
- 役割: スペシャリスト
- 特徴: <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">k6</span>, <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span>
- リソース: 5 ハート, 3 <span class="rpg-token token-power">PM</span>, 2 Ł<span class="rpg-token token-stat">S</span>
- タレント: 「ハッカー」、「影」
- 装備: ピストル, 軽装甲, 侵入セット, ロープ, 懐中電灯

---



---

### 2. 基本ルール: テスト

この部分が最も重要です — もしあなたがこれを理解しているなら、あなたはシステムを理解しています。

### 2.1 テストを行う時


テストは、次の2つの条件が満たされるときに行います：
1) 結果が不確実である（成功するかもしれないし、失敗するかもしれない）、および
2) 賭けが現実的である（失敗が何かを変える/何かを費やす）。

もし行動が単純でプレッシャーがない場合、GMはサイコロを振らずに「成功した」と言うことができます。

### 2.2 テストの実行方法 (ステップバイステップ)

1) プレイヤーは **何をするか** と **その理由** を言います。
2) GMは特性を選びます: **<span class="rpg-token token-stat">S</span>** または **<span class="rpg-token token-stat">Z</span>** または **<span class="rpg-token token-stat">M</span>**。
3) GMは **難易度 (T)** を設定し、失敗の意味（賭け）を説明します。
4) プレイヤーは **特性のサイコロ** を振ります。
5) 結果をTと比較し、影響を判断します。

### 2.3 難易度 (T)


使用簡單的門檻。如果你有疑問——選擇較低的門檻，而「難易度」則通過後果來顯示。

- **T 3** – 簡單（幾乎肯定成功，但有時在壓力下值得檢查）
- **T 4** – 標準（典型挑戰）
- **T 5** – 困難（需要能力或優勢）
- **T 6** – 非常困難（沒有優勢會有風險）
- **T 8** – 英雄級（對於最佳者或經過良好準備）
- **T 12** – 傳說級（很少「純粹」；通常作為戰役目標、計劃、儀式、大條件）

### 2.4 テストの結果

- **結果 ≥ T → 成功。** 目的の効果を達成します。
- **結果 < T → 失敗。** 効果を達成できず、状況が変化します（複雑化またはコスト）。
- **1が出た → 失敗 + 複雑化。** 複雑化は確実に発生します。
- **サイコロの最大結果 → 特別成功。**
  - 成功に加えて、**追加の利点**を得ます（より早く、静かに、強く、安全に、追加の効果）。

> コストを伴う成功の例: 「ドアを突破することができましたが、音を立ててしまい、誰かが確認しに来ます。」

### 2.5 簡易化と困難 (計算なし)

代わりに、ロールに +1/−1 を加えるのではなく、**サイコロのサイズ**を変更します。

- **良い状況** → **サイコロを1段階上げる**  
  <span class="rpg-token token-d6">k6</span> → <span class="rpg-token token-d8">k8</span> → <span class="rpg-token token-d12">k12</span> → <span class="rpg-token token-d20">k20</span>
- **悪い状況** → **サイコロを1段階下げる**  
  <span class="rpg-token token-d20">k20</span> → <span class="rpg-token token-d12">k12</span> → <span class="rpg-token token-d8">k8</span> → <span class="rpg-token token-d6">k6</span> → <span class="rpg-token token-d4">k4</span>

**簡易化の例:** 準備、良い道具、位置の優位性、奇襲、支援。  
**困難の例:** 暗闇、滑りやすい、時間のプレッシャー、騒音、気を散らすもの、防御。

**秩序の原則:** 迅速さのために、通常は1つのテストに対して**最大1つの簡易化と1つの困難**を適用することを受け入れてください（相殺される可能性があります）。

### 2.6 味方の助け

味方は自分のアクション（または戦闘以外のシーンでの時間）を捧げて助けることができます。

**効果:** この1回のテストに対して**サイコロを1段階上げる**。

助けは意味のある方法で説明されなければなりません（防御、道具の提供、注意をそらす、安定化、ヒント）。

### 2.7 テストの繰り返し

テストが失敗した場合、状況を変えずに「繰り返す」ことはしないでください。
- 何かを異なる方法で行う（異なる特性 / 異なる道具 / 異なる方法）、
- あるいはコストを受け入れる（時間、警報、資源）、
- あるいは撤退する。

### 2.8 テストの例（戦闘以外）

**例 A — 静かな通過**
- プレイヤー: 「照明が戻る前に中庭を通り抜けます。」
- GM: 敏捷性（A）。時間に追われている → 難易度 **T 5**。
- キャラクターは「影」の才能を持っている → 有利、サイコロが1段階上昇。
- ロール: <span class="rpg-token token-d12">d12</span>で4 → 失敗。GM: 「すぐには気づかれませんが、誰かが音を聞いて周囲を調べ始めます（複雑さ: プレッシャーが高まります）。」

**例 B — 力ずくでの強行**
- プレイヤー: 「警備員が角に来る前に金属のドアをこじ開けます。」
- GM: 力（<span class="rpg-token token-stat">S</span>）、難易度 **T 6**（道具なしでは非常に困難）。
- 誰かが鍵を押さえてドアを固定するのを手伝う → サイコロが1段階上昇。
- ロール: <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d12">d12</span>で12 → 特殊成功: ドアはすぐに開き、予想よりも静かに行えます。



---

### 3. 移動と距離（グリッドはオプション）

デフォルトではNDEはマップなしで動作します：シーンとキャラクターの位置を説明します。

### 3.1 デフォルト: 描写距離


使用する距離帯は4つ:
- **近い** — 手の届く範囲、近接戦闘。
- **少し遠い** — 数歩、簡単に近づける。
- **遠い** — シーンの反対側、明確な移動が必要。
- **非常に遠い** — スナイパー/車両/「シーンの境界で」。

ターン中、通常は距離を**1つの帯域**変更できます（例: 遠い → 少し遠い）。

### 3.2 オプション: グリッドでのプレイ (戦術用)

具体的な内容を好む場合:
- 1マス = 1–2メートル。
- ターン中の移動: **最大5マス**。
- 斜め移動は許可されています（通常のマスとしてカウントされます）。

### 3.3 シールドと行動ライン

- **完全シールド:** 「ラインを越えて」影響を与えることはできません（射撃、観察、多くの能力）。
- **部分シールド:** 難易度を上げます — 通常、**攻撃者/観察者のサイコロを1段階下げます**。

---



---

### 4. 戦闘

戦闘は通常のテストシーンであり、ターン制に整理されています。

### 4.1 戦闘が始まるとき

戦闘は以下の条件で始まります:
- 少なくとも一方が他方を傷つけたいと望んでいること、かつ
- 誰がいつ行動するかが重要です。

状況が短く明白な場合、GMは1回のテストでそれを決定することができます。

### 4.2 ターンの順序 (簡易版)

最も簡単に言えば:
- まずすべてのプレイヤーが行動します（任意の順序で）、
- 次に敵が行動します、
- そしてこのループを繰り返します。

### 4.3 あなたのターンで何をしますか

あなたのターンでは、以下のことができます:
- **移動**（ゾーンの変更 / グリッドバリアントで最大5マス）、
- **1アクション**（攻撃、テスト、援助、能力の使用、装備、シーンとのインタラクション）。

### 4.4 攻撃: それはどう機能するか

1) 目標を選び、攻撃を説明する。
2) 特徴を選択する:
   - **近接** → **力（<span class="rpg-token token-stat">S</span>）**のロール,
   - **遠距離** → **敏捷性（<span class="rpg-token token-stat">Z</span>）**のロール,
   - **魔法** → 通常は**魔力（<span class="rpg-token token-stat">M</span>）**のロール（第5章を参照）。
3) 目標の**防御**を設定する。
4) サイコロを振り、防御と比較する。

### 4.6 ダメージと「耐久力」

- ヒットは**1 ハート**を与えます。
- **特別成功**は**2 ハート**を与えるか、強力な効果（武器の解除、転倒、遮蔽からの押し出し）をもたらします — 一つを選んでください。

最も基本的な敵のアーキタイプ:
- **下っ端:** 1回のヒットで倒れます。
- **エリート:** **2 ハート**を持っています。
- **ボス:** **3 ハート**を持っています（または最終シーンでは5ハート）。

> 注意: 「倒れる」とは必ずしも死を意味するわけではありません。意識を失っている、逃げた、降伏した、行動から除外された可能性があります。

### 4.5 敵の防御（目安）

- **弱い:** 防御 **4**
- **標準的:** 防御 **5**
- **エリート:** 防御 **6**
- **ボス:** 防御 **8**（伝説のボス: **12**）

シールドと状況は通常、攻撃者のダイスのサイズを変更します（簡易化/困難化）、防御には影響しません。

### 5.7 攻撃の範囲（デフォルト）
数を増やさないために、簡単なルールを使いましょう：
- 直接：隣接するマスの目標。
- 距離：「視界内」のボード上の目標。
  - GMが制限を望む場合：**10マスまで**はペナルティなしで受け入れ、それ以上は<span class="rpg-token token-<span class="rpg-token token-math">tn</span>"><span class="rpg-token token-math">TN</span></span> +1段階。

### 5.8 複数の敵との接触
もし複数の敵が1人のキャラクターと「接触」している場合、GMは以下のことができます：
- 難易度を1段階上げる（プレッシャー）、または
- 失敗が追加の複雑さを意味することを認める（例：ポジションを失う）。

ルールは迅速であるべきです：**1つの判定 → 1つの効果**。

### 4.7 戦闘の例

**例 A — 兵士との近接戦闘**
- 突撃（<span class="rpg-token token-stat">S</span> <span class="rpg-token token-d12">k12</span>）が兵士を攻撃（防御 5）。
- 状況は良好（不意打ち）→ サイコロが1段階上昇するが、すでに<span class="rpg-token token-d12">k12</span>なので、上昇は<span class="rpg-token token-d20">k20</span>になる。
- <span class="rpg-token token-d20">k20</span>の振り = 7 → 命中、兵士は倒れる。

**例 B — 隠れ蓑からエリートを狙う**
- 専門家（<span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">k12</span>）がエリート（防御 6）を狙って射撃する。
- 標的は部分的に隠れている → 難易度上昇、サイコロが<span class="rpg-token token-d8">k8</span>に下がる。
- <span class="rpg-token token-d8">k8</span>の振り = 6 → 命中、エリートは1つのハートを失う（残りは1）。

**例 C — ボスと幸運の一撃**
- 見習い（<span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">k12</span>）がボス（防御 8）を力で無力化しようとする。
- <span class="rpg-token token-d12">k12</span>の振り = 4 → 失敗。プレイヤーは再振りのために1つのLSを使う。
- 再振り = 10 → 成功。ボスは1つのハートを失うが、GMはコストを追加する：「効果が大きく、アラームが鳴る。」



---

### 5. 力 (<span class="rpg-token token-stat">M</span>) と力ポイント (<span class="rpg-token token-power">PM</span>)

NDEにおいて「力」とは特殊効果のカテゴリーです。世界によって次のような意味を持つことがあります：
- 魔法、超能力、儀式、
- 高度な技術、ドローン、リアルタイムハッキング、
- 映画のヒーローの演技（例：「マスタリー集中」）、
- 会話が「力」となるゲームにおける社会的影響。

### 5.1 <span class="rpg-token token-power">PM</span>を使う時

<span class="rpg-token token-power">PM</span>を使うのは、**標準以上**の効果を得ようとする時です。

---

### 5.2 力を使う方法（ステップバイステップ）

1) 得たい効果を説明してください。
2) GMが難易度と<span class="rpg-token token-power">PM</span>のコストを決定します。
3) <span class="rpg-token token-power">PM</span>を使います。
4) **<span class="rpg-token token-stat">M</span>**を振り、難易度と比較します。

**失敗:** 効果は発揮されず; <span class="rpg-token token-power">PM</span>は失われ; 複雑さが発生します（オーバーロード、痕跡、暴露、副作用）。

### 5.3 効果のレベル (難易度 / コスト)

- **トリック** (短いトリック): **T 4 / 0–1 <span class="rpg-token token-power">PM</span>**  
  光、音、小さなカーテン、一時的な混乱。
- **スタンダード**: **T 5 / 1 <span class="rpg-token token-power">PM</span>**  
  弾丸、シールド、インパルス、ジャンプ、強化。
- **強力**: **T 6 / 2 <span class="rpg-token token-power">PM</span>**  
  エリア、コントロール、治療、麻痺、「戦闘中のハック」。
- **偉大な**: **T 8–12 / 3 <span class="rpg-token token-power">PM</span>**  
  シーンを変える効果またはキャンペーンに影響を与える結果。

### 5.4 特殊な成功の力

サイコロ<span class="rpg-token token-stat">M</span>で最大値を出した場合:
- スケールを増加させる（より広い範囲 / より長く / より強く）、または
- 追加の利点を加える（より静かに、より正確に、より安全に）、または
- GMは**1 <span class="rpg-token token-power">PM</span>**を返すことができる（フィクションに合う場合）。

### 5.5 <span class="rpg-token token-power">PM</span>の回復

- 戦闘のシーンの後、**1 <span class="rpg-token token-power">PM</span>**を回復します。
- 安全に休息を取ると、完全に回復します。

### 5.6 力の例

**例 A — 走り抜けるための盾**
- プレイヤー: 「より良い位置に走り抜けるために短い遮蔽を設置します。」
- GM: 標準 **T 5**、コスト 1 <span class="rpg-token token-power">PM</span>。
- ロール <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">k12</span> = 9 → 成功: 安全に走り抜けます。

**例 B — 失敗による結果**
- プレイヤー: 「エリートをその場に留めます。」
- GM: 強力な **T 6**、コスト 2 <span class="rpg-token token-power">PM</span>。
- ロール = 1 → 失敗 + 複雑化: 2 <span class="rpg-token token-power">PM</span>を失い、効果が反射してあなたの位置を暴露します。

---



---

### 6.1 0 ハート

もしあなたのハートが0になった場合:
- あなたは**行動不能**になります（負傷、気絶、ショック — コンベンションに応じて）、
- 同盟者は行動を犠牲にしてあなたを**1 ハート**で立たせることができます。

### 6.2 休息

- 戦闘のシーンの後、もし少しの余裕と基本的な条件があれば、あなたは完全なハートに戻ることができます。
- より厳しいキャンペーンでは、GMは完全に戻るために安全な休息を要求することがあります。

---

### 7.3 休息
戦闘/対立の後、安全に休息できる瞬間（および基本的な条件）があれば、あなたは完全に回復します：
- ヒットポイント、
- マナ。

これにより、システムは迅速に保たれ、長時間の治療を必要としません。



---

### 7. キャラクターの成長

**成長するタイミング:** 冒険、ミッション、または重要なストーリーの章の後（通常は1〜3セッションごと）。

**1つ選んでください:**
- **1つの能力値を1段階上げる**（最大<span class="rpg-token token-d20">k20</span>まで）、または
- **+1 ハート**（最大7）、または
- **+1 マナ**（最大5）、または
- **新しい特技**（1文で、GMと合意した具体的な能力）。

> 例: スペシャリストは、キャンペーンが追跡と銃撃戦の段階に入ったため、<span class="rpg-token token-stat">Z</span>を<span class="rpg-token token-d12">k12</span>から<span class="rpg-token token-d20">k20</span>に上げます。

---



---

### 8. バリアントのみ<span class="rpg-token token-d6">k6</span>: 2k6

異なるサイコロを使用したくない場合は、**2k6**でプレイしてください。

### 8.1 特徴を修正値として

サイズの代わりに修正値を分けてください:
- 一つの特徴は **+2**
- 一つは **+1**
- 一つは **+0**

### 8.2 テスト

サイコロを振る **2d6 + 特徴修正**。

**結果:**
- **6以下** – 結果が悪い
- **7–9** – コストを伴う成功
- **10以上** – 完全な成功
- **12** – 特別な成功（追加の利益）

### 8.3 状況の難易度

代わりに閾値を変更するのではなく、次のようにします:
- **+1** 優位性、準備、良い計画のために、
- **−1** 障害、プレッシャー、カバー、混沌のために。

### 8.4 幸運のルール 2d6

1ポイントの幸運を消費して:
- 2d6を再ロールするか、
- テストの結果に**+1**を加えるか、
- 失敗をコストを伴う成功に変える。

### 8.5 クイックマッピング（オプション）

もしキャラクターをバリエーション間で「再計算」したい場合は：
- <span class="rpg-token token-d6">k6</span> ≈ +0
- <span class="rpg-token token-d8">k8</span> ≈ +1
- <span class="rpg-token token-d12">k12</span> ≈ +2
- <span class="rpg-token token-d20">k20</span> ≈ +3（非常に経験豊富な場合）

---



---

[JA] コンテンツ準備中...




---

### 1. はじめに

7.2 これらの追加機能は必須ではありませんが、時には運営を容易にします。

### 9.1 防御（アーマー）を単純なリソースとして


もし「防御」が明確な効果を持つことを望むなら:
- 防御を持つキャラクターは **シーンごとに1つのアーマーチップを持つ**、
- 1つのハートを失う代わりに、アーマーチップを消費することができる。

### 9.2 時間のプレッシャーとしてのストッパー

シーンに時間制限がある場合、GMは「カウントダウン」を設定します（例：3ステップ）。各失敗はカウントを1つ進めます。カウントが終了すると、結果が発生します（警報、ターゲットの逃走、通路の崩壊）。

---

### 9.3 復讐（リスクのある戦闘のバリエーション）

戦闘をより「鋭く」迅速にしたい場合：
- **近接攻撃**を行い、**外した**場合、相手が実際にあなたに届くことができたなら、**1ハート**を失います。
これはバリエーションです — NDEの核心では、戦闘の失敗の結果は主にフィクションとGMの決定に基づいています。

