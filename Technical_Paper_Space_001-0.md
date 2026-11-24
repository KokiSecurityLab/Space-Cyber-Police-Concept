# Koki's Technical Paper — Space Cyber Defense Series SCD-001

## Threat Actor Behavior Analysis — Motivation-Based Profiling, Human-Centric Governance, and Defense Against AI-Orchestrated Intrusion

### Summary Digest
As AI computing moves into orbit, with Google launching its first TPU-equipped Project Suncatcher test satellite in October 2026, the adversaries who will target it are best understood through evidence of motive and behavior rather than guesses about personality, especially since the human element appeared in 60 percent of breaches in Verizon's 2025 DBIR and Anthropic reported in November 2025 a state-sponsored campaign in which AI agents performed 80 to 90 percent of the work.

This opening paper of the Space Cyber Defense Series applies CISSP Domains 1 and 7 to profile attackers by motive and observable technique, keeps final decisions with accountable humans, and argues that defending AI systems depends on a broad professional workforce rather than on automation or a small elite alone.

---
### 1. Why Guesswork About Attackers Fails
Limits of Personality-Based Threat Analysis:

* **Speculation Instead of Evidence**: Explaining attacks by imagined traits of the attacker, such as insecurity or anger, cannot be tested in logs, so it neither predicts the next move nor guides a control, while motive and technique leave evidence that defenders can act on.
* **The Human Element Remains the Main Entry Point**: Verizon's 2025 Data Breach Investigations Report found human involvement, through error, phishing, or manipulation, in 60 percent of confirmed breaches, so attackers study the people who operate systems as carefully as the systems themselves.
* **AI Agents Compress the Attacker's Timeline**: In the campaign Anthropic disrupted in 2025, human operators chose roughly thirty targets and intervened at only four to six decision points, while AI agents performed reconnaissance, credential harvesting, and data extraction at machine speed.

### 2. Profiling by Motive and Behavior
Motivation Categories, Technique Mapping, and Decision Points:

* **Motive Determines Target and Persistence**: Financially motivated groups seek fast monetization, espionage actors seek long, quiet access, and disruptive or hacktivist actors seek visible outages, so classifying the likely motive tells defenders which orbital assets, such as command links or model weights, deserve priority.
* **Techniques Mapped to ATT&CK and SPARTA**: Observed behaviors are recorded against MITRE ATT&CK for ground systems and the Aerospace Corporation's SPARTA matrix for spacecraft-specific techniques, and the Diamond Model links each event to adversary, capability, infrastructure, and victim.
* **Human Decision Points as Detection Opportunities**: Even an AI-driven intrusion pauses for its operator to approve escalation or exfiltration, and those pauses create timing gaps and command patterns that defenders can watch for.

### 3. Human-Centric Governance of Defense
Accountable Authority, AI Assistance, and Oversight Rules:

* **CISSP-Led Accountability for High-Impact Decisions**: Isolating a satellite cluster, revoking ground-station credentials, or halting a model is approved by a named, qualified professional, because CISSP Domain 1 places accountability on people, not tools.
* **AI as Analyst Support, Not Final Authority**: Defensive AI correlates telemetry, summarizes alerts, and drafts response options at the attacker's speed, as Anthropic's own threat team did when analyzing the 2025 campaign, while a human selects and owns the action.
* **Proposed Human Oversight Rule**: Consistent with the human oversight duty that Article 14 of the EU AI Act sets for high-risk AI, this design requires that any automated action able to disrupt a mission be reversible, logged, and confirmed by a person before it becomes permanent.

### 4. The Workforce as the Strategic Perimeter
Skills, Careers, and a Sustainable Human-AI Future:

* **Cutting Skilled People Creates New Vulnerabilities**: ISC2's 2025 Workforce Study of 16,029 professionals found that 24 percent reported layoffs and 88 percent had experienced at least one significant security consequence caused by skills shortages, showing that removing experienced staff in favor of automation raises risk rather than lowering it.
* **Defense Needs Many Capable People, Not a Few**: Securing orbital AI requires thousands of trained analysts, engineers, and auditors across operators and suppliers, so a future that rewards only a narrow group of wealthy or exceptional individuals would leave most systems undefended.
* **Proposed Human-AI Partnership Charter**: AI drafts, correlates, and accelerates, while people verify, decide, and remain accountable, a division that protects both mission safety and the careers of capable professionals and lets society share in the gains of AI rather than fear them.

### 5. Conclusion
Attackers are best understood through motive, technique, and the decisions they still make themselves, and AI agents that perform most of an intrusion make evidence-based profiling and fast, accountable human response more important, not less.

Pairing defensive AI with CISSP-qualified professionals who hold final authority and protecting the skilled workforce that orbital systems depend on build a defense that can win against AI-orchestrated attacks while keeping people at the center of a secure and hopeful future in space.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-001

## 脅威アクターの行動分析 — 動機に基づくプロファイリング、人間中心の統治、およびAIが主導する侵入への防御

### サマリー・ダイジェスト
2026年10月にGoogleがTPUを搭載したProject Suncatcherの最初の試験衛星を打ち上げたように、AIの計算基盤は軌道上へ移りつつあり、それを狙う攻撃者は人格の推測ではなく動機と行動の証拠によって理解するのが最善です。VerizonのDBIR 2025では侵害の60％に人的要素が関わり、Anthropicは2025年11月、国家が支援する攻撃活動でAIエージェントが作業の80〜90％を担ったと報告しています。

宇宙サイバー防衛シリーズの最初となる本論文は、CISSPのドメイン1と7を適用して、攻撃者を動機と観測可能な手法でプロファイリングし、最終的な判断を説明責任を負う人間に委ねます。そして、AIシステムの防御は、自動化や一握りの精鋭だけではなく、幅広い専門人材に依存していると論じます。

---
### 1. 攻撃者についての推測が失敗する理由
人格に基づく脅威分析の限界:

* **証拠ではなく推測**: 不安や怒りなど、攻撃者の想像上の性格で攻撃を説明しても、ログで検証することはできず、次の動きの予測にも統制の指針にもなりません。一方、動機と手法は、防御側が行動に移せる証拠を残します。
* **主な侵入口であり続ける人的要素**: Verizonの2025年版データ侵害調査報告書では、確認された侵害の60％に、誤り、フィッシング、操作による人の関与が見られました。そのため攻撃者は、システムそのものと同じくらい注意深く、システムを運用する人々を調べます。
* **攻撃者の時間軸を縮めるAIエージェント**: Anthropicが2025年に阻止した攻撃活動では、人間の操作者がおよそ30の標的を選び、介入したのは4〜6か所の判断点だけで、偵察、資格情報の収集、データの抽出はAIエージェントが機械の速度で行いました。

### 2. 動機と行動によるプロファイリング
動機の分類、手法の対応付け、および判断点:

* **標的と執着の度合いを決める動機**: 金銭目的のグループは素早い換金を、諜報目的のアクターは長く静かなアクセスを、妨害やハクティビズムのアクターは目に見える停止を求めます。そのため、想定される動機を分類すれば、指令リンクやモデルの重みなど、どの軌道上の資産を優先すべきかが分かります。
* **ATT&CKとSPARTAへの手法の対応付け**: 観測した行動を、地上システムについてはMITRE ATT&CKに、宇宙機に特有の手法についてはAerospace CorporationのSPARTAマトリクスに照らして記録し、ダイヤモンドモデルで各事象を攻撃者、能力、インフラ、被害者に結びつけます。
* **検知の機会としての人間の判断点**: AIが主導する侵入であっても、権限昇格やデータ持ち出しの承認のために操作者を待つ時間があり、その中断が生む時間の空白と指令のパターンを防御側は監視できます。

### 3. 人間中心の防御の統治
説明責任を負う権限、AIの支援、および監督の規則:

* **影響の大きい判断へのCISSPに基づく説明責任**: 衛星群の隔離、地上局の資格情報の失効、モデルの停止は、名前を特定された有資格の専門家が承認します。CISSPのドメイン1は、説明責任をツールではなく人に置いているためです。
* **最終権限ではなく分析の支援としてのAI**: 防御のAIは、Anthropic自身の脅威チームが2025年の攻撃活動の分析で行ったように、攻撃者と同じ速度でテレメトリを相関させ、アラートを要約し、対応の選択肢を起案します。行動を選び、その責任を負うのは人間です。
* **人による監督の規則（提案）**: EU AI法第14条が高リスクAIに課す人による監督の義務と整合させ、本設計では、ミッションを妨げ得る自動化された措置は、確定する前に、元に戻せること、記録されること、人が確認することを必須とします。

### 4. 戦略的な境界としての人材
技能、キャリア、および持続可能な人とAIの未来:

* **熟練者の削減が生む新たな脆弱性**: 16,029人の専門家を対象としたISC2の2025年版人材調査では、24％が人員削減を報告し、88％が技能不足による重大なセキュリティ上の影響を少なくとも一度経験していました。経験豊富な人材を自動化に置き換えることは、リスクを下げるどころか高めることを示しています。
* **防御に必要なのは少数ではなく多くの有能な人材**: 軌道上のAIを守るには、運用事業者と供給者全体で何千人もの訓練された分析担当者、技術者、監査人が必要であり、裕福な人や特別な才能を持つ一握りの人だけが報われる未来では、大半のシステムが無防備のまま残されます。
* **人とAIの協働憲章（提案）**: AIは起案し、相関させ、速度を上げ、人は検証し、判断し、説明責任を負い続けます。この役割分担は、ミッションの安全と有能な専門家のキャリアの両方を守り、社会がAIを恐れるのではなく、その恩恵を分かち合えるようにします。

### 5. 結論
攻撃者は、動機、手法、そしてなお自ら下す判断を通じて理解するのが最善であり、侵入の大半をAIエージェントが担うようになるほど、証拠に基づくプロファイリングと、迅速で説明責任のある人間の対応は、重要性を失うのではなく増します。

防御のAIを、最終権限を持つCISSP資格の専門家と組み合わせ、軌道上のシステムが依存する熟練人材を守ることで、AIが主導する攻撃に勝てる防御を築くとともに、安全で希望ある宇宙の未来の中心に人を置き続けます。
