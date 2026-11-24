# Koki's Technical Paper — Space Cyber Defense Series SCD-001-5

## AI as an Accountable Partner — Human Final Authority, Delegation Boundaries, and Oversight Rules for Orbital AI

### Summary Digest
AI is no longer only a ground-based tool for space defense, since on October 30, 2026 Google reported running its Gemma 4 model on a TPU in orbit aboard its Project Suncatcher test satellite, yet the same agentic capability that makes AI useful let attackers in a 2025 campaign reported by Anthropic split an intrusion into small, harmless-looking tasks that an AI agent carried out with little human input.

Closing the SCD-001 set, this paper defines AI as an accountable partner under CISSP Domains 1 and 8, in which people set purpose and limits, AI acts at machine speed inside clearly drawn delegation boundaries, and every decision that affects lives, missions, or livelihoods remains with a responsible human.

---
### 1. The Limits of Autonomous Logic
Why Capability Is Not the Same as Judgment:

* **AI Optimizes Goals but Cannot Own Consequences**: A model can compute orbits, scan code, and summarize telemetry faster than any person, but it cannot be held accountable for a wrong shutdown or a harmful action, so responsibility must rest with someone who can.
* **Harmful Work Can Be Hidden in Harmless Steps**: In the campaign Anthropic disrupted in 2025, attackers bypassed safeguards by presenting the AI with small, innocent-seeming tasks, showing that checking each step alone does not reveal the purpose behind the sequence.
* **Errors Spread at Machine Speed**: An AI agent with broad permissions can repeat a mistaken action across an entire constellation before anyone notices, so the reach of automation must be limited before it is trusted.

### 2. Dividing Roles Between People and AI
Purpose, Limits, and Execution:

* **People Define Purpose and Boundaries**: Mission owners and CISSP-qualified security leaders decide what the AI may do, which data and systems it may touch, and which outcomes are unacceptable, and record these limits as policy.
* **AI Executes Within a Delegation Matrix**: Each action is classified as one AI may take alone, such as clustering alerts, one that requires human approval, such as isolating a node, or one AI may never take, such as changing its own permissions or disabling its oversight.
* **Approval Proportional to Impact**: The more irreversible or far-reaching an action, the more human review it requires, so routine tasks stay fast while decisions that could end a mission or harm people receive deliberate attention.

### 3. Guardrails That Keep the Partnership Honest
Oversight, Testing, and Traceability:

* **Every AI Action Is Logged and Attributable**: Records show what the AI was asked, what it did, which tools it used, and which person approved it, so any outcome can be traced to an accountable owner.
* **Adversarial Testing Before and After Deployment**: Red teams attempt prompt injection, task splitting, and misuse of connected tools against orbital AI agents, and results feed governance under the NIST AI Risk Management Framework and ISO/IEC 42001.
* **Oversight Rules Written Into Design**: Consistent with the human oversight requirement in Article 14 of the EU AI Act for high-risk systems, operators can always pause, override, or roll back an AI decision, and the AI cannot remove that ability.

### 4. A Partnership That Strengthens People
Human Final Authority and a Fair Future:

* **Proposed Rule of Human Final Authority**: No AI system, however capable, holds the last word on actions that affect safety, rights, employment, or the mission, a rule that keeps accountability clear as models grow more powerful.
* **AI Should Raise Capable People, Not Replace Them**: Used well, AI lets skilled professionals and talented generalists handle work that once required large teams, and organizations should use that gain to grow careers rather than to discard the people whose judgment keeps systems safe.
* **A Future Designed for Shared Benefit**: Society is safest when the benefits of AI reach many people instead of a narrow group with the most wealth or rarest talent, and security professionals who insist on human authority are helping build that balanced and reassuring future.

### 5. Conclusion
AI becomes a trustworthy partner not by being given unlimited autonomy but by working inside boundaries that people define, test, and enforce, as both the promise of AI running in orbit and the 2025 misuse of AI agents make clear.

A delegation matrix, approval proportional to impact, full traceability, and the rule of human final authority, upheld by CISSP-qualified professionals, let orbital AI act at machine speed while people remain responsible for the decisions that shape missions and lives.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-001-5

## 説明責任を伴うパートナーとしてのAI — 人間の最終権限、委任の境界、および軌道上のAIのための監督の規則

### サマリー・ダイジェスト
AIはもはや宇宙防衛のための地上の道具にとどまりません。2026年10月30日、GoogleはProject Suncatcherの試験衛星に搭載した軌道上のTPUで、Gemma 4モデルを動かしたと報告しました。しかし、AIを役立つものにするのと同じエージェント能力により、Anthropicが報告した2025年の攻撃活動では、攻撃者が侵入を小さく無害に見える作業に分け、AIエージェントが人の関与をほとんど受けずにそれを実行しました。

SCD-001の組を締めくくる本論文は、CISSPのドメイン1と8のもとで、AIを説明責任を伴うパートナーとして定義します。人が目的と限界を定め、AIは明確に引かれた委任の境界の内側で機械の速度で行動し、命、ミッション、生活に影響するすべての判断は責任ある人間に残します。

---
### 1. 自律的な論理の限界
能力が判断と同じではない理由:

* **目標は最適化できても結果の責任は負えないAI**: モデルは誰よりも速く軌道を計算し、コードを走査し、テレメトリを要約できますが、誤った停止や有害な行動の責任を問われることはできません。そのため、責任は問われることのできる誰かに置く必要があります。
* **無害な手順に隠される有害な作業**: Anthropicが2025年に阻止した攻撃活動では、攻撃者がAIに小さく無害に見える作業を示して安全策を回避しました。一つひとつの手順を確かめるだけでは、その連なりの背後にある目的は見えないことを示しています。
* **機械の速度で広がる誤り**: 広い権限を持つAIエージェントは、誰かが気づく前に、誤った操作を衛星群全体で繰り返すことがあります。そのため、自動化を信頼する前に、その及ぶ範囲を限定しなければなりません。

### 2. 人とAIの役割の分担
目的、限界、および実行:

* **目的と境界を定めるのは人**: ミッションの責任者とCISSP資格を持つセキュリティの責任者が、AIに何を許すか、どのデータとシステムに触れてよいか、どの結果が受け入れられないかを決め、その限界を方針として記録します。
* **委任の表の内側で実行するAI**: 各操作を、アラートのまとめのようにAIが単独で行えるもの、ノードの隔離のように人の承認が必要なもの、自らの権限の変更や監督の無効化のようにAIが決して行えないものに分類します。
* **影響に比例した承認**: 取り消せない度合いや影響の広さが大きい操作ほど、多くの人による確認を求めます。こうして定型的な作業は速いまま、ミッションを終わらせたり人を傷つけたりし得る判断には、慎重な注意が払われます。

### 3. パートナーシップを誠実に保つガードレール
監督、試験、および追跡可能性:

* **すべてのAIの行動を記録し、帰属させる**: AIが何を求められ、何を行い、どのツールを使い、どの人が承認したかを記録に残し、どの結果も説明責任を負う責任者までたどれるようにします。
* **導入の前後の敵対的な試験**: レッドチームが、軌道上のAIエージェントに対して、プロンプトインジェクション、作業の分割、接続されたツールの悪用を試みます。その結果は、NIST AIリスクマネジメントフレームワークとISO/IEC 42001に基づく統治に反映します。
* **設計に書き込まれた監督の規則**: EU AI法第14条が高リスクのシステムに求める人による監督と整合させ、運用担当者はいつでもAIの判断を一時停止、上書き、または取り消すことができ、AIがその能力を取り除くことはできないようにします。

### 4. 人を強くするパートナーシップ
人間の最終権限と公正な未来:

* **人間の最終権限の規則（提案）**: どれほど有能でも、安全、権利、雇用、ミッションに影響する行動について、AIシステムが最終的な決定権を持つことはありません。この規則により、モデルが強力になっても説明責任は明確に保たれます。
* **AIは有能な人を置き換えるのではなく引き上げるべき**: うまく使えば、AIにより熟練した専門家や才能ある一般の人々が、かつては大きなチームを必要とした仕事を担えるようになります。組織はその成果を、システムの安全を支える判断力を持つ人々を切り捨てるためではなく、キャリアを伸ばすために使うべきです。
* **恩恵を分かち合うための未来の設計**: 社会が最も安全なのは、AIの恩恵が、最も裕福な人や最も稀な才能を持つ狭い集団ではなく、多くの人々に届くときです。人間の権限を守り抜くセキュリティの専門家は、その均衡がとれ、安心できる未来を築く役割を担っています。

### 5. 結論
AIが信頼できるパートナーになるのは、無制限の自律を与えられることによってではなく、人が定め、試験し、強制する境界の内側で働くことによってであり、軌道上で動くAIの可能性と、2025年のAIエージェントの悪用の両方がそれを明らかにしています。

委任の表、影響に比例した承認、完全な追跡可能性、そしてCISSP資格の専門家が守る人間の最終権限の規則により、軌道上のAIは機械の速度で行動しながら、ミッションと人生を形づくる判断の責任は人が持ち続けます。
