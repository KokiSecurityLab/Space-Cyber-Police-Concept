# Koki's Technical Paper — Space Cyber Defense Series SCD-012

## Logical Intent Filtering — Runtime Guardrails for AI Agents in Space Operations

### Summary Digest
AI agents no longer only answer questions; they read documents, call tools, and take actions. In April 2026, industry researchers reported that indirect prompt injection had moved from proof of concept to live exploitation, and on May 1, 2026, cybersecurity agencies of the United States, Australia, Canada, New Zealand, and the United Kingdom published their first joint guidance on the careful adoption of agentic AI services.

This main paper of SCD-012 introduces runtime guardrails for AI agents that support satellite and ground operations. It applies CISSP Domains 3, 5, and 8, explains how to inspect inputs, intended actions, and outputs, and shows why humans must hold final authority over any action that could affect a spacecraft or critical service.

---
### 1. Why AI Agents Need Runtime Guardrails
From Answering Questions to Taking Actions:

* **Agents Act on What They Read**: An AI agent that reads telemetry reports, tickets, emails, or web pages can be redirected by instructions hidden in that content, a risk ranked first in the OWASP Top 10 for LLM Applications as prompt injection.
* **Attacks Are Already Happening**: A Cloud Security Alliance study published in April 2026 found that 65% of organizations had experienced at least one AI agent-related security incident in the previous twelve months.
* **Space Operations Raise the Stakes**: When an agent can draft commands, change schedules, or adjust ground station settings, a manipulated decision can have physical consequences that cannot easily be reversed.

### 2. Five Layers of Logical Intent Filtering
A Structure for the SCD-012 Series:

* **Recognize Manipulation**: SCD-012-1 explains how agents are tricked into giving false information or taking harmful actions through prompt injection.
* **Check Intent and Test Safely**: SCD-012-2 describes filtering based on the intended effect of an action, and SCD-012-3 describes running unverified commands in isolated environments before they touch real systems.
* **Protect Policies and Clean Data Flows**: SCD-012-4 explains how to keep safety policies outside the agent's control, and SCD-012-5 explains how to sanitize inputs and outputs in real time.

### 3. AI Agents Under Human Authority
Guardrails That Do Not Depend on the Model Alone:

* **Enforce Outside the Model**: Security decisions such as access checks and command approval are made by separate systems, because instructions given to a model can be overridden by crafted inputs, consistent with NIST AI 100-2e2025.
* **Least Privilege for Agents**: The joint agentic AI guidance recommends folding agents into existing zero-trust, defense-in-depth, and least-privilege frameworks and never granting agents unrestricted access to critical systems.
* **Proposed Agent Action Rule**: An AI agent may analyze data, propose commands, and perform pre-approved low-risk tasks, but any command to a spacecraft, change to safety policies, or action outside its approved scope requires approval by a qualified operator.

### 4. People Who Govern the Agents
Human Oversight as a Permanent Role:

* **Agents Need Owners**: Every AI agent has a named team responsible for its permissions, testing, monitoring, and retirement, so no agent operates without accountability.
* **Automation Should Support, Not Replace**: Organizations that replace experienced operators with agents lose the judgment needed to notice when an agent has been misled, while teams that pair people with agents gain speed without losing safety.
* **CISSP Provides Structure**: CISSP Domain 3 covers secure design, Domain 5 covers identity and access management for agents and people, and Domain 8 covers secure development and testing of AI-enabled software.

### 5. Conclusion
AI agents can make space operations faster and more responsive, but they can also be manipulated through the very information they are designed to read.

By inspecting inputs, checking the intent of actions, testing commands safely, protecting policies outside the model, and keeping qualified people in charge of every consequential decision, the space community can welcome AI agents as trustworthy partners that help people do their work better.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-012

## 論理的な意図のフィルタリング — 宇宙の運用で働くAIエージェントのための、実行時の安全柵

### サマリー・ダイジェスト
AIエージェントは、もう質問に答えるだけではありません。文書を読み、ツールを呼び出し、行動します。2026年4月、業界の研究者は、間接プロンプトインジェクションが実験の段階から実際の悪用の段階に移ったと報告しました。そして2026年5月1日、米国、オーストラリア、カナダ、ニュージーランド、英国のサイバーセキュリティ機関は、エージェント型AIサービスの慎重な導入について、初めての共同の指針を公表しました。

SCD-012の本編である本論文は、衛星と地上の運用を支えるAIエージェントのための、実行時の安全柵を紹介します。CISSPのドメイン3、5、8を適用し、入力、意図された行動、出力をどう検査するかを説明し、宇宙機や重要なサービスに影響しうる行動については、人が最終的な権限を持たなければならない理由を示します。

---
### 1. AIエージェントに実行時の安全柵が必要な理由
質問に答えることから、行動することへ:

* **エージェントは読んだものにもとづいて動く**: テレメトリの報告、対応依頼、メール、ウェブページを読むAIエージェントは、その中に隠された指示によって行き先を変えられることがあります。このリスクは、OWASPのLLMアプリケーションのトップ10で、プロンプトインジェクションとして1位に挙げられています。
* **攻撃はすでに起きている**: 2026年4月に公表されたクラウド・セキュリティ・アライアンスの調査では、65%の組織が、過去12か月の間にAIエージェントに関係するセキュリティのインシデントを少なくとも1回経験していました。
* **宇宙の運用では危険が大きくなる**: エージェントが指令の下書きを作り、予定を変え、地上局の設定を調整できる場合、操作された判断は、簡単には元に戻せない物理的な結果を生むことがあります。

### 2. 論理的な意図のフィルタリングの5つの層
SCD-012シリーズの構成:

* **操作に気づく**: SCD-012-1は、エージェントがプロンプトインジェクションによって、偽の情報を伝えたり有害な行動をとったりするようだまされる仕組みを説明します。
* **意図を確かめ、安全に試す**: SCD-012-2は行動の意図された効果にもとづくフィルタリングを、SCD-012-3は確認されていない指令を、本物のシステムに触れる前に隔離した環境で動かすことを述べます。
* **方針を守り、データの流れをきれいにする**: SCD-012-4は安全の方針をエージェントの手の届かないところに置く方法を、SCD-012-5は入力と出力をリアルタイムで無害にする方法を説明します。

### 3. 人の権限の下でのAIエージェント
モデルだけに頼らない安全柵:

* **モデルの外で強制する**: アクセスの確認や指令の承認のようなセキュリティの判断は、別のシステムで行います。モデルに与えた指示は、作り込まれた入力で上書きされることがあるからです。これはNIST AI 100-2e2025と同じ趣旨です。
* **エージェントにも最小の権限を**: エージェント型AIについての共同の指針は、エージェントを、今あるゼロトラスト、多層防御、最小権限の枠組みに組み込み、重要なシステムへの制限のないアクセスを決してエージェントに与えないよう勧めています。
* **エージェントの行動の規則（提案）**: AIエージェントはデータを分析し、指令を提案し、前もって承認されたリスクの低い作業を行ってかまいません。しかし、宇宙機へのあらゆる指令、安全の方針の変更、承認された範囲の外での行動には、有資格の運用担当者の承認が必要です。

### 4. エージェントを治める人々
ずっと続く役割としての人の監督:

* **エージェントには持ち主が要る**: どのAIエージェントにも、その権限、試験、監視、引退に責任を持つ、名前のあるチームがいます。そうすれば、責任の所在がないまま動くエージェントはなくなります。
* **自動化は支えるもので、置き換えるものではない**: 経験のある運用担当者をエージェントに置き換える組織は、エージェントがだまされたときに気づくための判断力を失います。一方、人とエージェントを組ませるチームは、安全を失わずに速さを得られます。
* **CISSPが枠組みを与える**: CISSPのドメイン3は安全な設計を、ドメイン5はエージェントと人のためのIDとアクセスの管理を、ドメイン8はAIを使うソフトウェアの安全な開発と試験を扱います。

### 5. 結論
AIエージェントは、宇宙の運用をより速く、より素早く反応できるものにできます。しかし、まさに読むように作られた情報によって、操られることもあります。

入力を検査し、行動の意図を確かめ、指令を安全に試し、方針をモデルの外で守り、そして結果を伴うすべての判断を有資格の人が担うことで、宇宙の世界はAIエージェントを、人がよりよく働けるよう助ける、信頼できる仲間として迎えられます。
