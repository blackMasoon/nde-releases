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
generated_at: "2026-01-12T20:14:22.064Z"
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
# モンスターの書



---



---

### 1. はじめに

- 基本原則とMGの書にある用語を同じように使用します。
- **サイコロを振るのはプレイヤーだけです。** 敵は<span class="rpg-token token-tn">TN</span>や動きによってプレッシャーをかけます; ダメージは通常「反撃」やプレイヤーに強制されたテストから生じます。



---

### 1. はじめに

> 名前 — クラス、<span class="rpg-token token-tn">TN</span>、傷、役割、移動、特別

- **クラス:** パチョレク | エリート | ボス
- **<span class="rpg-token token-tn">TN</span>:** 敵を攻撃/回避する難易度を示す4/6/8/12の数値。
- **傷:** エリートとボスのみ（エリート: 2、ボス: 3がデフォルト）。パチョレクには傷がありません（攻撃を受けると倒れます）。
- **役割:** ブルート（近接戦）、スカーミッシャー（機動型）、アーティラリー（遠距離）、コントローラー（場の制御）、サポート（支援）。
- **移動:** デフォルトで5マス。移動性がユニークな場合は変更（例: 6速い、飛行、ジャンプ3）。
- **特別:** 1〜2の短い能力の説明（「特徴」と「動き」のセクションを参照）。

記録の例: 「エリートガード — エリート、<span class="rpg-token token-tn">TN</span> 8、傷 2、ブルート、移動 5、特別: 重装甲; 突撃」。



---

### パチョレク（ミニオン）：

- **Pachołek (ミニオン):** <span class="rpg-token token-tn">TN</span> 6、1回のヒットで倒れる。数が多いとプレッシャーをかける。外れた場合の報復: −1 ハート。
- **エリート:** <span class="rpg-token token-tn">TN</span> 8、2ダメージ。通常は1つの防御特性または機動性を持つ。外れた場合の報復: −1 ハート; 時々追加の状況効果。
- **ボス:** <span class="rpg-token token-tn">TN</span> 12、3ダメージ。2〜3の特殊な動きを持ち、地形/テンポに影響を与える。プレイヤーにテストを引き起こすことができる（例: 回避、安定化）。



---

### ブリュート（徒手格闘）

- **ブルート（近接戦闘）:** 突進して接触し、シールドを押し出す。
- **スカーミッシャー（機動型）:** 接触に入り/出て、孤独を罰する。
- **アーティラリー（遠距離）:** シールドの後ろから撃ち、移動を強いる。
- **コントローラー（制御）:** 脅威のゾーン、煙、押し出すフィールドを作成する。
- **サポート（支援）:** 同盟者を強化し、同盟者の<span class="rpg-token token-tn">TN</span>を下げるか、状況に応じてヒーローの<span class="rpg-token token-tn">TN</span>を1段階上げる。



---

### 1. はじめに

1–2をステータスブロックに追加します。常に説明的に機能し、意味がある場合にのみ<span class="rpg-token token-tn">TN</span>を1段階変更します。
- **自然の盾:** 敵の射程内にいる場合、通常は部分的な遮蔽を持つ（その敵への攻撃 → <span class="rpg-token token-tn">TN</span> +1段階）。
- **軽装甲:** このユニットに対する最初の1ハートの損失は無視される（シーン内での報復）。
- **タフ:** このユニットに対する最初の成功は傷を与えない（ただし、押し戻し/位置を変える）— ボスに適している。
- **速い（移動6）:** ターンごとに1マスの困難な地形を無視する。
- **クライマー/ジャンパー:** 垂直に/障害物を平坦な地面のように移動し、3マスのジャンプが可能。
- **飛行:** 地形の障害物を無視する（GMが合理的な遮蔽を考慮する）。
- **スカウト:** 不意打ちを受けにくい; 彼に対する最初の隠密試行は<span class="rpg-token token-tn">TN</span> +1。
- **耐性 [タイプ]:** シーン内でのそのタイプの最初の効果は軽減される（GMが説明: 範囲が狭い、持続時間が短い）。
- **感受性 [タイプ]:** このタイプの攻撃に対して<span class="rpg-token token-tn">TN</span>が1段階低くなる。
- **群れ:** 目標の隣に立っているとき、外れた攻撃の報復が1の範囲内の2人のヒーローに当たる可能性がある。



---

### 1. はじめに

選択肢 1–2 の特徴的な動き。動きは効果を説明します。もしそれがキャラクターに脅威を与える場合、GMは彼らに対して相手の<span class="rpg-token token-tn">TN</span>に対する適切なテスト（ZまたはM）を行うよう指示することがあります。
- **圧力（Brute）：** キャラクターが攻撃を受けた後、さらに1–2マス移動させます。
- **防御の破壊：** このユニットが命中した場合、対象の防御は次のターンの終わりまで無効になります。
- **引き裂き（Skirmisher）：** 接触からの出入りは反撃を引き起こしません。
- **集中砲火（Artillery）：** 3×3のエリア；エリア内の全員は<span class="rpg-token token-tn">TN</span>に対してZのテストを行います；失敗：−1ハートと1マス押し出されます。
- **アンカー（Controller）：** 3×3のフィールドが「粘着地形」となり（入るのに全アクションが必要）、次のターンの終わりまで続きます。
- **強化（Support）：** 一人の味方はラウンドの終わりまで1段階有利になります（攻撃者は<span class="rpg-token token-tn">TN</span> +1）。
- **召喚（Boss）：** 戦闘開始時に2体の小兵を空いているマスに召喚します。
- **バリア（Boss）：** 神の側のターンの終わりまで、キャラクターは遠距離攻撃を<span class="rpg-token token-tn">TN</span> +1で行います。
- **衝撃（Boss）：** 2マス以内の全員がS対<span class="rpg-token token-tn">TN</span>のテストを行います；失敗：−1ハートまたはノックダウン（このターンの移動を失います）。



---

### 1. はじめに

1) **クラスを選択:** コーン / エリート (2ダメージ) / ボス (3ダメージ)。
2) **<span class="rpg-token token-tn">TN</span>を設定:** 6 / 8 / 12 (非常に弱い場合は例外的に4、タフなエリートの場合は10)。
3) **役割を設定:** ブルート、スカーミッシャー、アーティラリー、コントローラー、サポート。
4) **1～2の特徴**と**1つの特別な動き**を追加 (ボス: 2～3の動き)。
5) **移動:** 通常は5; 重要な場合のみ変更。

完了。 この骨組みはすべてのリアリティで機能します。



---

### 1. はじめに

以下のエントリーを世界の名前/色に置き換えてください。

### 7.1 パチョウキ
- **ガーディアン パチョウキ — パチョウキ, <span class="rpg-token token-tn">TN</span> 6, —, ブルート, 移動 5, 特殊: ナチュラルシールド.**
- **スカウト パチョウキ — パチョウキ, <span class="rpg-token token-tn">TN</span> 6, —, スカーミッシャー, 移動 6, 特殊: スカウト.**
- **シューティング パチョウキ — パチョウキ, <span class="rpg-token token-tn">TN</span> 6, —, アーティラリー, 移動 5, 特殊: サルヴォ (小範囲 2×2, 警告のみ: 失敗時 −1 ハート).**
- **コントローラー パチョウキ — パチョウキ, <span class="rpg-token token-tn">TN</span> 6, —, コントローラー, 移動 5, 特殊: アンカー (1ターン, 一度限り).**
- **サポート パチョウキ — パチョウキ, <span class="rpg-token token-tn">TN</span> 6, —, サポート, 移動 5, 特殊: バフ (シーンごとに1回).**

### 7.2 エリート
- **エリートガード — エリート、<span class="rpg-token token-tn">TN</span> 8、傷 2、ブルート、移動 5、特技: 軽装甲; 突進。**
- **エリートアサシン — エリート、<span class="rpg-token token-tn">TN</span> 8、傷 2、スカーミッシャー、移動 6、特技: 引き裂き; 脆弱性 [観察]（見つけやすい）。**
- **エリートシューター — エリート、<span class="rpg-token token-tn">TN</span> 8、傷 2、アーティラリー、移動 5、特技: 自然の防御; サルヴォ（準備後3×3）。**
- **エリートコントローラー — エリート、<span class="rpg-token token-tn">TN</span> 8、傷 2、コントローラー、移動 5、特技: アンカー; 特殊成功時に1マス押し出し。**
- **エリートメディック — エリート、<span class="rpg-token token-tn">TN</span> 8、傷 2、サポート、移動 5、特技: 強化; ヒット時に味方の1つのコンプリーケーションを解除（説明的に）。**

### 7.3 ボス
- **リーダー — ボス, <span class="rpg-token token-tn">TN</span> 12, 傷 3, サポート, 移動 5, 特殊: 呼び出し; 強化; バリア.**
- **コロッサス — ボス, <span class="rpg-token token-tn">TN</span> 12, 傷 3, ブルート, 移動 5, 特殊: 突進（最大2マスまで）; タフ; ショック.**
- **ハンター — ボス, <span class="rpg-token token-tn">TN</span> 12, 傷 3, スカーミッシャー, 移動 6, 特殊: 引き裂き; 偵察者; バースト（ジャンプ — 移動後）.**
- **タクティシャン — ボス, <span class="rpg-token token-tn">TN</span> 12, 傷 3, コントローラー, 移動 5, 特殊: アンカー（1マナ/ターンで維持）; バリア; 呼び出し（1つのミニオン/ターン、最大3まで）.**



---

### 1. はじめに

危険要素「無思考の敵」または環境効果。ターンまたはトリガーで機能します。  
フォーマット: **名前 — <span class="rpg-token token-tn">TN</span>, 効果, 無効化方法**  
- **タレット — <span class="rpg-token token-tn">TN</span> 8, 効果: 敵のターン中、射線上の各キャラクターは<span class="rpg-token token-tn">TN</span>に対するテストを行う; 失敗: −1 ハート; 無効化: パネルでのMまたはZ <span class="rpg-token token-tn">TN</span> 8のテスト。**  
- **トラップ — <span class="rpg-token token-tn">TN</span> 6, 効果: フィールドに入るとZのテストを強制; 失敗: 麻痺または−1 ハート; 無効化: ツールを使ったZ <span class="rpg-token token-tn">TN</span> 6。**  
- **反発フィールド — <span class="rpg-token token-tn">TN</span> 8, 効果: ターンの開始時に2マスエッジに向かって移動; 無効化: M <span class="rpg-token token-tn">TN</span> 8（拡散）または電源遮断（S <span class="rpg-token token-tn">TN</span> 6）。**  
- **ガス/煙 — <span class="rpg-token token-tn">TN</span> 6, 効果: 3×3のエリア内でMまたはZのテスト; 失敗: ブラインドスポット/−1 ハート; 無効化: 換気（S）またはシール（Z）。**



---

### 1. はじめに

1. シーンの目的: 通過 / 回収 / 無効化 / 護送 / 盗み / 防御
2. 地形: 開けた場所 / 狭い廊下 / 複数階層 / モジュール式の遮蔽 / 危険な縁 / 霧-煙
3. 敵: 6× 兵士 / 4× 兵士 + エリート / 2× エリート / ボス / ボス + 2× 兵士 / エリート + 危険
4. 敵の優位性: 遮蔽 / 高さ / 機動性 / タイムリミット / 狭い通路 / 遠距離支援
5. プレイヤーの優位性: 奇襲 / 高いレベル / ツール / 短いバリア / ショートカット / 中立の同盟者



---

### 1. はじめに

代わりに数値の<span class="rpg-token token-tn">TN</span>を使用するのではなく、段階を使用してください：
- **パコーレク:** 「ノーマル」（<span class="rpg-token token-tn">TN</span> 6の相当）
- **エリート:** 「ハード」（+1段階）
- **ボス:** 「ヒーロー」（+2段階）および3つのダメージ
特徴や動きは同じように機能します。「<span class="rpg-token token-tn">TN</span> +1」と説明にある場合は、段階を上げてください。



---

### 7.2 戦いが短すぎる場合

- 戦闘が短すぎる場合: コーンを波のように追加（ターンごとに2つ）するか、敵の有利な位置に対して<span class="rpg-token token-tn">TN</span>を1段階上げる。
- 戦闘が長引く場合: より良い位置を作ることで特別な成功を得る機会を増やすか、弱体化した敵の<span class="rpg-token token-tn">TN</span>を下げる。
- エリート2体 ≈ 小さなボス; ボス + 4体のコーン ≈ 2時間のセッションの最終戦。



---

### 防衛隊 — パホレク、<span class="rpg-token token-tn">TN</span> 6、—、砲兵、移動 5、特別：自然の盾。

- **防衛隊 — パチョレク, <span class="rpg-token token-tn">TN</span> 6, —, 大砲, 移動 5, 特殊: 自然の盾。**
- **移動パトロール — パチョレク, <span class="rpg-token token-tn">TN</span> 6, —, スカーミッシャー, 移動 6, 特殊: 偵察。**
- **重攻撃部隊 — エリート, <span class="rpg-token token-tn">TN</span> 8, 傷 2, ブルート, 移動 5, 特殊: 軽装甲; 突撃。**
- **戦術家 — エリート, <span class="rpg-token token-tn">TN</span> 8, 傷 2, コントローラー, 移動 5, 特殊: アンカー; 強化。**
- **現場指導者 — ボス, <span class="rpg-token token-tn">TN</span> 12, 傷 3, サポート, 移動 5, 特殊: 呼び出し; バリア; 強化。**
- **地上コロッサス — ボス, <span class="rpg-token token-tn">TN</span> 12, 傷 3, ブルート, 移動 5, 特殊: 硬い; 衝撃; 突撃。**

---
これは敵を迅速に作成するためのツールセットです。<span class="rpg-token token-tn">TN</span>を設定し、クラスと役割を選び、1〜2の特性と移動を追加すれば、プレイ可能な敵がボードに登場します。

