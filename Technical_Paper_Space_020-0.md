# Koki's Technical Paper — Space Cyber Defense Series SCD-020

## Astraeus Shield Integration — One Security Architecture Linking Ground, Space, and Cloud

### Summary Digest
The first nineteen papers of this series examined separate parts of space cyber defense: threat actors, laser links, power and robotics, swarm security, debris, orbital computing, supply chains, fair access, state threats, timing, reconnaissance, AI agents, self-repair, authentication, data hygiene, incident response, mesh networks, ethics, and resilience. Real missions, however, are defended as a whole. U.S. Space Policy Directive 5 of September 2020 defines a space system as a combination of ground systems, sensor networks, and space vehicles, NIST IR 8401 of December 2022 applies the Cybersecurity Framework to the satellite ground segment, and NIST Cybersecurity Framework 2.0, released on February 26, 2024, adds a Govern function that connects security to mission priorities.

This main paper of SCD-020 integrates the first half of the series into one architecture called the Astraeus Shield. It applies CISSP Domains 1, 3, and 7, describes how operations, architecture, roles, maturity, and mission assurance fit together, and shows why people must govern the whole.

---
### 1. Why Integration Is Needed
Separate Controls, Shared Weaknesses:

* **Attacks Cross Boundaries**: Real incidents, such as the 2022 attack that entered through a ground network and disabled user terminals, move across ground, space, and user segments, so isolated defenses leave gaps.
* **Many Organizations Share One Mission**: Satellite operators, ground station providers, cloud services, and suppliers each control part of a mission, and security must connect their responsibilities.
* **Space and Terrestrial Security Are One Discipline**: Space Policy Directive 5 states that cybersecurity principles that apply to terrestrial systems also apply to space systems, while some principles are particularly important in space.

### 2. Five Elements of the Astraeus Shield
A Structure for the SCD-020 Series:

* **Integrated Operations**: SCD-020-1 describes a security operations center that watches ground, space, and cloud together.
* **One Reference Architecture**: SCD-020-2 assembles the lessons of SCD-001 to SCD-019 into one layered design.
* **Clear Roles, Measured Progress, Clear Purpose**: SCD-020-3 defines roles and responsibilities, SCD-020-4 measures maturity with CSF 2.0, and SCD-020-5 explains mission assurance as the purpose of all security work.

### 3. AI Across the Integrated Shield
One Intelligence Layer, Many Human Decisions:

* **AI Connects Signals Across Segments**: AI can correlate events from ground stations, spacecraft telemetry, cloud services, and threat intelligence into a single picture.
* **Integration Creates a High-Value Target**: A unified AI layer that sees everything could become a single point of failure or manipulation, consistent with NIST AI 100-2e2025, so it is protected, monitored, and limited in authority.
* **Proposed Integration Authority Rule**: AI may correlate, prioritize, and recommend across all segments, but actions affecting more than one segment or more than one mission, such as fleet-wide containment, are approved by a qualified mission security lead.

### 4. People Who Hold the Whole Together
Integration Is a Human Achievement:

* **Integration Requires Communication**: Engineers, operators, security analysts, and partner organizations must share information and trust each other, which no tool can create alone.
* **Experienced Generalists Are Valuable**: Professionals who understand ground systems, spacecraft, networks, and governance can see how parts fit together, and the CISSP's broad scope prepares people for exactly this role.
* **CISSP Supports Integrated Security**: CISSP Domain 1 covers governance and risk, Domain 3 covers security architecture, and Domain 7 covers security operations across environments.

### 5. Conclusion
Space cyber defense succeeds only when ground, space, and cloud are protected as one system, governed by clear priorities and connected by shared operations.

The Astraeus Shield brings together the lessons of the first half of this series into one architecture, supported by AI and guided by people, so that missions can deliver their services safely and the people who depend on them can trust what space provides.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-020

## アストレアの盾の統合 — 地上、宇宙、クラウドを結ぶひとつのセキュリティの設計

### サマリー・ダイジェスト
このシリーズの最初の19本の論文は、宇宙のサイバー防衛の別々の部分を調べてきました。攻撃者、レーザー通信、電力と保守ロボット、群れのセキュリティ、宇宙ごみ、軌道上の計算基盤、サプライチェーン、公平な利用、国家による脅威、時刻、偵察、AIエージェント、自己修復、認証、データの衛生、インシデント対応、メッシュのネットワーク、倫理、そして回復力です。しかし実際のミッションは、全体として守られます。2020年9月の米国の宇宙政策指令5は、宇宙システムを、地上のシステム、センサーのネットワーク、宇宙機の組み合わせと定めています。2022年12月のNIST IR 8401は、サイバーセキュリティ・フレームワークを衛星の地上部分に当てはめました。そして2024年2月26日に公表されたNISTのサイバーセキュリティ・フレームワーク2.0は、セキュリティをミッションの優先順位とつなぐ「統治（Govern）」の機能を加えました。

SCD-020の本編である本論文は、シリーズの前半を「アストレアの盾」と呼ぶひとつの設計にまとめます。CISSPのドメイン1、3、7を適用し、運用、設計、役割、成熟度、ミッション保証がどう組み合わさるかを説明し、全体を人が治めなければならない理由を示します。

---
### 1. 統合が必要な理由
別々の統制、分け合う弱さ:

* **攻撃は境界を越える**: 地上のネットワークから入り、利用者の端末を使えなくした2022年の攻撃のように、本当のインシデントは地上、宇宙、利用者の部分をまたいで動くため、ばらばらの防御はすき間を残します。
* **多くの組織がひとつのミッションを分け合う**: 衛星の運用者、地上局の提供者、クラウドのサービス、供給業者がそれぞれミッションの一部を管理しており、セキュリティはそれぞれの責任をつながなければなりません。
* **宇宙と地上のセキュリティはひとつの分野**: 宇宙政策指令5は、地上のシステムに当てはまるサイバーセキュリティの原則は宇宙システムにも当てはまる一方で、宇宙で特に大切な原則もあると述べています。

### 2. アストレアの盾の5つの要素
SCD-020シリーズの構成:

* **統合した運用**: SCD-020-1は、地上、宇宙、クラウドを一緒に見張るセキュリティ運用センターを説明します。
* **ひとつの参照の設計**: SCD-020-2は、SCD-001からSCD-019の教訓を、ひとつの層を重ねた設計に組み立てます。
* **はっきりした役割、測られた進歩、はっきりした目的**: SCD-020-3は役割と責任を定め、SCD-020-4はCSF 2.0で成熟度を測り、SCD-020-5は、すべてのセキュリティの仕事の目的としてのミッション保証を説明します。

### 3. 統合した盾の全体にわたるAI
ひとつの知能の層、多くの人の判断:

* **AIが部分をまたいで信号をつなぐ**: AIは、地上局、宇宙機のテレメトリ、クラウドのサービス、脅威情報からの出来事を、ひとつの全体像に結びつけられます。
* **統合は価値の高い標的を生む**: すべてを見渡す一体のAIの層は、ひとつの弱点や操作の的になりうるため、守り、見張り、権限を限ります。これはNIST AI 100-2e2025と同じ趣旨です。
* **統合の権限の規則（提案）**: AIはすべての部分にまたがって、結びつけ、優先順位を付け、勧めてかまいません。しかし、機体の群れ全体の封じ込めのように、2つ以上の部分や2つ以上のミッションに影響する行動は、有資格のミッション・セキュリティの責任者が承認します。

### 4. 全体をまとめる人々
統合は人が成し遂げるもの:

* **統合には意思の疎通が要る**: 技術者、運用担当者、セキュリティの分析担当者、協力する組織は、情報を分け合い、お互いを信頼しなければならず、それはどんな道具もひとりではつくれません。
* **経験のある幅広い専門家は貴重**: 地上のシステム、宇宙機、ネットワーク、ガバナンスを理解する専門家は、部分がどう組み合わさるかを見渡せます。そしてCISSPの幅広い範囲は、まさにこの役割に人を備えさせます。
* **CISSPが統合したセキュリティを支える**: CISSPのドメイン1はガバナンスとリスクを、ドメイン3はセキュリティの設計を、ドメイン7は環境をまたいだセキュリティの運用を扱います。

### 5. 結論
宇宙のサイバー防衛は、地上、宇宙、クラウドが、はっきりした優先順位に治められ、分け合う運用でつながれた、ひとつのシステムとして守られたときにだけ成功します。

アストレアの盾は、このシリーズの前半の教訓をひとつの設計にまとめ、AIに支えられ、人に導かれます。そうすることで、ミッションは安全にサービスを届け、それに頼る人々は、宇宙がもたらすものを信頼できます。
