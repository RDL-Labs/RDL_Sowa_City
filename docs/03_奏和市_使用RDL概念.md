# 奏和市 使用RDL概念

> 本文書は、奏和市で使用するRDL概念を現行体系へ対応づけるための索引である。
>
> 奏和市固有の応用語彙を、RDL Core primitiveと混同しない。

---

## 1. T0：基盤層

| 概念 | 奏和市での扱い |
|---|---|
| **SILN** | 人間、妖精族（仮）、地区、文化、制度、Praxis等を、必要な境界で有限な関係構造として扱うための基礎 |
| **B** | Praxisや各主体が扱える有限な観測・記述・判断境界。都市全体を無境界に観測することは前提としない |
| **M_B** | B内で安定している関係拘束構造。市民・地区・文化・Praxis等について有限に構成される |
| **RIB / RIB_B** | 対象が参加する相互作用と、そのうちPurpose / finite Bで選ばれた有限断面 |
| **ξ** | 現在の有限Bによる記述が、関係全体を終端的に回収したとは保証できないこと。秘密情報・ノイズ・ランダム性そのものではない |
| **[B-ξ]** | `∀ B_finite : ξ(B) != 0`。奏和市やPraxisも自己例外化しない |
| **Aporapeiron** | 有限閉包が終端化せず、再検査・再構成可能性を残すという基底的見方 |
| **ADDξ** | 現在の閉包を終端化せず、残余関係を保持したまま再検査可能にする操作。奏和市ではPraxis自己モデル等への適用候補 |

---

## 2. T0最低動作仕様との対応

奏和市での基本的な読み方：

```text
SILN
  ↕
{RIB_1, RIB_2, ..., RIB_n, ...}
  ↓ Purpose / finite B
RIB_B
  ↓
F = interp(M_B, RIB_B)
  ↓
F' → E → review
             ├─ resolved / local
             └─ reviewed unresolved remainder → H
                                      ↓
                                   θ / M_Δ
                                      ↓
                           展開・検査・再構成
```

重要：

> **Eが非ゼロだから自動的にHへ入るわけではない。**

奏和市で「葛藤がある」「予想外が起きた」ことと、
それが未解決負荷として蓄積することは分ける。

---

## 3. F / E / H

| 概念 | 奏和市での扱い |
|---|---|
| **F** | 現在のM_BとRIB_Bのもとでの局所的解釈・作用評価 |
| **F'** | 新しい観測・相互作用後の評価 |
| **E** | FとF'の差分。差分があるだけで危機とはしない |
| **H** | 有限な検査・レビューを経ても未解決として残った負荷の蓄積。恐怖・ストレス等と同一視しない |
| **θ** | 応用上の再検査・再構成開始条件の候補 |
| **M_Δ** | 現在の構造を固定せず、展開・検査・再構成へ移る相 |

---

## 4. T1：SILN操作層

奏和市では主に次を用いる。

### 展開

対象を単一説明へ固定せず、

- 個人
- 関係
- 地区
- 文化
- 制度
- 技術
- 歴史
- Praxis自身

へ複数断面を開く。

### 検査・選別

- どの不整合が局所で吸収可能か
- どの経路が自己強化するか
- どの技術・概念接続が破局へつながるか
- どの介入が依存や支配を増やすか

を検査する。

### 再構成

破局回避のために、

- 距離
- 役割
- 制度
- 動線
- 資源
- 文化的意味
- 接続関係

を組み替える。

### ΔB

同じ問題を、

- 個人
- 家族
- 地区
- 都市
- 世代
- 歴史

など別境界で再観測する。

---

## 5. T2：奏和市固有の応用語彙

以下はRDL Core primitiveではない。

| 奏和市語彙 | 役割 |
|---|---|
| **動的幸福** | 不幸ゼロではなく、失敗・葛藤・喪失から再び生きられる状態へ戻れる関係動態 |
| **破局的不整合** | 局所的不整合が固定化・自己強化・広域波及し、回復困難な破断へ接続する状態候補 |
| **三重の無知** | 人間、妖精族（仮）、生活世界から見たPraxisの認識遮蔽構造 |
| **概念工学的な実質的焚書** | 危険な完成知識の禁止より、そこへ到達しやすい概念地図・接続経路を社会的に細らせる設計 |
| **局所関係調整個体** | 妖精族（仮）を設計・運用側から記述する機能名 |
| **妖精族（仮）** | 住民が一つの社会的種族として認識する作中呼称 |
| **スロー表層** | 高度な裏側に対し、生活世界の変化頻度を意図的に下げる都市設計 |
| **季節変動窓** | 退屈・探索圧を周期的な文化変動へ流す応用設計 |
| **還界の理** | 死と喪失を共同体内で処理するための文化的再意味化 |

---

## 6. PraxisのRDL上の位置

Praxisは、

```text
observer outside Sowa City
```

ではない。

Praxis自身もSowa CityのSILNへ参加する内部要素であり、
複数のRIBへ参加し、有限BのもとでRIB_Bを選び、有限なM_Bを構成する。

したがって、

```text
Praxis model complete under current B
and
ξ(B) != 0
```

は両立する。

Praxisは高能力でも、終端的な全知主体にはしない。

---

## 7. 妖精族（仮）のRDL上の位置

妖精族（仮）を、

```text
Praxis → endpoint → human
```

という単純な一方向端末にしない。

実際には、

```text
Praxis
↕
妖精族（仮）
↕
human
↕
district / culture / environment
```

のように、複数関係へ参加する。

個体の関係履歴そのものが、現在の局所構造に影響する。

---

## 8. 概念工学の扱い

概念工学的な実質的焚書は、RDL Core primitiveではなく奏和市固有の運用仮説である。

RDLで分析する場合は、

- どの概念がどの概念へ接続しているか
- どの接続が高危険度技術へ到達しやすいか
- どの接続を弱めると別の創造性まで失われるか
- どこで破局回避と知的自由が衝突するか

を有限Bごとに展開・検査する。

ここでも完全封鎖は前提としない。

---

## 9. Layeringとの接続

Praxis規模では、一つの階層だけで都市を整理しない。

候補軸：

- temporal scale
- spatial scale
- social scope
- culture / institution
- observability
- stability
- intervention cost
- reversibility
- dependency
- break / risk
- history depth

必要なときだけ、

```text
high-dimensional Layer Space
↓ Purpose / finite B
projection
↓
relevant axes
```

として扱う。

Layerは対象そのものではなく、用途に応じた整理道具である。

---

## 10. 現在使わない旧語彙

現行奏和市文書では、以下を現在概念として使用しない。

- SSD
- 限界空間
- 形而上空間
- EFP / 素流圧
- ξ = 揺らぎ
- M_B = 整合慣性という固定定義
- 旧T0〜T5体系
- 汎用階層構造4層
- RDL-GR
- 網絡化演算子N

歴史比較が必要な場合のみ旧資料として参照する。

---

## 11. 最短圧縮

```text
奏和市
= finite relational city under B

Praxis
= high-capability internal adjustment node

妖精族（仮）
= social species in lived world
= local relational adjustment individuals in design view

幸福
= static absence of unhappiness ではない

ξ
= hidden secret ではない
= terminal closure is not guaranteed

local mismatch
= allowed

catastrophic break
= intervention target
```
