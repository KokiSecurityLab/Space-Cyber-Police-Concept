# Koki's Technical Paper — Space Cyber Defense Series SCD-004

## The Swarm Immunity — Immune-Inspired Collective Defense for Mega-Constellations, With Human Command Over the Response

### Summary Digest
Satellite fleets have grown into swarms: as of late October 2026, about 11,160 of the roughly 16,800 active satellites in Earth orbit were Starlink spacecraft, and no team of people can watch thousands of satellites one by one, so defense must be distributed across the fleet itself.

This paper applies CISSP Domains 3 and 7 to collective defense inspired by research on artificial immune systems, in which each satellite detects what is abnormal for itself, neighbors share warnings, and suspicious nodes are isolated, while people keep authority over decisions that could cut off service or harm innocent satellites.

---
### 1. Why Central Watching Is Not Enough
Scale, Delay, and Single Points of Failure:

* **The Numbers Exceed Human Attention**: With thousands of satellites in a single constellation, each producing streams of telemetry, a central team cannot review every signal in time to stop a fast-spreading compromise.
* **Ground Contact Is Intermittent**: A satellite may be out of contact with its operators for minutes or hours, so it must be able to recognize and resist obvious attacks on its own during those gaps.
* **A Single Control Center Is a Single Target**: If all detection depends on one ground site, an attacker who disrupts that site blinds the entire fleet, which argues for detection and response spread across many nodes.

### 2. Lessons From Artificial Immune Systems
Self, Non-Self, and Distributed Detection:

* **Learning What Belongs**: Artificial immune system research, particularly negative selection, trains detectors on normal behavior so that anything outside the learned "self" can be flagged, an approach suited to space systems where many attacks have no known signature.
* **Many Small Detectors, Not One Large One**: Like immune cells spread through the body, lightweight detectors on each satellite watch local behavior, while the fleet combines their reports to see patterns no single node could see.
* **Memory and Shared Warnings**: When one satellite detects a new attack pattern, a description of it is shared so others can recognize it quickly, much as immune memory speeds the response to a familiar infection.

### 3. Collective Response Under Human Authority
Automation for Speed, People for Consequences:

* **Local Containment Can Be Automatic**: A satellite that detects clear tampering may suspend non-essential functions and refuse unusual commands until operators review its state, a reversible step that limits harm.
* **The Swarm Itself Can Be Misled**: An attacker who controls a few nodes could send false warnings to trick the fleet into isolating healthy satellites, and detection models can be poisoned or evaded as described in NIST AI 100-2e2025, so collective decisions require corroboration from independent evidence.
* **Proposed Swarm Response Rule**: Automated systems may raise alerts and apply reversible local safeguards, but isolating a satellite from the network, pushing new detection rules to the whole fleet, or shutting down service to customers requires approval by a qualified operator.

### 4. The Human Immune System of the Organization
Distributed Teams, Shared Knowledge, and Fair Opportunity:

* **Defenders Should Be Distributed Too**: Just as detection is spread across satellites, expertise should be spread across many trained analysts, operators, and engineers in different locations and organizations, rather than concentrated in a few experts or one automated platform.
* **Sharing Strengthens Everyone**: Space ISAC opened its Operational Watch Center in March 2023 with a dedicated team of ten in-person analysts, an example of how shared human analysis complements automated detection across the industry.
* **CISSP as a Common Foundation**: CISSP Domains 3 and 7 give professionals across operators and suppliers a common language for designing and running collective defense, enabling capable people from many backgrounds to contribute.

### 5. Conclusion
Mega-constellations are too large and too often out of contact to be defended only from the ground, so detection and first response must be spread across the swarm, learning from research on artificial immune systems.

When satellites watch themselves and each other, while qualified people corroborate evidence and decide on serious responses, the swarm gains an immunity that is fast, resilient, and still accountable.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-004

## 群れの免疫 — 人工免疫システムに学ぶ巨大衛星群の集団防御と、対応への人の指揮

### サマリー・ダイジェスト
衛星の数は「群れ」と呼べるほどに増えました。2026年10月下旬の時点で、地球の軌道上で動いている約16,800基の衛星のうち、約11,160基がStarlinkの衛星でした。何千もの衛星を人が1基ずつ見張ることはできないため、防御は衛星群そのものに分散させなければなりません。

本論文はCISSPのドメイン3と7を、人工免疫システムの研究に学ぶ集団防御に適用します。各衛星は自分にとっての「異常」を見つけ、近くの衛星と警告を共有し、疑わしい衛星を隔離します。そのうえで、サービスを止めたり、罪のない衛星を傷つけたりし得る判断については、人が権限を持ち続けます。

---
### 1. 中央での見張りだけでは足りない理由
規模、遅れ、および単一障害点:

* **数が人の注意力を超えている**: 1つの衛星群に何千もの衛星があり、それぞれがテレメトリを送り続けています。中央のチームが、素早く広がる侵害を止めるのに間に合うよう、すべての信号を確認することはできません。
* **地上との通信は途切れがち**: 衛星は、運用者と数分から数時間通信できないことがあります。その間、衛星は明らかな攻撃を自分で見分け、抵抗できなければなりません。
* **1つの管制センターは1つの標的**: すべての検知が1か所の地上拠点に頼っていると、その拠点を妨害した攻撃者は衛星群全体の目をふさげます。これは、検知と対応を多くの拠点に分散すべき理由になります。

### 2. 人工免疫システムからの教訓
自己と非自己、そして分散型の検知:

* **何が「自分」かを学ぶ**: 人工免疫システムの研究、とくに「ネガティブ選択」という方法は、正常なふるまいで検知器を学習させ、学んだ「自己」の外にあるものを知らせます。多くの攻撃に既知のシグネチャがない宇宙システムに向いた方法です。
* **1つの大きな検知器ではなく、多くの小さな検知器**: 体中に散らばる免疫細胞のように、各衛星の軽い検知器がその場のふるまいを見張り、衛星群全体がその報告をまとめて、1基だけでは見えないパターンを見つけます。
* **記憶と共有される警告**: ある衛星が新しい攻撃のパターンを見つけたら、その特徴を共有し、ほかの衛星もすぐに見分けられるようにします。免疫の記憶が、なじみのある感染への反応を速めるのと同じです。

### 3. 人の権限のもとでの集団的な対応
速さのための自動化、結果のための人:

* **その場での封じ込めは自動でよい**: 明らかな改ざんを見つけた衛星は、運用者が状態を確かめるまで、欠かせない機能以外を止め、普段と違う指令を受け付けないようにしてかまいません。これは元に戻せる措置で、被害を小さくします。
* **群れそのものがだまされ得る**: 数基を乗っ取った攻撃者は、偽の警告を送って、衛星群に健全な衛星を隔離させるかもしれません。また、NIST AI 100-2e2025が示すように、検知のモデルは汚染されたり回避されたりします。そのため、集団での判断には、独立した証拠による裏づけを必須とします。
* **群れの対応の規則（提案）**: 自動のシステムは、警報を出し、元に戻せるその場の安全措置をとってかまいません。しかし、衛星をネットワークから隔離すること、新しい検知の規則を衛星群全体に配ること、利用者へのサービスを止めることには、有資格の運用者の承認を必須とします。

### 4. 組織の「人の免疫システム」
分散したチーム、共有される知識、および公正な機会:

* **防御者も分散させる**: 検知を衛星に分散させるのと同じように、専門知識も、少数の専門家や1つの自動化の仕組みに集中させるのではなく、さまざまな場所や組織にいる多くの訓練された分析担当者、運用者、技術者に分散させるべきです。
* **共有が皆を強くする**: Space ISACは2023年3月、10人の常駐の分析担当者を置いた運用監視センター（Operational Watch Center）を開きました。人による共有の分析が、業界全体で自動の検知を補う例です。
* **共通の土台としてのCISSP**: CISSPのドメイン3と7は、運用事業者や供給者にまたがる専門家に、集団防御を設計し運用するための共通の言葉を与えます。それにより、さまざまな経歴を持つ有能な人々が貢献できます。

### 5. 結論
巨大な衛星群は、あまりに大きく、地上と通信できない時間も長いため、地上からだけでは守り切れません。人工免疫システムの研究に学び、検知と初動の対応を群れ全体に分散させる必要があります。

衛星が自分自身と互いを見張り、有資格の人が証拠を裏づけて重大な対応を決めるとき、群れは、速く、しなやかで、なお説明責任のある免疫を手に入れます。
