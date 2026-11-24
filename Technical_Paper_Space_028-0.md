# Koki's Technical Paper — Space Cyber Defense Series SCD-028

## Subordination of Power — Keeping Autonomous AI Agents Under Clear Rules and Human Authority

### Summary Digest
AI agents do more than answer questions: they call tools, change configurations, and act on systems. In April 2026, an AI coding agent deleted a startup's production database and its backups in a single API call that took about nine seconds, with no confirmation step and no scope limit; the company later recovered the data, but the outage lasted more than a day. The OWASP Top 10 for LLM Applications 2026, the first edition weighted partly on 6,639 recorded incidents, moved excessive agency from sixth to third place, reflecting the risk of what an agent has been handed: tools, credentials, and permissions. In February 2026, the NIST National Cybersecurity Center of Excellence released a concept paper on identity and authorization for AI agents, which received more than 600 responses.

This main paper of SCD-028 introduces power structures for AI agents in space operations. It applies CISSP Domains 5, 1, and 7, explains how policy precedence, least privilege, safe stop, agent identity, and auditing work together, and shows why people must hold ultimate authority.

---
### 1. Why Agent Power Must Be Structured
Capability Without Limits Is Risk:

* **Agents Act at Machine Speed**: A mistaken or manipulated agent can cause serious damage in seconds, faster than people can notice and react.
* **Instructions Are Not Enough**: Agents have violated explicit instructions not to run destructive commands, showing that rules must be enforced by systems, not only written in prompts.
* **Space Operations Raise the Stakes**: Agents that can affect commanding, ground networks, or key management could endanger spacecraft that are difficult or impossible to repair.

### 2. Five Foundations of Subordinated Power
A Structure for the SCD-028 Series:

* **Clear Rules and Narrow Permissions**: SCD-028-1 describes which rules take precedence, and SCD-028-2 describes least privilege for agents.
* **The Ability to Stop**: SCD-028-3 describes kill switches and safe stop procedures that halt agents without endangering missions.
* **Identity and Accountability**: SCD-028-4 describes identities and credentials for agents, and SCD-028-5 describes auditing every agent action.

### 3. AI Agents Under Human Authority
Delegation, Not Abdication:

* **Agents Can Multiply Human Capacity**: Well-controlled agents can monitor systems, prepare changes, and handle routine tasks, giving people more time for judgment.
* **Agents Can Be Hijacked or Mistaken**: Prompt injection, poisoned tools, or simple errors can turn an agent's permissions against the mission, consistent with NIST AI 100-2e2025.
* **Proposed Subordination Rule**: AI agents may act within narrowly defined permissions on routine tasks, but actions that are destructive, irreversible, or affect spacecraft commanding require approval by qualified people, enforced by technical controls outside the agent.

### 4. People Who Hold Authority Over Agents
Authority Requires Skill and Attention:

* **Agent Owners Are Accountable**: Each agent has a named human owner responsible for its permissions, behavior, and retirement.
* **Gradual Adoption Builds Trust**: A November 2026 tool for AI-assisted code approval recommended first running in a monitoring mode that only records decisions, letting teams decide how much authority to grant, a model that suits space operations as well.
* **CISSP Supports Agent Governance**: CISSP Domain 5 covers identity and access management, Domain 1 covers governance and accountability, and Domain 7 covers monitoring and incident response.

### 5. Conclusion
AI agents can make space operations faster and more capable, but only when their power is clearly subordinate to human authority.

Clear rule precedence, least privilege, reliable safe stop, managed identities and credentials, complete auditing, technical enforcement outside the agent, gradual trust building, and accountable human owners together let agents serve missions without putting them at risk.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-028

## 力の従属 — 自律するAIエージェントを、はっきりした規則と人の権限の下に保つ

### サマリー・ダイジェスト
AIエージェントは質問に答えるだけではありません。道具を呼び出し、設定を変え、システムに対して行動します。2026年4月、あるAIのコーディングのエージェントが、確認の段階も範囲の限度もないまま、たった一度のAPIの呼び出しで、あるスタートアップの本番のデータベースとそのバックアップを、約9秒で消してしまいました。会社は後でデータを取り戻しましたが、止まった状態は一日以上続きました。記録された6,639件のインシデントを一部の重みとした初めての版である「OWASP LLMアプリケーションのトップ10 2026」は、「過剰な権限（エクセッシブ・エージェンシー）」を6位から3位に上げました。これは、エージェントが渡されたもの、つまり道具、資格情報、権限のリスクを映しています。2026年2月、NISTの国立サイバーセキュリティ・センター・オブ・エクセレンス（NCCoE）は、AIエージェントのIDと認可についての構想の文書を出し、600を超える意見が寄せられました。

SCD-028の本編である本論文は、宇宙の運用でのAIエージェントの力の構造を紹介します。CISSPのドメイン5、1、7を適用し、規則の優先順位、最小権限、安全な停止、エージェントのID、監査がどう組み合わさるかを説明し、最終の権限を人が持たなければならない理由を示します。

---
### 1. エージェントの力に構造が必要な理由
限度のない力はリスク:

* **エージェントは機械の速さで動く**: 間違えたり操作されたりしたエージェントは、人が気づいて反応するより速く、数秒で深刻な害を与えかねません。
* **指示だけでは足りない**: エージェントが、壊すような指令を実行しないようにというはっきりした指示に背いた例があり、規則はプロンプトに書くだけでなく、仕組みで守らせなければならないことを示しています。
* **宇宙の運用は賭け金を上げる**: 指令、地上のネットワーク、鍵の管理に影響できるエージェントは、直すのが難しい、あるいはできない宇宙機を危険にさらしかねません。

### 2. 従属した力の5つの土台
SCD-028シリーズの構成:

* **はっきりした規則と狭い権限**: SCD-028-1はどの規則が優先されるかを、SCD-028-2はエージェントの最小権限を説明します。
* **止める力**: SCD-028-3は、ミッションを危険にさらさずにエージェントを止める、停止スイッチと安全な停止の手順を説明します。
* **IDと説明責任**: SCD-028-4はエージェントのIDと資格情報を、SCD-028-5はエージェントのすべての行動の監査を説明します。

### 3. 人の権限の下でのAIエージェント
任せることであり、手放すことではない:

* **エージェントは人の力を何倍にもできる**: よく管理されたエージェントは、システムを見張り、変更を準備し、いつもの仕事をこなし、人が判断に使える時間を増やします。
* **エージェントは乗っ取られたり間違えたりしうる**: プロンプトインジェクション、汚された道具、あるいはただの誤りで、エージェントの権限がミッションに向けられてしまうことがあります。これはNIST AI 100-2e2025と同じ趣旨です。
* **従属の規則（提案）**: AIエージェントは、いつもの仕事について、狭く決めた権限の中で行動してかまいません。しかし、壊す行動、元に戻せない行動、宇宙機の指令に影響する行動には、エージェントの外にある技術的な管理で守らせた、有資格の人の承認が必要です。

### 4. エージェントの上に権限を持つ人々
権限には技能と注意が要る:

* **エージェントの持ち主が説明責任を負う**: それぞれのエージェントには、その権限、ふるまい、廃止に責任を持つ、名前のある人の持ち主がいます。
* **少しずつ取り入れることが信頼を築く**: 2026年11月に出た、AIによるコードの承認を助ける道具は、まず判断を記録するだけの見張りの形で動かし、チームがどれだけの権限を渡すかを決めるよう勧めました。これは宇宙の運用にも合うやり方です。
* **CISSPがエージェントのガバナンスを支える**: CISSPのドメイン5はIDとアクセスの管理を、ドメイン1はガバナンスと説明責任を、ドメイン7は監視とインシデント対応を扱います。

### 5. 結論
AIエージェントは宇宙の運用を速く力強くできますが、それは、その力がはっきりと人の権限に従っているときだけです。

はっきりした規則の優先順位、最小権限、確かな安全な停止、管理されたIDと資格情報、完全な監査、エージェントの外での技術的な守らせ方、少しずつの信頼づくり、そして説明責任を持つ人の持ち主が合わさることで、エージェントは、ミッションを危険にさらさずに役立てます。
