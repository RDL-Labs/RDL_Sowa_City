# 奏和市：現行RDL概念マップ v0.2

## 0. 目的

この文書は、奏和市で使っている考え方を、**現在の `Aporapeiron/RDL_Core` の意味境界へ対応づけるための索引**である。

奏和市はRDLの応用事例であり、Core概念の定義元ではない。

```text
RDL_Core
= semantic authority

RDL_Sowa_City
= application / thought experiment
```

過去の奏和市文書には、旧 `限界空間 / 形而上空間 / EFP（素流圧） / M_B=整合慣性 / ξ=揺らぎ / 旧T0〜T5` 等が含まれていた。

これらを現行RDLのCore定義としては使用しない。

---

## 1. T0 基盤層との対応

### SILN

奏和市では、分析目的に応じて都市全体・地区・共同体・個人・金属族・プラクシス・制度などを、SILNとして対象化できる。

ただし、

```text
奏和市 = SILN
```

と常に固定するわけではない。

Purpose / B に応じて、どの構造を対象SILNとして扱うかを明示する。

例：

```text
Purpose: 地区間対立を検査する
Target SILN: District A / District B / inter-district relation structure

Purpose: 金属族との依存関係を検査する
Target SILN: Human-Metal relational structure
```

---

### RIB / RIB_B

奏和市で旧来「環境から与える圧」「素流圧」と呼んでいたものを、そのまま一つのCore変数へ置き換えない。

現在は、

```text
都市環境
人との遭遇
仕事負荷
祭礼
移動条件
金属族との接触
評判
自然条件
```

などを、対象との相互作用へ参加する複数の `RIB` として考え、有限Bで選ばれた作用断面を `RIB_B` として扱う。

```text
EFP / 素流圧
→ deprecated as Core term

interaction bundles
→ RIB

finite selected interaction section
→ RIB_B
```

---

### B

`B` は奏和市の設計上きわめて重要である。

プラクシスも市民も金属族も、都市全体のすべての関係を一度に取得しない。

例：

```text
B_person
B_household
B_district
B_event
B_city_operation
B_long_term_culture
```

これらは固定的な自然階層ではなく、用途・問いに応じた有限境界である。

---

### M_B

`M_B` は「整合慣性」という都市固有の曖昧な総量ではない。

現行Coreでは、有限Bのもとで解釈・予測・応答・更新を拘束する自己側有限関係拘束構造として扱う。

奏和市では例えば、

- 市民がある地区をどう理解しているか
- 金属族が特定の人との関係をどう保持しているか
- プラクシスが現在の有限運用境界でどの関係拘束を保持しているか

を分析する際に `M_B` が関係する。

```text
M_B
!= personality score
!= happiness score
!= inertia scalar
```

---

### F

`F` は `interp(M_B, RIB_B)` による有限な作用解釈・予測として扱う。

同じ都市イベントでも、異なる市民・金属族・地区が異なる `M_B` を持てば、異なる `F` を形成しうる。

例：

```text
同じ祭礼の混雑
→ ある市民には楽しい交流
→ 別の市民には負荷
→ 金属族には救助・誘導条件
```

これは `F` が一つの感情ラベルそのものという意味ではない。

---

### E / H / θ / M_Δ

奏和市旧文書では `E=誤差量`、`H=熱` として都市スケールの幸福管理に直接使っていたが、この読みは現行Coreへそのまま持ち込まない。

現行では概念的に、

```text
F / F'
↓
E = difference
↓ finite assessment
unresolved remainder
↓
H
↓ compare with θ
M_Δ when required
```

という意味境界を維持する。

したがって、

```text
市民が不機嫌
→ H += 1

地区対立が激しい
→ H = conflict score
```

のような直接対応はしない。

奏和市固有の幸福・緊張・対立・回復可能性などの評価指標が必要なら、GameAI-local / Sowa-local descriptorとして別に定義する。

---

### ξ / [B-ξ]

奏和市にとって最重要の注意条件の一つ。

```text
∀B_finite : ξ(B) != 0
```

ここで `ξ` は、

```text
randomness
uncertainty score
unknown count
failure count
fluctuation amount
```

ではない。

現在の有限Bでは回収されない関係が残ることを示す。

したがって、プラクシスが広域観測を行っても、

```text
Praxis observes more
!= Praxis reaches ξ = 0
```

である。

奏和市の安定も、都市全体の終端的閉包を意味しない。

---

### [SELF]

奏和市・プラクシス・幸福維持Purpose・本概念マップそのものも、例外化しない。

```text
RDL applies to Sowa City
and
Sowa City's RDL reading is itself revisable
```

特に、

> 「幸福維持のためだからこの介入は正しい」

を自己正当化の終端条件にしてはならない。

---

## 2. T1 SILN操作層との対応

### 展開 / Expansion

都市で問題が発生した際、最初から一つの原因へ閉じず、関係候補を展開する。

例：地区間対立なら、

```text
resource distribution
history
festival rivalry
transport
reputation
individual incidents
weather
Praxis intervention history
Metal Tribe behavior
```

などを候補として開く。

---

### Probe

介入は、都市全体を直接書き換える万能操作ではなく、有限な探りとして扱える。

例：

```text
meeting timing change
route change
small event placement
support introduction
temporary workload reduction
```

を入れ、後続 `RIB_B` と解釈差を観察する。

---

### Inspection & Selection

候補関係を、現在のPurpose / B / 許容損失 / provenanceのもとで検査する。

```text
retain
reject
defer
```

のように、採用・棄却・保留を区別する。

奏和市では特に、短期的な幸福改善だけで選別しない。

介入が、

- 依存
- 不可視支配
- 地区文化の均質化
- 自律性喪失
- 長期的な回復経路減少

を生んでいないかも検査対象とする。

---

### Reconstruction

選別後、必要なら `M_B'` を再構成する。

奏和市では、これは「都市を再プログラムする」ことと同一ではない。

対象が市民、金属族、プラクシス自身の運用モデルなど、どのSILN_SELFを扱っているかで再構成対象は異なる。

また、再構成後も有限であり `ξ` は残る。

---

## 3. RDL_General_Modulesとの接続

### RDL 横断レイヤリング_キット

奏和市では、社会・都市構造を整理する補助Viewとして使える。

例：

```text
Geography / Environment
        ↓
History / Culture
        ↓
Institution / City Rules
        ↓
District / Organization
        ↓
Individual
        ↓
Realtime Event
```

これは存在論的な固定階層ではない。

Purpose / B / Axisによって切り方は変わる。

奏和市は特に、

```text
Layering != Hierarchy
```

を維持する必要がある。

プラクシスが広域Layerを扱うからといって、存在論的に市民より上位であるとは限らない。

---

## 4. 奏和市固有の応用概念

以下はCore primitiveではなく、奏和市固有の設計概念である。

| 概念 | 奏和市での意味 |
|---|---|
| **幸福維持** | 静止した快楽最大化ではなく、回復・再接続可能性を長期的に維持する設計Purpose |
| **プラクシス** | 都市内部の広域観測・調整・保守機構 |
| **金属族** | 都市機能と個体的関係形成を同時に担う人工的隣人種族 |
| **非暴力制約** | プラクシス・金属族の通常解決経路から暴力的強制・誘導を外すSowa-local constraint |
| **還界の理** | 死後に残る関係を共同体で再配置する文化的枠組み |
| **地区共同体** | 都市内部の局所文化・技能・評判・関係形成単位 |
| **不可視支援** | 市民の日常主体性を残しつつ背景側で致命的破断を防ぐ支援構造 |

これらをRDL Coreへ自動昇格させない。

---

## 5. 旧語彙の移行表

| 旧文書の語 | 現在の扱い |
|---|---|
| 限界空間 | 使用しない。有限境界 `B` と `[B-ξ]` で扱う |
| 形而上空間 | 独立基底として使用しない |
| EFP / 素流圧 | Core語として廃止。相互作用は `RIB / RIB_B` へ分解して扱う |
| M_B = 整合慣性 | 使用しない。`M_B` は自己側有限関係拘束構造 |
| ξ = 揺らぎ | 使用しない。`ξ` は現在の有限Bで未回収の関係 |
| E = 都市誤差量 | 使用しない。`E` は比較された解釈差 |
| H = 熱 | 使用しない。`H` は有限assessment後の未解消残存不整合 |
| 汎用階層構造4層 | 固定一般則にしない。必要なら横断レイヤリング・キットのProfileとして使う |
| 旧T0〜T5 | 使用しない。CoreのT0 / T1 / TDと、外部応用・Moduleの責務へ再配置 |

---

## 6. 奏和市を読む最小フロー

```text
対象 / Purposeを決める
↓
有限Bを置く
↓
対象SILNと関係するRIBを整理
↓
RIB_Bを取得
↓
M_BのもとでFを形成
↓
後続条件との差をEとして観測
↓
有限assessment
↓
必要ならT1で展開・検査・選別・再構成
↓
再び有限Bへ戻る
↓
ξは残る
```

奏和市は、このサイクルを「都市全体を一度に完全管理する」ためではなく、**複数スケールの有限な調整を繰り返すための思考実験**として利用する。

---

## 7. 一文圧縮

> **奏和市は、RDL Coreの有限B・SILN・RIB/RIB_B・M_B・F/E/H・ξ・T1操作を意味上の基準としつつ、幸福維持・非暴力制約・プラクシス・金属族・地区文化などをSowa-localな応用概念として検査する最大射程の都市思考実験である。**
