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
generated_at: "2026-01-13T12:22:52.342Z"
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
# 基本ルールブック



---



---

### ゲームに必要なもの

[JA] コンテンツ準備中...
- （オプション）グリッドボード（グリッド紙、マット、VTT）とキャラクターマーカー。
- 鉛筆とキャラクターシート。
- サイコロ：**<span class="rpg-token token-d6">d6</span>、<span class="rpg-token token-d8">d8</span>、<span class="rpg-token token-d10">d10</span>、<span class="rpg-token token-d12">d12</span>、<span class="rpg-token token-d20">d20</span>**。
  - 実際には**各サイコロを1つずつ**（テーブル/パーティー用）で十分です。なぜなら、一度に1つのサイコロを振るからです。
  - もし<span class="rpg-token token-d6">d6</span>しか持っていない場合は、「<span class="rpg-token token-d6">d6</span>のみ」バリアントを使用してください（最後に）。



---

[JA] コンテンツ準備中...




---

[JA] コンテンツ準備中...


### 3.1 いつロールするか
[JA] コンテンツ準備中...


### 3.2 ロールの方法
[JA] コンテンツ準備中...


### 3.3 難易度（<span class="rpg-token token-tn">TN</span>）
[JA] コンテンツ準備中...


### 3.4 結果
[JA] コンテンツ準備中...


### 3.5 難易度の調整
[JA] コンテンツ準備中...


### 3.6 援助
[JA] コンテンツ準備中...




---

[JA] コンテンツ準備中...


### 4.1 マス
[JA] コンテンツ準備中...


### 4.2 移動
[JA] コンテンツ準備中...


### 4.3 カバー
[JA] コンテンツ準備中...


### 3.4 テスト結果

**難易度 (<span class="rpg-token token-tn">TN</span>)**: 4 (簡単)、6 (普通)、8 (難しい)。

**ロール結果:**
- **1**: 失敗 + 複雑化。
- **< <span class="rpg-token token-tn">TN</span>**: 失敗。
- **≥ <span class="rpg-token token-tn">TN</span>**: 成功。
- **Max (10/20)**: 成功 + 利益。

### 3.4 テスト結果
- **結果 ≥ <span class="rpg-token token-tn">TN</span> → 成功。** キャラクターは意図した効果を達成します。
- **結果 < <span class="rpg-token token-tn">TN</span> → 失敗。** 効果が出ません。
- **1が出た → 失敗 + 複雑化。** （<span class="rpg-token token-tn">TN</span>が低くても。）
- **サイコロの最大値 → 特別な成功。**
  - 成功に加えて、**追加の利益**を得ます。
  - 追加の利益は状況に応じて得られるべきです（より多くの効果、リスクの低減、より早く、より静かに、など）。

### 3.5 難易度の「計算なし」調整
+1/-1を振りに追加する代わりに、難易度（<span class="rpg-token token-tn">TN</span>）を**1段階**変更します。

- **悪条件** → <span class="rpg-token token-tn">TN</span> +1段階（例：6→8）:
  - 対象の遮蔽、暗闇、滑りやすさ、時間のプレッシャー、騒音、気を散らす要素。
- **良条件** → <span class="rpg-token token-tn">TN</span> -1段階（例：8→6）:
  - 準備、良い道具、位置の優位性、驚き、完全な集中。

もし何かが「極端に」難しい/簡単であれば、GMは**2段階**変更することができます。

**限界:**
- <span class="rpg-token token-tn">TN</span>が下げられて4未満になる場合、それは「ほぼ確実」と見なします（通常は振らずに成功）。
- <span class="rpg-token token-tn">TN</span>が上げられて12を超える場合、それは「ほぼ不可能」と見なします（通常は計画や別のアプローチが必要）。

### 3.6 同盟者の助け
同盟者は自分のターン（または戦闘外のシーン）で、アクションを捧げて助けることができます。

**助けの効果（コア）：** この1回のテストに対してサイコロを1サイズ上げます：
- <span class="rpg-token token-d6">d6</span> → <span class="rpg-token token-d8">d8</span> → <span class="rpg-token token-d10">d10</span> → <span class="rpg-token token-d12">d12</span> → <span class="rpg-token token-d20">d20</span>

順序のルール：
- 通常、**1人**が1回のテストに対して助けを提供できます（「助けの塔」を作らないため）。
- 助けは意味のある方法で説明されなければなりません：防御、道具の提供、注意をそらす、安定化、ヒント。

### 3.7 テストの繰り返し
テストが失敗した場合、状況を変えずに「繰り返し」行わないでください。
- 何かを異なる方法で行う（異なる特徴 / 異なるツール / 異なるアプローチ）、
- それとも複雑さを受け入れる（例：時間の消費、アラーム）、
- それとも撤退する。

### 3.8 テストの例（戦闘以外）
**例 A — 静かな通過:**
- プレイヤー: 「目立たずに開けた場所を通り抜けたい」。
- GM: 敏捷性（AG）。薄暗く、障害物がある → 難易度6（通常）。
- <span class="rpg-token token-d10">d10</span>のロール=5 → 失敗。GM: 「すぐには気づかれませんが、誰かが音を聞いて周囲を調べ始めます（複雑さ: 時間のプレッシャー）」。

**例 B — 道具を使う:**
- プレイヤー: 「機械を素早く起動させたい」。
- GM: 物理的な場合は力（<span class="rpg-token token-tn">ST</span>）、特別な効果の場合は魔法（MA）；ここでは: 力（<span class="rpg-token token-tn">ST</span>）。難易度6。
- 同盟者が助ける（サイコロを上げる）。<span class="rpg-token token-d12">d12</span>のロール=12 → 特殊成功: すぐに動作し、さらに音を立てません。



---

[JA] コンテンツ準備中...


### 5.1 戦闘開始
[JA] コンテンツ準備中...


### 5.2 ターン順序
[JA] コンテンツ準備中...


### 5.3 アクション
[JA] コンテンツ準備中...




---

[JA] コンテンツ準備中...


### 6.1 マナ
[JA] コンテンツ準備中...


### 6.2 解決
[JA] コンテンツ準備中...


### 6.3 エフェクトレベル
[JA] コンテンツ準備中...


### 6.4 クリティカル魔法

1) 目標を選択します（視界内で、かつ距離内にあるもの）。
2) 武器または魔法を選択します。
3) 使用する特性を確認します（例：近接攻撃の力、遠距離攻撃の敏捷性、魔法の呪文）。
4) **振ります。** 相手の**難易度（<span class="rpg-token token-tn">TN</span>）**と比較します。

### 6.4 クリティカル魔法
[JA] コンテンツ準備中...


### 6.5 魔法の例

- **パチョレク**: 死亡（または戦闘から脱落）。
- **エリート/ボス**: **1 ハート**を失う。
- **プレイヤー**: **1 ハート**を失う（ただし、アーマーを持っている場合は、アーマーが攻撃を吸収するが、消耗する）。

### 6.5 魔法の例
[JA] コンテンツ準備中...


### 5.6 パドロと「復讐」

戦闘にはリスクがあります。もし**当たらなかった場合**（結果 < <span class="rpg-token token-tn">TN</span>）や**1**を出した場合：
- 敵が反撃します：**1ハート**を失います。
- または、他の論理的な複雑さが発生します（例：武器を失う、倒される）。

*これは敵のターンではありません — あなたの失敗した攻撃の結果です。*

### 5.6 Pudłoと「復讐」
戦いにはリスクがあります。攻撃して当たらないと、相手はしばしば「反撃」します。

**反撃の原則（コア）:** 攻撃の結果 < <span class="rpg-token token-tn">TN</span> で、相手が実際にあなたに届く可能性があった場合、**1ハート**を失います。

「届く可能性があった」とはどういうことか（複雑さなしで）：
- 近接攻撃をする場合（隣に立っている） — ほぼ常にそうです、
- 遠距離攻撃をする場合、開けた場所にいて相手が攻撃する可能性がある場合 — 通常そうです、
- 完全な遮蔽がある場合や、実際の脅威の範囲外にいる場合 — 通常そうではありません。

**戦闘で1を振った場合:** 失敗 + 複雑化。最も一般的には、1ハートを失い、さらに何かが悪化します（例：倒れる、武器を失う、遮蔽から押し出される）。

### 5.7 攻撃の範囲（デフォルト）
数を増やさないために、簡単なルールを使いましょう：
- 直接：隣接するマスの目標。
- 距離：「視界内」のボード上の目標。
  - GMが制限を望む場合：**10マスまで**はペナルティなしで受け入れ、それ以上は<span class="rpg-token token-tn">TN</span> +1段階。

### 5.8 複数の敵との接触
もし複数の敵が1人のキャラクターと「接触」している場合、GMは以下のことができます：
- 難易度を1段階上げる（プレッシャー）、または
- 失敗が追加の複雑さを意味することを認める（例：ポジションを失う）。

ルールは迅速であるべきです：**1つの判定 → 1つの効果**。

### 5.9 戦闘の例（ステップバイステップ）
**例 A — 接近戦での簡単な交換:**
- 戦士（S <span class="rpg-token token-d10">d10</span>）がコーンの隣に立っています（<span class="rpg-token token-tn">TN</span> 6）。
- サイコロ <span class="rpg-token token-d10">d10</span>=4 → 外れ。接近戦なので、反撃が発生 → 戦士は1つのハートを失います。

**例 B — ボスと特別な成功:**
- ローグ（Z <span class="rpg-token token-d10">d10</span>）がボス（<span class="rpg-token token-tn">TN</span> 12）に射撃します。GMは「準備なしでは難しい」と言います。
- 仲間が助けます（サイコロ <span class="rpg-token token-d12">d12</span>）し、ローグは良い位置にいます（<span class="rpg-token token-tn">TN</span> 12 → 8）。
- サイコロ <span class="rpg-token token-d12">d12</span>=12 → 特別な成功: ボスは2つのダメージを受けます。



---

[JA] コンテンツ準備中...


### 6.1 マナ
- スタート時に**3マナ**を持っています。
- マナは「通常の能力を超えた効果」を得ようとする際に消費されます。

### 6.2 マジックの使用方法
1) 得たい効果を説明します。
2) GMが<span class="rpg-token token-tn">TN</span>とマナのコストを設定します。
3) マナを消費します。
4) マジックのサイコロ（M）を振り、<span class="rpg-token token-tn">TN</span>と比較します。

**失敗:** 効果が発揮されない; マナが無駄になる; 軽微な結果が生じる。

### 6.3 効果のレベル (<span class="rpg-token token-tn">TN</span> とコスト)
- **トリック:** <span class="rpg-token token-tn">TN</span> 4, コスト 0–1
  - 小さな効果: 光、音、煙幕、一時的な気を散らすもの。
- **スタンダード:** <span class="rpg-token token-tn">TN</span> 6, コスト 1
  - 弾丸、バリア、5マスのジャンプ、短時間の強化。
- **強力:** <span class="rpg-token token-tn">TN</span> 8, コスト 2
  - エリア、コントロール、治療 +2 ハート、麻痺。
- **大きな力:** <span class="rpg-token token-tn">TN</span> 12, コスト 3
  - 大きく、状況を変えるステージ効果。

### 6.4 マジックにおける特別な成功
マジックのサイコロで最大値を出した場合：
- 効果のスケールを増加させる（例：より広い範囲 / より長く / より強力に）、または
- コストを下げる（GMは1マナを返還できる）、または
- 追加の利点を加える（例：効果が静かで、正確で、味方に安全である）。

### 6.5 魔法の例
**例 A — 防御:**
- プレイヤー: 「安全に5マス走るために短いバリアを張りたい。」
- GM: 標準<span class="rpg-token token-tn">TN</span> 6、コスト1。
- ロール M <span class="rpg-token token-d10">d10</span>=9 → 成功: 走り抜け、状況が安全になる。

**例 B — 失敗と結果:**
- プレイヤー: 「エリートを無力化したい」(<span class="rpg-token token-tn">TN</span> 8、コスト2)。
- ロール=3 → 失敗: 効果が発動せず、2マナを失い、複雑な状況が発生する（例: 自分がさらけ出される）。



---

### 7.1 セルフ (生活)
- 標準で **5つのセルフ**を持っています。
- セルフの喪失は、現実の損害または疲労を意味します — 世界によって異なります。

### 7.2 0 サーク

もし0ハートに落ちた場合：
- あなたは**倒れた**状態です。
- 行動を行うことができません（這うことと、残りの力で話すことだけが可能です）。
- 同盟者があなたを「起こす」ことができます（助けのアクション）、これにより1ハートが回復します。
- 倒れた状態でダメージを受けると、**消滅**します。

### 7.2 0 ハート
0 ハートに落ちた場合：
- あなたは **倒れて** いて、アクションを実行できません、
- 同盟者はアクションを捧げて、あなたを **1 ハート** で立ち上がらせることができます。

### 7.3 休息
戦闘/対立の後、安全に休息できる瞬間（および基本的な条件）があれば、あなたは完全に回復します：
- ヒットポイント、
- マナ。

これにより、システムは迅速に保たれ、長時間の治療を必要としません。



---

[JA] コンテンツ準備中...




---

[JA] コンテンツ準備中...


### 9.1 骨のサイズの代わりに — スレッショルド
各特徴には<span class="rpg-token token-d6">d6</span>での成功のスレッショルドがあります：
- **マスター:** 3以上で成功
- **訓練された:** 4以上で成功
- **初心者:** 5以上で成功
- **熟練なし:** 6のみで成功

### 9.2 難易度と状況
<span class="rpg-token token-tn">TN</span> 4/6/8/12の代わりに「難易度」を使用し、しきい値を変更します：
- 通常は自分のしきい値で振ります、
- 1段階難しく → しきい値 +1、
- 1段階簡単に → しきい値 -1、
- （最小2、最大6）。

### 9.3 助け舟

### 9.4 ただ‑<span class="rpg-token token-d6">d6</span>の戦い
同じ敵のカテゴリを残すことができますが、<span class="rpg-token token-tn">TN</span>の代わりに「段階」を使用します：
- 小兵: 「通常」（しきい値の変更なし）、
- エリート: 「難しい」（しきい値に+1）、
- ボス: 「英雄的」（しきい値に+2）および3つの傷。

### 9.5 発展
発展は単独の<span class="rpg-token token-d6">d6</span>で行います：
- 一つの特性のレベルを上げる（例：初心者→熟練者）、
- または+1 ハート/マナ。



---

[JA] コンテンツ準備中...




---

### 1. はじめに

7.2 これらの追加機能は必須ではありませんが、時には運営を容易にします。

### 11.1 防御（アーマー）を単純なリソースとして
「防御」が機械的な意味を持つようにしたい場合：
- 防御を持つキャラクターは、シーンごとに1つの**アーマーチケット**を持っています。
- 1つのハート（反撃/攻撃）を失うことになった場合、代わりにアーマーを消費することができます。

### 11.2 時間のプレッシャーとしてのストッパー
シーンに時間制限がある場合、GMは「カウントダウン」を設定します（例：3ステップ）。各失敗はカウントを1つ進めます。カウントが終了すると、結果が発生します（アラーム、ターゲットの逃走、通路の崩壊）。

---
基本ルールブックの終了。

