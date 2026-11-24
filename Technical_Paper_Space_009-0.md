# Koki's Technical Paper — Space Cyber Defense Series SCD-009

## The Sovereign Shield — Defending Space Systems Against State-Sponsored Intrusion, Espionage, and Hijacking

### Summary Digest
Nation-state actors already target space and communications infrastructure: on May 10, 2022, the United States, the United Kingdom, and the European Union formally attributed the February 2022 cyberattack on Viasat's KA-SAT network to Russia, and in August 2025 the FBI and allied agencies warned that the Salt Typhoon campaign had targeted about 200 companies in 80 countries.

This paper applies CISSP Domains 1 and 7 to state-sponsored threats against space systems, describing how well-resourced adversaries operate, how operators can make hijacking and espionage harder, and why decisions in a state-level crisis must rest with accountable people working with governments and partners.

---
### 1. What Makes State Actors Different
Resources, Patience, and Strategic Goals:

* **Attacks Timed to Geopolitical Events**: The KA-SAT attack occurred about one hour before the invasion of Ukraine began, showing that state actors may use cyber operations to support military or political objectives.
* **Long, Quiet Access Is the Goal**: Salt Typhoon compromised telecommunications providers in many countries for espionage, and U.S. officials said the campaign had likely been underway for one to two years before it was discovered.
* **Known Weaknesses Are Often Enough**: Allied agencies reported that Salt Typhoon exploited known vulnerabilities in widely used network devices rather than zero-day flaws, showing that basic patching remains a frontline defense even against nation-states.

### 2. Building the Sovereign Shield
Hardening Against Patient, Capable Adversaries:

* **Patch and Harden the Edge**: Routers, VPN gateways, and management interfaces at ground stations are kept current and monitored, because these devices are common entry points for state actors.
* **Separate Management From Service Networks**: The KA-SAT incident began in the network management segment, so management systems that can command terminals or satellites are isolated and protected with strong authentication.
* **Watch for Proximity and Signals Intelligence**: Russia's Luch (Olymp-K) satellite has repeatedly moved close to commercial satellites in geostationary orbit, coming within about 4 kilometers of Intelsat 37e in October 2022, so operators encrypt links and monitor nearby objects for possible eavesdropping.

### 3. AI Under Human Command in a State-Level Crisis
Speed, Caution, and Accountability:

* **AI Can Detect Stealthy Campaigns**: Models that analyze network and command data across long periods can reveal the slow, quiet patterns typical of state-sponsored intrusions.
* **State Actors Also Use AI**: Anthropic reported in November 2025 that a state-sponsored group used AI agents to perform most of an intrusion campaign, and adversaries may try to poison or evade defensive models as NIST AI 100-2e2025 describes.
* **Proposed Crisis Authority Rule**: AI may detect and contain suspicious activity within preset limits, but attributing an attack to a state, shutting down service to a region during a conflict, or coordinating with government agencies requires decisions by accountable leaders and qualified incident responders.

### 4. Defenders Who Serve the Public Interest
Skilled People, Trusted Partnerships, and Shared Duty:

* **State-Level Defense Requires Experienced Teams**: Recognizing and evicting a patient adversary takes analysts, threat hunters, and incident responders with deep experience, and organizations should invest in them rather than rely on automation alone.
* **Partnerships Multiply Strength**: Information sharing among operators, governments, and groups such as Space ISAC helps smaller organizations defend against adversaries far larger than themselves.
* **CISSP Supports Governance and Response**: CISSP Domain 1 covers legal and regulatory considerations, and Domain 7 covers investigations and incident response, preparing professionals for incidents with national consequences.

### 5. Conclusion
State-sponsored actors bring patience, resources, and strategic aims to attacks on space systems, but they often succeed through known weaknesses and poorly separated networks.

Patched and hardened edges, isolated management networks, encrypted links, monitoring of nearby objects, AI that reveals quiet campaigns, and accountable leaders who decide in a crisis together form a sovereign shield that protects both operators and the public.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-009

## 主権の盾 — 国家が支援する侵入、諜報、乗っ取りから宇宙システムを守る

### サマリー・ダイジェスト
国家を背景とする攻撃者は、すでに宇宙と通信のインフラを狙っています。2022年5月10日、米国、英国、欧州連合は、2022年2月のViasatのKA-SAT網へのサイバー攻撃をロシアによるものと正式に断定しました。また2025年8月には、FBIと同盟国の機関が、「Salt Typhoon」の攻撃活動が80か国の約200社を標的にしていたと警告しました。

本論文はCISSPのドメイン1と7を、国家が支援する宇宙システムへの脅威に適用します。資源の豊富な攻撃者がどのように動くか、運用者が乗っ取りや諜報をどう難しくできるかを説明し、国家規模の危機での判断は、政府や協力先と連携する説明責任のある人々が担うべき理由を示します。

---
### 1. 国家を背景とする攻撃者が違う点
資源、忍耐、そして戦略的な目的:

* **地政学的な出来事に合わせた攻撃**: KA-SATへの攻撃は、ウクライナ侵攻が始まる約1時間前に起きました。国家を背景とする攻撃者が、軍事的・政治的な目的を支えるためにサイバー作戦を使うことがあると示しています。
* **長く静かな侵入こそが目的**: Salt Typhoonは、諜報のために多くの国の通信事業者を侵害しました。米国の当局者は、この活動が発見されるまでに1〜2年続いていた可能性が高いと述べています。
* **既知の弱点で足りることが多い**: 同盟国の機関は、Salt Typhoonが未知の脆弱性ではなく、広く使われるネットワーク機器の既知の脆弱性を突いていたと報告しました。国家を相手にしても、基本的なパッチの適用が最前線の防御であり続けることを示しています。

### 2. 主権の盾を築く
忍耐強く有能な攻撃者に備えて守りを固める:

* **境界にパッチを当て、強化する**: 地上局のルーター、VPNのゲートウェイ、管理用の窓口は、国家を背景とする攻撃者のよくある入り口です。そのため、これらの機器は最新に保ち、監視します。
* **管理のネットワークをサービスのネットワークから分ける**: KA-SATの事案はネットワーク管理の区画から始まりました。そのため、端末や衛星に指令を出せる管理のシステムは、隔離し、強い認証で守ります。
* **接近と信号の傍受に目を光らせる**: ロシアの衛星「Luch（Olymp-K）」は、静止軌道で商用の衛星に繰り返し近づき、2022年10月にはIntelsat 37eから約4キロメートルまで接近しました。そのため運用者は、回線を暗号化し、近くの物体を傍受の可能性という観点から監視します。

### 3. 国家規模の危機での、人の指揮のもとのAI
速さ、慎重さ、および説明責任:

* **AIはひそかな攻撃活動を見つけられる**: 長い期間にわたるネットワークと指令のデータを分析するモデルは、国家が支援する侵入に典型的な、ゆっくりした静かなパターンを明らかにできます。
* **国家を背景とする攻撃者もAIを使う**: Anthropicは2025年11月、国家が支援する集団がAIエージェントを使って侵入活動の大半を行ったと報告しました。また攻撃者は、NIST AI 100-2e2025が示すように、防御側のモデルを汚染したり回避したりしようとするかもしれません。
* **危機時の権限の規則（提案）**: AIは、あらかじめ決めた範囲内で、疑わしい活動を検知し封じ込めてかまいません。しかし、攻撃を国家によるものと断定すること、紛争中にある地域へのサービスを止めること、政府機関と連携することは、説明責任を負う責任者と有資格のインシデント対応者が決めます。

### 4. 公共の利益に仕える防御者
熟練した人々、信頼できる協力関係、そして共有の務め:

* **国家規模の防御には経験豊富なチームが要る**: 忍耐強い攻撃者を見抜き、追い出すには、深い経験を持つ分析担当者、脅威ハンター、インシデント対応者が必要です。組織は、自動化だけに頼るのではなく、こうした人々に投資すべきです。
* **協力が力を何倍にもする**: 運用者、政府、Space ISACのような団体の間での情報共有は、小さな組織が、自らよりはるかに大きな攻撃者から身を守る助けになります。
* **CISSPがガバナンスと対応を支える**: CISSPのドメイン1は法と規制の考慮を、ドメイン7は調査とインシデント対応を扱い、国家的な影響を持つインシデントに専門家が備える助けになります。

### 5. 結論
国家を背景とする攻撃者は、忍耐、資源、戦略的な目的を持って宇宙システムを攻撃しますが、多くの場合、既知の弱点と十分に分けられていないネットワークを通じて成功しています。

パッチを当てて強化した境界、隔離された管理のネットワーク、暗号化された回線、近くの物体の監視、静かな攻撃活動を明らかにするAI、そして危機の中で判断する説明責任のある責任者がそろって、運用者と人々の両方を守る主権の盾となります。
