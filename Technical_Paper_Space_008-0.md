# Koki's Technical Paper — Space Cyber Defense Series SCD-008

## The Neutral Orbit — Fair Access, Concentration Risk, and Keeping Space Infrastructure Open and Secure for Everyone

### Summary Digest
Space infrastructure is becoming highly concentrated: as of late October 2026, about two-thirds of all active satellites belonged to one constellation, while the European Union is building its own IRIS² system of about 290 satellites, with governmental services planned by 2030, to secure sovereign and resilient connectivity.

This paper applies CISSP Domains 1 and 3 to fairness and concentration in orbit, arguing that dependence on any single provider is a security risk, that open standards and shared rules protect resilience, and that decisions about access to essential space services must be made by accountable people with the public interest in mind.

---
### 1. Why Concentration Is a Security Risk
One Provider, Many Dependents:

* **Single Points of Failure Grow With Market Share**: When governments, businesses, and emergency services rely heavily on one network, a cyberattack, technical failure, or policy decision affecting that provider can disrupt them all at once.
* **Bargaining Power Becomes Leverage**: A dominant provider can set terms of access that customers cannot easily refuse, and in a crisis those terms may not match the public interest.
* **Diversity Has Begun to Grow**: Amazon reported in July 2026 that it had about 396 satellites in orbit and enough to begin initial service later that year, and Europe's IRIS² aims to provide sovereign connectivity, both of which reduce reliance on a single operator over time.

### 2. Principles for a Neutral Orbit
Shared Heritage, Open Standards, and Diversity:

* **Space Belongs to Everyone**: The Outer Space Treaty states that the exploration and use of outer space shall be carried out for the benefit and in the interests of all countries, a principle that should guide how essential services are offered.
* **Open Standards Enable Choice**: Common protocols, such as CCSDS standards and the U.S. Space Development Agency's standardized optical terminal interface, allow users to switch or combine providers and allow different builders' satellites to work together.
* **Design for Multi-Provider Resilience**: Critical users connect through more than one network where possible, so that losing one provider does not leave them without communication or navigation.

### 3. AI and Fairness Under Human Governance
Automated Allocation Without Hidden Bias:

* **AI Manages Capacity at Scale**: Large networks use AI to allocate bandwidth, route traffic, and prioritize users, decisions that can quietly favor some customers or regions over others.
* **Allocation Models Can Be Manipulated or Biased**: Poisoned demand data or biased training could steer capacity away from certain users, consistent with the risks described in NIST AI 100-2e2025, so allocation outcomes are audited for fairness.
* **Proposed Access Fairness Rule**: AI may allocate capacity within published policies, but cutting off service to a region, changing priority rules for emergency or public-interest users, or denying access to a class of customers requires approval by accountable people and, where appropriate, notification to regulators.

### 4. A Fair Future for Space Professionals and Users
Many Providers, Many Careers, Many Voices:

* **Diversity of Providers Supports Diversity of Jobs**: More operators in more countries create opportunities for engineers, analysts, and security professionals worldwide, rather than concentrating expertise in a few organizations.
* **Public-Interest Decisions Need Human Judgment**: Deciding how essential services are shared in emergencies involves ethics, law, and diplomacy, areas where qualified people, not algorithms, must remain responsible.
* **CISSP Supports Governance and Resilience**: CISSP Domain 1 covers governance, third-party risk, and business continuity, helping organizations evaluate and reduce dependence on any single provider.

### 5. Conclusion
When most of the world's satellites belong to one network, concentration itself becomes a security risk, because failures, attacks, or decisions at one provider can affect everyone.

Shared principles of benefit for all, open standards, multi-provider resilience, AI allocation audited for fairness, and accountable people who decide on access keep orbit neutral and secure for every user.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-008

## 中立な軌道 — 公平な利用、集中のリスク、および宇宙のインフラを誰にとっても開かれた安全なものに保つ

### サマリー・ダイジェスト
宇宙のインフラは大きく集中しつつあります。2026年10月下旬の時点で、稼働中のすべての衛星の約3分の2が1つの衛星群に属していました。一方で欧州連合は、主権を持つ回復力のある通信を確保するため、約290基の衛星からなる独自のIRIS²を構築しており、2030年までに政府向けのサービスを始める計画です。

本論文はCISSPのドメイン1と3を、軌道上の公平さと集中に適用します。単一の事業者への依存はセキュリティのリスクであり、公開の標準と共有のルールが回復力を守ること、そして欠かせない宇宙のサービスへのアクセスについての判断は、公共の利益を考える説明責任のある人々が行わなければならないことを論じます。

---
### 1. 集中がセキュリティのリスクである理由
1つの事業者と、多くの依存者:

* **単一障害点は市場の占有率とともに大きくなる**: 政府、企業、緊急サービスが1つのネットワークに大きく頼っていると、その事業者に影響するサイバー攻撃、技術的な故障、方針の決定が、それらすべてを一度に混乱させることがあります。
* **交渉力がてこになる**: 支配的な事業者は、利用者が簡単には断れない利用条件を決められ、危機のときにはその条件が公共の利益と合わないかもしれません。
* **多様性は育ち始めている**: Amazonは2026年7月、約396基の衛星が軌道上にあり、その年のうちに初期のサービスを始められる数に達したと報告しました。欧州のIRIS²は主権を持つ通信を目指しています。どちらも、時間をかけて1つの事業者への依存を減らします。

### 2. 中立な軌道のための原則
共有の遺産、公開の標準、および多様性:

* **宇宙はすべての人のもの**: 宇宙条約は、宇宙空間の探査と利用は、すべての国の利益のために、すべての国の関心に沿って行われなければならないと定めています。この原則は、欠かせないサービスをどう提供するかの指針になるべきです。
* **公開の標準が選択を可能にする**: CCSDSの標準や、米国宇宙開発庁（SDA）の標準化された光通信端末の接続方式のような共通のプロトコルは、利用者が事業者を切り替えたり組み合わせたりすることを可能にし、別々の製造者の衛星が一緒に働けるようにします。
* **複数の事業者を前提とした回復力の設計**: 重要な利用者は、できるかぎり複数のネットワークを通じてつながります。1つの事業者を失っても、通信や測位を失わずに済むようにするためです。

### 3. 人の統治のもとでのAIと公平さ
隠れた偏りのない自動の割り当て:

* **AIが大規模な容量を管理する**: 大きなネットワークは、AIを使って通信容量を割り当て、通信の経路を決め、利用者の優先順位をつけます。こうした判断は、ひそかに一部の利用者や地域をほかより優遇することがあります。
* **割り当てのモデルは操作されたり偏ったりし得る**: 汚染された需要のデータや偏った学習は、NIST AI 100-2e2025が示すリスクと同じように、特定の利用者から容量をそらすかもしれません。そのため、割り当ての結果は公平さの観点から監査します。
* **アクセスの公平さの規則（提案）**: AIは公表された方針の範囲内で容量を割り当ててかまいません。しかし、ある地域へのサービスを止めること、緊急や公共の利益のための利用者の優先順位の規則を変えること、ある種類の利用者へのアクセスを拒むことには、説明責任を負う人の承認と、必要に応じて規制当局への通知を必須とします。

### 4. 宇宙の専門家と利用者にとっての公正な未来
多くの事業者、多くの仕事、多くの声:

* **事業者の多様性が仕事の多様性を支える**: より多くの国により多くの事業者がいれば、少数の組織に専門性を集中させるのではなく、世界中の技術者、分析担当者、セキュリティの専門家に機会が生まれます。
* **公共の利益の判断には人の判断が要る**: 緊急時に欠かせないサービスをどう分かち合うかを決めることには、倫理、法律、外交が関わります。そこでは、アルゴリズムではなく有資格の人が責任を負い続けなければなりません。
* **CISSPがガバナンスと回復力を支える**: CISSPのドメイン1は、ガバナンス、第三者のリスク、事業継続を扱い、組織が単一の事業者への依存を評価し、減らす助けになります。

### 5. 結論
世界の衛星のほとんどが1つのネットワークに属するとき、集中そのものがセキュリティのリスクになります。1つの事業者での故障、攻撃、判断が、すべての人に影響し得るからです。

すべての人の利益という共有の原則、公開の標準、複数の事業者による回復力、公平さの観点から監査されるAIの割り当て、そしてアクセスを決める説明責任のある人々が、軌道をすべての利用者にとって中立で安全なものに保ちます。
