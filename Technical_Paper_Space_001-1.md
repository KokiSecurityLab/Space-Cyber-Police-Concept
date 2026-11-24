# Koki's Technical Paper — Space Cyber Defense Series SCD-001-1

## Adversary Capability Assessment — Separating Visible Aggression From Real Capability, Noise-Versus-Signal Triage, and Calm Response Discipline

### Summary Digest
Loud activity such as mass scanning or denial-of-service floods is easy to see but often reveals little about what an attacker can truly do, as the February 2022 attack on Viasat's KA-SAT network showed when the outage first looked like a flood of traffic but proved to be AcidRain wiper malware that disabled modems across Europe and cut remote control of 5,800 Enercon wind turbines in Germany.

Building on SCD-001 under CISSP Domain 7, this paper assesses adversaries by demonstrated capability rather than apparent aggression, uses AI to sort the growing volume of machine-generated noise, and relies on experienced human analysts to judge intent and decide the response.

---
### 1. When Aggression Misleads Defenders
How Visible Pressure Distorts Judgment:

* **Volume Is Not Capability**: Internet-wide scanning and automated exploit attempts reach every exposed service many times a day, and treating each burst as a sophisticated threat exhausts analysts while quieter, more capable activity goes unexamined.
* **Noise as a Smokescreen**: In the Viasat case, attackers entered through a misconfigured VPN appliance into the network's trusted management segment, while early reporting focused on traffic floods, showing that the most visible signal is not always the one that matters.
* **AI Multiplies Low-Cost Noise**: Generative AI lets attackers produce phishing text, scanning scripts, and fake traffic at almost no cost, so defenders can no longer read volume as a measure of the adversary's skill or commitment.

### 2. Evidence-Based Capability Assessment
Observed Techniques, Infrastructure, and Persistence:

* **Grade What the Adversary Has Demonstrated**: Capability is rated from evidence such as custom malware, valid credential use, or access to management networks, mapped to MITRE ATT&CK for ground systems and SPARTA for spacecraft techniques, rather than from the force or tone of the attack.
* **Track Infrastructure and Persistence**: Reused command servers, code overlaps, such as those SentinelLabs observed between AcidRain and the earlier VPNFilter malware, and attempts to survive reboots indicate an organized, persistent actor worth priority.
* **Separate Disruption From Destruction**: An outage that recovers when traffic stops differs fundamentally from firmware that has been overwritten, and Viasat ultimately shipped nearly 30,000 replacement modems, a cost that capability assessment must anticipate before an attack, not after.

### 3. Triage Through Human-AI Teaming
Machine-Speed Filtering With Human Judgment:

* **AI Clusters and Suppresses Routine Noise**: Defensive AI groups repetitive scans, known botnet traffic, and commodity exploit attempts, and enriches them with threat intelligence so the queue that reaches analysts holds events that are new, targeted, or touching critical assets.
* **Experienced Analysts Judge Intent**: Deciding whether unusual activity is reconnaissance for a mission-ending attack requires context about operations, geopolitics, and the organization's own systems that a qualified professional, applying CISSP Domain 7 practices, brings to the decision.
* **Calm, Documented Response**: Responders follow prepared playbooks, record their reasoning, and escalate by evidence rather than alarm, so a dramatic but harmless flood does not trigger a damaging shutdown of a healthy constellation.

### 4. Sustaining the Analysts Who Separate Signal From Noise
Experience, Training, and Fair Workloads:

* **Pattern Recognition Comes From People Who Stay**: The ability to notice that a small anomaly resembles a past intrusion grows over years in one environment, so organizations that replace experienced analysts with automation lose the memory that triage depends on.
* **AI Should Remove Drudgery, Not Careers**: Assigning repetitive filtering to AI frees analysts for investigation and threat hunting, and the gain should be reinvested in training and deeper defense rather than in cutting the people who interpret what the machines surface.
* **A Broad Bench of Capable Defenders**: Orbital networks, ground stations, and suppliers each need trained people on duty, which makes a wide workforce of skilled professionals, not a narrow circle of experts, the real measure of a society prepared for AI-enabled attacks.

### 5. Conclusion
Visible aggression and real capability are different things, and an adversary is best measured by demonstrated techniques, infrastructure, and persistence, as the hidden wiper behind the apparent flood in the Viasat attack made clear.

AI that filters machine-generated noise, analysts who judge intent and own the response, and organizations that keep those analysts rather than replace them let defenders stay calm and accurate when AI-amplified attacks try to overwhelm them.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-001-1

## 攻撃者の能力評価 — 目に見える攻撃性と実際の能力の区別、雑音と兆候の選別、および冷静な対応の規律

### サマリー・ダイジェスト
大量のスキャンやサービス妨害の通信の洪水のような目立つ活動は見つけやすい一方で、攻撃者が本当に何をできるかについてはほとんど示しません。2022年2月のViasatのKA-SATネットワークへの攻撃では、障害は当初、通信の洪水のように見えましたが、実際にはAcidRainというワイパー型マルウェアが欧州各地のモデムを使用不能にし、ドイツの5,800基のEnercon製風力発電機の遠隔制御を断っていました。

本論文はSCD-001を踏まえ、CISSPのドメイン7に基づいて、攻撃者を見かけの攻撃性ではなく実証された能力で評価し、増え続ける機械生成の雑音の選別にAIを用い、意図の判断と対応の決定は経験豊富な人間の分析担当者に委ねます。

---
### 1. 攻撃性が防御側を惑わすとき
目に見える圧力が判断をゆがめる経緯:

* **量は能力ではない**: インターネット全体へのスキャンや自動化された攻撃の試みは、公開されたすべてのサービスに1日に何度も届きます。その一つひとつを高度な脅威として扱えば分析担当者は疲弊し、より静かで能力の高い活動が調べられないまま残ります。
* **煙幕としての雑音**: Viasatの事例では、攻撃者は設定に不備のあったVPN機器から、ネットワークの信頼された管理区画に侵入していました。一方、初期の報道は通信の洪水に注目しており、最も目立つ兆候が最も重要な兆候とは限らないことを示しています。
* **低コストの雑音を増幅するAI**: 生成AIにより、攻撃者はフィッシングの文面、スキャン用のスクリプト、偽の通信をほとんど費用をかけずに作り出せます。そのため防御側は、量を攻撃者の技能や本気度の尺度として読むことができなくなりました。

### 2. 証拠に基づく能力評価
観測された手法、インフラ、および持続性:

* **実証されたものによる評価**: 能力は、攻撃の勢いや口調ではなく、独自開発のマルウェア、正規の資格情報の使用、管理ネットワークへのアクセスなどの証拠から評価し、地上システムについてはMITRE ATT&CKに、宇宙機の手法についてはSPARTAに対応付けます。
* **インフラと持続性の追跡**: 再利用される指令サーバ、SentinelLabsがAcidRainとそれ以前のVPNFilterマルウェアの間に見出したようなコードの重なり、再起動後も生き残ろうとする試みは、優先して扱うべき組織的で執拗なアクターであることを示します。
* **妨害と破壊の区別**: 通信が止まれば回復する障害と、ファームウェアが上書きされた状態とは根本的に異なります。Viasatは最終的に交換用のモデムを3万台近く出荷しており、能力評価は攻撃の後ではなく前に、こうした費用を見込んでおく必要があります。

### 3. 人とAIの協働による選別
機械の速度での絞り込みと人間の判断:

* **定型的な雑音をまとめて抑えるAI**: 防御のAIは、繰り返されるスキャン、既知のボットネットの通信、汎用的な攻撃の試みをまとめ、脅威インテリジェンスで情報を補います。こうして分析担当者に届く待ち行列には、新しいもの、標的を絞ったもの、重要な資産に触れるものだけが残ります。
* **意図を判断する経験豊富な分析担当者**: 普段と異なる活動が、ミッションを終わらせる攻撃のための偵察かどうかを判断するには、運用、地政学、自組織のシステムについての文脈が必要です。それを判断に持ち込むのは、CISSPのドメイン7の実践を適用する有資格の専門家です。
* **冷静で記録に残る対応**: 対応者は準備されたプレイブックに従い、判断の理由を記録し、警戒心ではなく証拠によって段階を上げます。そうすることで、派手でも無害な通信の洪水が、健全な衛星群を停止させる有害な判断を引き起こさないようにします。

### 4. 雑音と兆候を見分ける分析担当者を支え続ける
経験、教育、および公正な業務量:

* **定着する人から生まれるパターン認識**: 小さな異常が過去の侵入に似ていると気づく力は、一つの環境で何年も働くうちに育ちます。そのため、経験豊富な分析担当者を自動化に置き換える組織は、選別を支える記憶を失います。
* **AIが奪うべきは単調な作業であってキャリアではない**: 繰り返しの絞り込みをAIに任せれば、分析担当者は調査や脅威ハンティングに時間を使えます。その成果は、機械が示したものを解釈する人々の削減ではなく、教育とより深い防御に再投資すべきです。
* **有能な防御者の幅広い層**: 軌道上のネットワーク、地上局、供給者のそれぞれに、訓練を受けた担当者が必要です。そのため、狭い専門家の輪ではなく、熟練した専門家の幅広い人材こそが、AIを使った攻撃に備えた社会の本当の尺度となります。

### 5. 結論
目に見える攻撃性と実際の能力は別のものであり、Viasatへの攻撃で見かけの洪水の裏に隠れていたワイパーが示したように、攻撃者は実証された手法、インフラ、持続性によって測るのが最善です。

機械生成の雑音を絞り込むAI、意図を判断して対応の責任を負う分析担当者、そしてその分析担当者を置き換えるのではなく支え続ける組織により、AIで増幅された攻撃が圧倒しようとしても、防御側は冷静で正確であり続けられます。
