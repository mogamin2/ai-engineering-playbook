# AI Engineering Playbook

AI時代のソフトウェア開発と意思決定を、単なる「速さ」ではなく、  
**何を保持し、何を失い、誰が責任を持つか**という観点から設計するための公開プレイブックです。

> Version: v0.1.0  
> Status: Early public release / Working hypothesis

 
## Purpose

このリポジトリでは、次の問いを実務で扱います。

- AI支援開発で、手戻り・品質低下・文脈喪失をどう検知するか
- AIへ委譲してよい範囲と、人間が保持すべき責任をどう決めるか
- 顧客や組織が、AI投資について責任ある判断を下せる状態をどう作るか
- 仮説をどのように測定・反証し、プレイブックを更新するか

完成された標準を提示するのではなく、実践と検証によって更新される運用モデルを目指します。

## Core Concepts

### Loss Scan

AIに仕事を任せる前に、次の3問で失われやすい価値を確認します。

1. AIはこの仕事の何を知らないか
2. 一番壊れやすい場所はどこか
3. 壊れたとき、どう気づくか

### Vibe Compression

AIによって短縮された時間の中で、何が保持され、何が失われたのかを検知・分類・制御・計測するための運用モデルです。

### Decision-Ready Slice

指定された意思決定者が、一つの投資・スコープ・AI委譲の判断を下せるだけの、最小のend-to-endな根拠一式です。

## Planned Contents

- Loss Scan Quick Start
- Vibe Compression Operating Model
- Risk Class
- Loss Budget
- PR Template
- CI/CD Gate Examples
- Decision-Ready Slice Canvas
- Completed Examples
- Experiment Logs
- Changelog

## Related Articles

### 全体像：AI時代のエンジニア像・育成・組織

[LLMという片道タイムマシンの先で](https://note.com/mogamin2/n/n26d3c0ad2334)

### 意思決定：AIプロジェクトで判断できる状態を作る

[AI時代の最初の成果物は、ソフトウェアではない](https://note.com/mogamin2/n/n1e452a37e4c0)

### 開発運用：AI開発の手戻りと品質を制御する

[AI開発は「爆速」ではなく「圧縮」せよ](https://note.com/mogamin2/n/nbc1648594f91)

## Principles

- 体感ではなく測る
- 成功事例だけでなく、失敗と反証を記録する
- AIに責任を移さない
- チェックリストを増やすこと自体を目的にしない
- 実践結果に基づいて継続的に更新する

## Disclaimer

本リポジトリは筆者個人による公開プロジェクトです。  
所属組織の公式見解・戦略・制度を示すものではありません。

掲載する事例は、機密情報や個人・顧客を特定できる情報を除外または匿名化します。  
各テンプレートや方法は、個別のシステム、法令、契約、セキュリティ要件に応じて調整してください。

## Feedback

提案、反論、適用事例、失敗事例はGitHub Issuesで受け付けます。

## License

This repository is licensed under the [Apache License 2.0](./LICENSE).

本リポジトリの文章、テンプレート、図表、コード例は、特記がない限りApache License 2.0の条件で利用できます。

