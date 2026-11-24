# Koki's Technical Paper — Space Cyber Defense Series SCD-006

## The Living Armor — Protecting Orbital AI Compute and Its Power, Thermal, and Firmware Foundations as One System

### Summary Digest
Orbital data centers have moved from concept to hardware: Starcloud launched a satellite carrying an NVIDIA H100 GPU in November 2025 and later trained a small language model in orbit, and Google's first Project Suncatcher prototype, carrying four TPUs and solar panels rated at about one kilowatt, launched on October 1, 2026.

This paper applies CISSP Domains 3 and 7 to orbital AI compute, arguing that processors, power, cooling, and firmware must be defended together as a living armor, because an attack on any one of them can disable the whole, and because no technician can reach the hardware to repair it.

---
### 1. A Data Center No One Can Visit
Why Orbital Compute Changes the Security Model:

* **No Hands-On Repair**: On Earth, a technician can replace a failed server or reflash corrupted firmware, but in orbit every recovery must be done remotely, so resilience must be designed in from the start.
* **Harsh Conditions Hide Attacks**: High-energy particles in space can flip bits in memory and corrupt computations, which means defenders must distinguish natural radiation effects from deliberate tampering.
* **Compute, Power, and Heat Are Linked**: AI processors draw large amounts of power and produce heat that must be radiated away, so an attack on power or thermal control can damage or shut down the computing payload.

### 2. Designing Defense in Layers
Hardware, Firmware, Power, and Workloads:

* **Radiation-Aware Hardware**: Google reported that its Trillium TPUs showed no hard failures from total ionizing dose up to the maximum tested 15 krad(Si), and error-correcting memory and redundancy help separate random upsets from attacks.
* **Resilient Firmware**: Following NIST SP 800-193, platform firmware is protected against unauthorized changes, monitored for corruption, and recoverable from a trusted image without human hands on the hardware.
* **Power and Thermal Guardrails**: Independent controllers enforce limits on power draw and temperature so that no software, including a compromised AI workload, can overheat or starve the platform.

### 3. AI Workloads Under Human Governance
Running AI in Orbit Without Losing Control:

* **The Payload Is Itself an AI System**: Models running in orbit can be targeted by poisoning, evasion, or extraction attacks described in NIST AI 100-2e2025, and their weights are valuable assets that must be protected from theft.
* **Automated Self-Protection Within Limits**: The platform may automatically throttle workloads, isolate a misbehaving process, or switch to a safe mode when it detects danger, actions that can be reversed.
* **Proposed Platform Authority Rule**: Automated systems may protect the platform within preset limits, but loading new firmware, changing power or thermal limits, deploying a new AI model, or restoring a compromised node requires approval by a qualified platform engineer and a security reviewer.

### 4. The People Who Run Data Centers in the Sky
New Careers and Shared Expertise:

* **Orbital Compute Needs Hybrid Skills**: Running AI hardware in orbit requires data center engineers, spacecraft engineers, firmware specialists, and AI security professionals, a combination that creates new careers rather than eliminating them.
* **Experience From Earth Still Matters**: Skills from terrestrial data center operations, such as capacity planning, incident response, and change control, transfer to orbit, so experienced staff should be retrained and valued rather than replaced.
* **CISSP Unifies Physical and Logical Security**: CISSP Domain 3 covers secure architecture and physical controls and Domain 7 covers operations, giving teams a common framework for defending systems where hardware and software are inseparable.

### 5. Conclusion
Orbital data centers combine processors, power, cooling, and firmware in a place no technician can reach, so their defense must treat these parts as one living armor rather than separate components.

Radiation-aware hardware, resilient firmware, independent power and thermal guardrails, protected AI workloads, and qualified people who approve every change allow AI computing in orbit to grow safely.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-006

## 生きた鎧 — 軌道上のAI計算基盤と、その電力・熱・ファームウェアの土台を1つのシステムとして守る

### サマリー・ダイジェスト
軌道上のデータセンターは、構想から実際の機器へと進みました。Starcloud社は2025年11月にNVIDIAのH100 GPUを積んだ衛星を打ち上げ、のちに軌道上で小さな言語モデルを学習させました。またGoogleのProject Suncatcherの最初の試作機は、4つのTPUと約1キロワットの太陽電池パネルを載せて、2026年10月1日に打ち上げられました。

本論文はCISSPのドメイン3と7を軌道上のAI計算に適用します。プロセッサー、電力、冷却、ファームウェアは「生きた鎧」として一緒に守らなければならないと論じます。そのどれか1つへの攻撃が全体を止め得るうえ、修理のために機器に手が届く技術者はいないからです。

---
### 1. 誰も訪れられないデータセンター
軌道上の計算がセキュリティのモデルを変える理由:

* **手で修理できない**: 地上なら技術者が壊れたサーバーを交換したり、壊れたファームウェアを書き直したりできますが、軌道上ではすべての復旧を遠隔で行わなければなりません。そのため回復力は、最初から設計に組み込む必要があります。
* **厳しい環境が攻撃を隠す**: 宇宙の高エネルギー粒子は、メモリーのビットを反転させ、計算を壊すことがあります。防御側は、自然の放射線の影響と、意図的な改ざんを見分けなければなりません。
* **計算、電力、熱はつながっている**: AIプロセッサーは大きな電力を使い、宇宙へ逃がさなければならない熱を出します。そのため、電力や温度の制御への攻撃は、計算のためのペイロードを壊したり止めたりし得ます。

### 2. 層を重ねて防御を設計する
ハードウェア、ファームウェア、電力、および処理:

* **放射線を考えたハードウェア**: Googleは、同社のTrillium TPUが、試験した最大の15 krad(Si)までの総電離線量で、致命的な故障を示さなかったと報告しています。誤り訂正機能付きのメモリーと冗長化は、偶然の誤動作と攻撃を区別する助けになります。
* **回復力のあるファームウェア**: NIST SP 800-193に沿って、基盤のファームウェアを無許可の変更から守り、破損を監視し、機器に人の手を触れずに信頼できるイメージから復旧できるようにします。
* **電力と温度の安全柵**: 独立した制御装置が電力の使用量と温度の上限を守ります。乗っ取られたAIの処理を含め、どんなソフトウェアも基盤を過熱させたり電力不足にしたりできないようにするためです。

### 3. 人の統治のもとでのAIの処理
制御を失わずに軌道上でAIを動かす:

* **ペイロードそのものがAIシステム**: 軌道上で動くモデルは、NIST AI 100-2e2025が示す汚染、回避、抽出の攻撃の標的になり得ます。その重み（モデルの中身）は、盗まれないよう守るべき価値ある資産です。
* **範囲を限った自動の自己防衛**: 基盤は危険を検知したとき、処理を自動で絞ったり、異常な処理を隔離したり、セーフモードに切り替えたりしてかまいません。いずれも元に戻せる措置です。
* **基盤の権限の規則（提案）**: 自動のシステムは、あらかじめ決めた範囲内で基盤を守ってかまいません。しかし、新しいファームウェアの読み込み、電力や温度の上限の変更、新しいAIモデルの展開、侵害されたノードの復旧には、有資格の基盤技術者とセキュリティの確認者の承認を必須とします。

### 4. 空のデータセンターを動かす人々
新しい仕事と共有される専門性:

* **軌道上の計算には複合的な技能が必要**: 軌道上でAIの機器を動かすには、データセンターの技術者、宇宙機の技術者、ファームウェアの専門家、AIセキュリティの専門家が必要です。この組み合わせは、仕事をなくすのではなく、新しい仕事を生みます。
* **地上での経験は今も大切**: 容量の計画、インシデント対応、変更管理など、地上のデータセンター運用で培った技能は軌道上でも生きます。そのため、経験のある人員は置き換えるのではなく、学び直しを通じて大切にすべきです。
* **CISSPが物理と論理のセキュリティをまとめる**: CISSPのドメイン3は安全なアーキテクチャと物理的な統制を、ドメイン7は運用を扱います。それにより、ハードウェアとソフトウェアが切り離せないシステムを守るための共通の枠組みが得られます。

### 5. 結論
軌道上のデータセンターは、技術者の手が届かない場所で、プロセッサー、電力、冷却、ファームウェアを組み合わせています。そのため、その防御は、これらを別々の部品ではなく1つの「生きた鎧」として扱わなければなりません。

放射線を考えたハードウェア、回復力のあるファームウェア、独立した電力と温度の安全柵、守られたAIの処理、そしてあらゆる変更を承認する有資格の人々がそろって、軌道上のAI計算を安全に育てることができます。
