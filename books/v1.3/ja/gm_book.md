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
generated_at: "2026-01-13T12:23:01.419Z"
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
# ゲームマスターの書



---



---

### 7.2 明確に料金を伝える。

- **明確にステークを伝える。** ロールが行われる前に、特徴、<span class="rpg-token token-tn">TN</span>、失敗の結果、助けの可能性を伝えます。
- **説明 → メカニクス → 結果。** 常にフィクションから始め、その後にロールを行います。
- **迅速なシーン。** ペースを維持します：1つのテスト = 1つの意味のある効果。
- **失敗はアクションを推進する。** 複雑さは状況を変え、「リセット」するのではなくシーンを進めます。
- **一貫性。** 同じ状況 → 同じ<span class="rpg-token token-tn">TN</span>と結果。



---

### 1. はじめに

1) プレイヤーは、自分が何をしているのか、何を達成したいのかを話します。
2) 特徴を選択します: **S** (力技)、**Z** (精密/迅速)、**M** (特殊効果)。
3) **<span class="rpg-token token-tn">TN</span>**を設定します: 4 簡単、6 普通、8 難しい、12 英雄的。
4) 失敗した場合のリスクを伝え、誰かが**助ける**ことができるかどうかを確認します（サイコロのサイズを1つ上げる）。
5) プレイヤーは特徴のサイコロを振り、<span class="rpg-token token-tn">TN</span>と比較します。
6) 結果を判断し、状況を更新します。

テーブル用の略語: 「特徴/<span class="rpg-token token-tn">TN</span>/ロール/結果」。



---

### 4 (簡単):

- **4 (簡単):** 条件が有利で、目標が抵抗しない。
- **6 (普通):** アドベンチャーの標準で、優位性なし。
- **8 (難しい):** 時間のプレッシャー、悪い位置、カバー、複雑な道具。
- **12 (英雄的):** 平均を超える挑戦; 通常、準備または高いサイコロが必要。

状況の修正: <span class="rpg-token token-tn">TN</span>を**1段階**移動（極端な場合は最大2）。
- 悪化: 暗い、滑りやすい、カバー、アラーム → <span class="rpg-token token-tn">TN</span> +1。
- 改善: 時間、道具、位置の優位性、驚き → <span class="rpg-token token-tn">TN</span> −1。

効果の迅速な直感（近似値）:
- <span class="rpg-token token-d6">d6</span> vs TN6 ≈ 17%; <span class="rpg-token token-d8">d8</span> vs 6 ≈ 38%; <span class="rpg-token token-d10">d10</span> vs 6 ≈ 50%; <span class="rpg-token token-d12">d12</span> vs 6 ≈ 58%。
- <span class="rpg-token token-d10">d10</span> vs TN8 ≈ 30%; <span class="rpg-token token-d12">d12</span> vs 8 ≈ 42%; <span class="rpg-token token-d20">d20</span> vs 12 ≈ 45%。
これらの数字は参考として使用し、リアルタイムで計算しないでください。

振らないべき時:
- 結果が明らかで、賭けがない場合。
- ロールが何も変えない場合（次の挑戦に進む方が良い）。



---

### 1 骨の中で

- **1のサイコロ**: 失敗 + 合併症。例：騒音、時間の浪費、誤った手がかり、小さな傷（−1ハート）、失われた資源、悪化したポジション。
- **失敗（結果 < <span class="rpg-token token-tn">TN</span>）**: 効果なしおよび場合によっては「報復」（戦闘中）または脅威の進行（戦闘外）。
- **特別成功（サイコロの最大値）**: 成功 + 追加の利益：より早く/静かに/コストなし/より大きな効果。

合併症を作成するためのチェックリスト：
1) 資源を攻撃する（時間、ポジション、ハート、マナ、装備）。
2) ボード上の配置を変更する（新しい障害物、遮断された道、強化されたシールド）。
3) プレッシャーを高める（カウント、アラーム、敵の強化）。



---

### ルーチュ

- **移動:** 1ターンで5マスまで; 斜め移動は可能。
- **遮蔽:** 部分的 → 遠距離攻撃の<span class="rpg-token token-tn">TN</span> +1; 完全 → 攻撃ラインなし。
- **困難な地形（オプション）:** マスに入るのに5ポイントのうち2ポイントを消費。
- **押し出し/移動:** S対<span class="rpg-token token-tn">TN</span> 6のテスト（状況に応じて修正）。成功: 対象を1〜2マス移動; 特殊成功: +1マス。
- **射程:** 10マスまでを「ペナルティなし」とし、それ以上は<span class="rpg-token token-tn">TN</span> +1。
スピードは細かい計算よりも重要です — ルールは軽く保ちましょう。



---

### 順序:

- **順序:** プレイヤー → 敵 → 繰り返し。
- **攻撃:** 近接 = S、遠距離 = Z; 敵の難易度: 兵士 6、エリート 8、ボス 12。
- **ヒット:** 兵士は倒れる; エリート/ボスは1つの傷を受ける（ボスは3つ持っている）。特別成功 = 通常は2つの傷。
- **外れ:** 敵が届くことができた場合 → ヒーローは1つのハートを失う（反撃）。遮蔽/遠距離の場合 — 通常は反撃なし。

プレッシャーのスケーリング:
- 多くの兵士が「近接」にいる場合 → 難易度 +1 または外れた場合の追加の複雑さ。
- 毎ターン地形を変更: 障害物、狭い通路、優位性を得る機会が出現する。



---

### 1. はじめに

シーンを5つのステップで構築する：
1) **目的**：シーンの目的（例：移動、アイテムの獲得、脅威の排除）。
2) **障害**：2～3種類の異なる障害（警備、城、アラーム、危険な地形）。
3) **脅威**：雑兵/エリート/ボス、危険要素、罠。
4) **カウンター（オプション）**：3～5ステップ；失敗するとカウンターが進む；最後に悪い結果。
5) **報酬/結果**：成功によって得られるもの、失敗によって変わるもの。

戦闘の規模の閾値（3～5人のヒーロー用）：
- **簡単**：3～5の雑兵または支援なしのエリート。
- **標準**：6～8の雑兵またはエリート + 2～4の雑兵。
- **難しい**：ボス + 2～4の雑兵または2のエリート + 3～5の雑兵。
- **英雄的**：ボス + 4～6の雑兵および/またはエリート。
テーブルに合わせて調整：地形と遮蔽物は大きな影響を与える。



---

### 1. はじめに

フォーマット（例、雰囲気なし）:
> **名前 — <span class="rpg-token token-tn">TN</span>、傷、戦術、特技**
- **小兵:** <span class="rpg-token token-tn">TN</span> 6、傷なし; 簡単な戦術。
- **エリート:** <span class="rpg-token token-tn">TN</span> 8、2傷; 明確な優位性を持つ（例: 機動性、遮蔽、戦場の制御）。
- **ボス:** <span class="rpg-token token-tn">TN</span> 12、3傷; 1〜2のユニークな動き（例: 押し返し、支援の召喚）。

反応と士気（軽いシステム）:
- 最初の小兵が倒れるか、エリートが傷を受けた場合、**<span class="rpg-token token-d6">d6</span>**を振る:
  - 1–2: 後退/潜伏; 3–4: ポジションを保持; 5–6: 突撃。
- 優位性/恐怖/ボスの近くに応じて±1を修正。



---

### 1. はじめに

魔法は「特殊効果」です。<span class="rpg-token token-tn">TN</span>（ターン数）とマナコストを以下のスケールに従って割り当てます：
- **トリック:** <span class="rpg-token token-tn">TN</span> 4、コスト 0–1（短い、小さな効果）。
- **スタンダード:** <span class="rpg-token token-tn">TN</span> 6、コスト 1（単一の対象、短いジャンプ、バリア）。
- **強力:** <span class="rpg-token token-tn">TN</span> 8、コスト 2（エリア、コントロール、治療 +2 ハート）。
- **大いなる力:** <span class="rpg-token token-tn">TN</span> 12、コスト 3（ステージ効果）。

補助ルール：
- **複数の対象:** コスト +1 マナ、または <span class="rpg-token token-tn">TN</span> +1 ステップのいずれか。
- **効果の維持:** 毎ターン 1 マナを支払うか、アクションを消費します。
- **呪文の反撃/回避:** キャラクターに適切なテスト（ZまたはM）を行わせ、同じ <span class="rpg-token token-tn">TN</span> に対抗して効果を減少または回避させることができます（フィクションに応じて）。



---

### 7.2 スクリトボイスト/スルー: **「アラームレベル」を **カウンター3-5として設定**

- **隠密行動/潜入:** 「警戒レベル」を**カウンター3–5**として設定します。失敗するとレベルが上がります。最大に達するとパトロールが出現し、ロックがかかるなどの影響があります。
- **追跡:** 「追跡のステップ」で距離を設定します（例：3）。各ターン: 両者がテストを行います。追跡者の成功は距離を短縮し、逃げる者の成功は距離を延長します。距離が0になると追いつき、5になると逃げ切ります。
- **環境の障害:** リスクのコストを明確に伝えます（例：落下 = −1ハートと不利な位置）、<span class="rpg-token token-tn">TN</span>は説明に依存します。



---

### 発展:

- **成長:** 冒険の後、各自が選択します: 特徴のサイズを増やす、+1 ハート（最大7）、または +1 マナ（最大5）。
- **物質的報酬:** 「許可」を与えます（新しい行動）または一回限りの利点（「シーンごとに<span class="rpg-token token-tn">TN</span>を1下げる」）。恒常的な修正は避けてください。
- **経済（オプション）:** シンプルな閾値: 安価/標準/高価 — 通貨を数えるのではなく、資源のテストで判定します。



---

### 1. はじめに

- プレイヤーとコンテンツの範囲を設定する（何がOKで、何を避けるべきか）。
- 不快な状況のための簡単な「ストップ」/「巻き戻し」サインを決める。
- コンフリクトはフィクションの中で解決し、テーブルでは行わない。



---

### 1. はじめに

1) **ハック:** 一文の問題。
2) **3つの場所**：戦術的特徴（遮蔽、高さ、狭い通路）。
3) **3つの障害物:** 城、警備、環境の脅威。
4) **賭けのリソース:** 時間、騒音、敵の注意。
5) **複雑さのリスト**（5つ）と**シーン用のカウンター**。
6) **敵:** 1行のエントリー（コーン/エリート/ボス） + シンプルな戦術。



---

# 合併症 — <span class="rpg-token token-d6">d6</span>（ユニバーサル）:
1. 時間の損失 / 敵の優位。
2. 位置の露見 / 警戒の上昇。
3. 軽微な損害: −1 ハートまたは資源。
4. 悪い位置: 押し出し/立ち往生。
5. 装備の損失/挟まり。
6. 新たな脅威がシーンに現れる。

# 特殊成功時の利益 — <span class="rpg-token token-d6">d6</span>:
1. より早く。
2. より静かに。
3. コストなし（例: マナなし/報復なし）。
4. より大きな効果（範囲/射程）。
5. 同盟者のより良い位置。
6. 追加のヒント/情報。



---

### プレイヤーの目標

- プレイヤーの目標: 確保された通路を通過すること。
- GM: 錠前 (<span class="rpg-token token-tn">TN</span> 6)、パトロール (カウンター 3)、狭い通路 (遮蔽)。
1) プレイヤー A: 「錠前を開けます」 (Z, <span class="rpg-token token-tn">TN</span> 6)。失敗 = +1 カウンター。ロール 5 → 失敗、カウンター 1/3。
2) プレイヤー B が助ける (サイコロを上げる)。A: 再度 (新しい道具、より良い位置)、ロール <span class="rpg-token token-d12">d12</span>=9 → 成功。
3) パトロールが接近中 (カウンター 2/3)。プレイヤー C が出口を守る (S, <span class="rpg-token token-tn">TN</span> 6)。特別成功 → チームに対する位置の優位性。
シーンは迅速に解決され、明確な賭けが設定された。

---
これが進行に必要なすべてです。残り (世界、モンスター、宝物) はモジュール式で、選択したユニバースに合わせて調整する必要があります。

