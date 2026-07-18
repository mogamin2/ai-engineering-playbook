# Decision-Ready Slice Canvas

AIプロジェクトの最初に、ソフトウェアを作ることではなく、  
**意思決定者が責任を持って判断できる状態を作る**ためのCanvasです。

> Version: v0.1.0  
> Default timebox: 1〜2週間  
> Primary output: Yes / No / Not Yetを判断できる根拠一式

## Decision-Ready Sliceとは

Decision-Ready Sliceは、指定された意思決定者が、一つの投資・スコープ・AI委譲の判断を下すために必要な、最小のend-to-endな根拠一式です。

これは小さな製品や、機能を限定したPoCではありません。

動くソフトウェアは、判断に必要な根拠の一部になる場合がありますが、最終目的ではありません。

重要なのは、次の2点を最初に明示することです。

1. **Named Decision**：何を決めるのか
2. **Named Decision Owner**：誰がその判断を下すのか


## Timeboxの扱い

1〜2週間は標準期間でも、すべての案件で守るべき期限でもありません。

最初の判断ループが、目的のない調査や実装によって際限なく広がることを防ぐための、デフォルトの上限です。

次のような条件では、延長が必要になる場合があります。

- 公共、金融、医療、安全性など、慎重な検証が必要な領域
- 利用可能なデータの確認や準備に時間がかかる
- 法務、セキュリティ、契約上の確認が必要
- 現場観察や複数部門での用語・業務定義の合意が必要
- 意思決定者が判断するための会議体や承認手続きが定められている

延長する場合は、単に作業を継続するのではなく、次を明示します。

- なぜ現在の根拠では判断できないのか
- 追加で必要な根拠は何か
- 誰が延長を判断するのか
- 次に判断する期限はいつか

つまり、延長自体も一つのNamed Decisionとして扱います。

---

## Canvas

以下をコピーして、プロジェクトごとに記入してください。

```markdown
# Decision-Ready Slice

## 1. Named Decision

今回、何を決めるのか。

例：
○○工程の一次判定をAIに委譲するための初期投資を行うか。

Decision:
<記入>

Decision deadline:
<記入>

---

## 2. Named Decision Owner

Yes / No / Not Yetを最終的に判断する人は誰か。

Owner:
<役職または責任者>

Decision participants:
<判断材料を提供する人・部門>

---

## 3. Options and Baseline

比較する選択肢を記載する。

必ず、AIを使わない選択肢または現状維持を含める。

Option A:
<記入>

Option B:
<記入>

Option C:
<記入>

Baseline / Do nothing:
<記入>

---

## 4. Workflow Lane

今回の判断に最も近い、一つの業務レーンを選ぶ。

Start:
<業務の開始地点>

End:
<業務の終了地点>

People / Roles:
<関係者>

Main decisions:
<業務上の判断>

Exceptions:
<例外・異常系>

---

## 5. Business and Data Meaning

業務とデータの意味を明示する。

Key business terms:
<重要用語と定義>

Identifiers:
<何を同一のものと判断するか>

States and transitions:
<状態と遷移>

Time:
<どの時点の事実か>

Data sources:
<データの出所>

Data destinations:
<データの利用先>

Known inconsistencies:
<部門・システム間で異なる定義>

---

## 6. AI Delegation Level

AIに何を任せるかを段階で指定する。

- [ ] Observe：情報を読む・整理する
- [ ] Propose：案を提案する
- [ ] Modify：承認された範囲を変更する
- [ ] Execute：処理を実行する
- [ ] Affect：顧客・資金・安全など外部へ影響を与える

Selected level:
<記入>

Human approval point:
<人間の承認が必要な地点>

Fallback:
<AIから人間へ戻す条件>

---

## 7. Assumptions and Falsifiers

現時点の仮説を記載する。

Assumption 1:
<記入>

Evidence supporting it:
<記入>

What would prove it wrong:
<反証条件>

Assumption 2:
<記入>

Evidence supporting it:
<記入>

What would prove it wrong:
<反証条件>

---

## 8. Evidence Required

判断に必要な根拠を記載する。

- [ ] 業務モデル
- [ ] データ定義
- [ ] 選択肢比較
- [ ] 技術的実現可能性
- [ ] 運用可能性
- [ ] セキュリティ・法務・契約条件
- [ ] 費用・期待効果
- [ ] AIを使わない場合との比較
- [ ] 失敗時の影響
- [ ] ロールバックまたは撤退条件

Additional evidence:
<記入>

---

## 9. Loss Scan

AIや実装へ進む前に確認する。

AIが知らない文脈:
<記入>

一番壊れやすい場所:
<記入>

壊れたときの検知方法:
<記入>

---

## 10. Compression-Prohibited Items

時間短縮のために、省略してはいけないものを記載する。

- <例：データ定義の合意>
- <例：認可境界>
- <例：現場責任者による業務モデル確認>

---

## 11. Result

Decision:
- [ ] Yes
- [ ] No
- [ ] Not Yet

Decision date:
<記入>

Reason:
<判断理由>

Conditions:
<条件付きの場合の条件>

Residual risks:
<残るリスク>

---

## 12. Next Action

Yesの場合:
<次に開始すること>

Noの場合:
<停止・破棄・記録すること>

Not Yetの場合:
<不足している根拠>

Next Decision-Ready Slice:
<次に検証する判断>
```

---

## 最初に記入する4項目

すべてを一度に埋める必要はありません。

最初は次の4項目だけを確定します。

1. Named Decision
2. Named Decision Owner
3. Options and Baseline
4. Decision deadline

この4つが決まっていない状態で、実装やデータ収集を始めないことが重要です。

---

## 良いNamed Decisionの条件

良いNamed Decisionは、Yes / No / Not Yetで回答できます。

### 不十分な例

```text
AI活用の可能性を検討する。
```

何を判断するのか、誰が判断するのか、判断後に何が変わるのかが不明です。

### 改善例

```text
顧客問い合わせの一次分類をAIに委譲するため、
3か月の限定導入投資を行うか。
```

判断対象、委譲範囲、投資の有無が明確です。

---

## 選択肢に必ず含めるもの

Decision-Ready Sliceは、AI導入を正当化するための資料ではありません。

比較には、原則として次を含めます。

- AIを利用する案
- AIを利用しない業務改善案
- 現状維持
- 対象範囲をさらに限定する案
- 判断を延期する案

ベースラインがなければ、比較ではなく追認になります。

---

## 成功の定義

Decision-Ready Sliceの成功は、必ずしもYesを得ることではありません。

次も成功です。

- 誤った対象への投資をNoと判断できた
- 不足する根拠を特定してNot Yetと判断できた
- AIを使わない方がよいと判断できた
- 業務モデルやデータ定義の誤りを、実装前に発見できた
- 次に検証すべき、より小さな判断を特定できた

---

## これは何ではないか

Decision-Ready Sliceは、次のものではありません。

- 小さなMVP
- デモを作るためのテンプレート
- AI導入を承認させるための営業資料
- すべての要件を確定する設計書
- 意思決定者に代わって結論を出す仕組み

判断を下すのは、人間のDecision Ownerです。

本Canvasは、責任ある判断に必要な根拠を揃えるための道具です。

---

## 利用後に記録すること

利用後は、次を記録してください。

- Named Decisionを決めるまでにかかった時間
- 判断までにかかった時間
- 判断前に発見できた前提の誤り
- 判断後に発覚した前提漏れ
- Yes / No / Not Yetの結果
- 後日、判断を開き直したか
- 判断の開き直しが必要になった理由
- Canvasで不要だった項目
- Canvasに不足していた項目

---

## Related Resources

- [Loss Scan Quick Start](../loss-scan/README.md)
- [AI時代の最初の成果物は、ソフトウェアではない](https://note.com/mogamin2/n/n1e452a37e4c0)
- [Project Roadmap](../../ROADMAP.md)
- [Repository README](../../README.md)

---

## Feedback

利用例、反論、改善案、失敗例はGitHub Issuesで受け付けます。

顧客名、案件名、個人情報、契約上の機密情報は投稿しないでください。

---

## Disclaimer

本Canvasは、意思決定の品質、投資効果、法令適合性、安全性を保証するものではありません。

対象案件の契約、法令、セキュリティ、組織の権限規程、専門家の判断を優先してください。
