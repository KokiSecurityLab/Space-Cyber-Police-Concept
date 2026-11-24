# Koki's Technical Paper — Space Cyber Defense Series SCD-016

## Orbital Response Units — Incident Response for Space Systems Under NIST SP 800-61 Revision 3

### Summary Digest
When a cyber incident affects a space system, the response must reach from ground networks to spacecraft hundreds or thousands of kilometers away. NIST finalized Special Publication 800-61 Revision 3 on April 3, 2025, replacing the 2012 incident handling guide and treating incident response as part of cybersecurity risk management across all functions of the Cybersecurity Framework 2.0. In 2026, space organizations practiced these skills more than ever, from a U.S. Space Command tabletop series with commercial partners to new commercial missions that can inspect satellites up close.

This main paper of SCD-016 introduces incident response for space systems. It applies CISSP Domains 1, 7, and 4, explains how cyber and physical responses connect, and shows why trained people must lead every major response decision.

---
### 1. Why Space Incident Response Is Different
Distance, Physics, and Shared Consequences:

* **Limited Contact Windows**: Operators may reach a satellite only during short passes over ground stations, so response actions must be planned and prioritized carefully.
* **Cyber Effects Can Become Physical**: The 2022 attack on a satellite network disrupted remote monitoring of about 5,800 wind turbines in Germany and Central Europe, showing how space incidents spread into other critical services.
* **Recovery Options Are Constrained**: Spacecraft cannot be visited or replaced quickly, so responders must preserve the mission while removing the threat.

### 2. Five Capabilities of an Orbital Response Unit
A Structure for the SCD-016 Series:

* **Connect Cyber and Physical Response**: SCD-016-1 explains how cyber teams, flight dynamics, and space safety work together.
* **Isolate and Inspect**: SCD-016-2 covers isolating compromised satellites from networks and constellations, and SCD-016-3 covers on-orbit inspection to confirm what has happened.
* **Prepare and Coordinate**: SCD-016-4 describes playbooks and exercises, and SCD-016-5 explains coordinated defense with partners and authorities rather than independent retaliation.

### 3. AI-Assisted Response Under Human Command
Speed for Analysis, Judgment for Action:

* **AI Speeds Triage**: AI can correlate alerts from ground networks, telemetry, and threat intelligence to suggest what is happening and which assets are at risk.
* **Response Tools Can Be Targeted**: Attackers may feed misleading data to automated response systems to trigger harmful actions, consistent with NIST AI 100-2e2025, so automated actions are limited and logged.
* **Proposed Orbital Response Rule**: AI may gather evidence, recommend actions, and execute pre-approved containment steps on ground systems, but commanding a spacecraft to change configuration, maneuver, or shut down a payload during an incident is approved by a qualified incident commander together with flight operations.

### 4. Responders as the Core of Resilience
People Who Stay Calm When Systems Fail:

* **Incident Response Needs Many Skills**: Effective response combines cyber analysts, satellite engineers, legal advisers, and communications staff, and these teams cannot be replaced by automation.
* **The Industry Needs More Experienced Defenders**: Space industry leaders have noted that the satellite sector still needs creative, experienced cyber professionals who can anticipate and respond to new threats.
* **CISSP Provides a Shared Language**: CISSP Domain 1 covers legal and regulatory obligations, Domain 7 covers incident management and recovery, and Domain 4 covers network containment.

### 5. Conclusion
Incident response for space systems must bridge long distances, limited contact, and physical consequences, while following the continuous risk management approach of NIST SP 800-61 Revision 3.

By connecting cyber and physical response, isolating and inspecting affected assets, practicing with realistic exercises, coordinating with partners, and keeping trained people in command, the space community can respond to incidents with confidence and keep essential services available for everyone.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-016

## 軌道の対応部隊 — NIST SP 800-61 Rev.3にもとづく宇宙システムのインシデント対応

### サマリー・ダイジェスト
サイバーのインシデントが宇宙システムに影響すると、その対応は、地上のネットワークから、何百キロ、何千キロも離れた宇宙機にまで届かなければなりません。NISTは2025年4月3日に特別出版物SP 800-61 Rev.3を確定させ、2012年のインシデント対応の手引きに代えて、インシデント対応を、サイバーセキュリティ・フレームワーク2.0のすべての機能にわたるサイバーセキュリティのリスク管理の一部として扱いました。2026年、宇宙の組織はこれまで以上にこうした技能を練習しました。民間の協力企業と行う米宇宙軍の統合軍の机上演習から、衛星を近くから点検できる新しい民間のミッションまでです。

SCD-016の本編である本論文は、宇宙システムのインシデント対応を紹介します。CISSPのドメイン1、7、4を適用し、サイバーと物理の対応がどうつながるかを説明し、大きな対応の判断はすべて、訓練を受けた人が率いなければならない理由を示します。

---
### 1. 宇宙のインシデント対応が違う理由
距離、物理、分かち合う結果:

* **限られた交信の時間**: 運用担当者が衛星に届くのは、地上局の上を通る短い時間だけのことがあるため、対応の行動は注意深く計画し、優先順位を付けなければなりません。
* **サイバーの影響は物理的になりうる**: 2022年の衛星ネットワークへの攻撃は、ドイツと中央ヨーロッパの約5,800基の風力発電機の遠隔監視を乱し、宇宙のインシデントがほかの重要なサービスにまで広がることを示しました。
* **回復の選択肢は限られる**: 宇宙機には行くことも、すぐに取り替えることもできないため、対応する人は、脅威を取り除きながら、ミッションを守らなければなりません。

### 2. 軌道の対応部隊の5つの力
SCD-016シリーズの構成:

* **サイバーと物理の対応をつなぐ**: SCD-016-1は、サイバーのチーム、軌道力学、宇宙の安全の担当がどう協力するかを説明します。
* **切り離し、点検する**: SCD-016-2は乗っ取られた衛星をネットワークとコンステレーションから切り離すことを、SCD-016-3は何が起きたかを確かめるための軌道上の点検を扱います。
* **備え、連携する**: SCD-016-4は対応手順書と演習を、SCD-016-5は独自の報復ではなく、協力相手や当局と連携した防御を説明します。

### 3. 人の指揮の下での、AIによる対応の支援
分析には速さを、行動には判断を:

* **AIが振り分けを速くする**: AIは、地上のネットワーク、テレメトリ、脅威情報からの警報を結びつけ、何が起きているか、どの資産が危ないかを示せます。
* **対応の道具も狙われることがある**: 攻撃者は、有害な行動を起こさせるために、自動の対応のシステムにまぎらわしいデータを流すかもしれません。これはNIST AI 100-2e2025と同じ趣旨です。そのため、自動の行動は限り、記録します。
* **軌道の対応の規則（提案）**: AIは証拠を集め、行動を勧め、地上のシステムで前もって承認された封じ込めの手順を実行してかまいません。しかし、インシデントの間に宇宙機の設定を変えること、軌道を変えること、搭載機器を止めることを命じるのは、有資格のインシデントの指揮者が飛行運用の担当と一緒に承認します。

### 4. 回復力の中心としての対応者
システムが止まったときにも落ち着いていられる人々:

* **インシデント対応には多くの技能が要る**: 効果的な対応には、サイバーの分析担当者、衛星の技術者、法律の助言者、広報の担当者が組み合わさり、こうしたチームは自動化では置き換えられません。
* **業界は経験のある守り手をもっと必要としている**: 宇宙業界の指導者たちは、衛星の分野には、新しい脅威を予測して対応できる、創造的で経験のあるサイバーの専門家がまだ必要だと指摘しています。
* **CISSPが共通の言葉を与える**: CISSPのドメイン1は法律と規制上の義務を、ドメイン7はインシデントの管理と復旧を、ドメイン4はネットワークの封じ込めを扱います。

### 5. 結論
宇宙システムのインシデント対応は、NIST SP 800-61 Rev.3の継続的なリスク管理の考え方に沿いながら、長い距離、限られた交信、物理的な結果を橋渡ししなければなりません。

サイバーと物理の対応をつなぎ、影響を受けた資産を切り離して点検し、現実的な演習で練習し、協力相手と連携し、訓練を受けた人が指揮を執り続けることで、宇宙の世界はインシデントに自信をもって対応し、みんなに欠かせないサービスを使える状態に保てます。
