# Koki's Technical Paper — Space Cyber Defense Series SCD-002-5

## Sensing the Cosmic Discord — Quantum Key Distribution, Physics-Based Eavesdropping Detection, and Human Governance of Quantum-Safe Keys

### Summary Digest
Quantum key distribution turns the act of eavesdropping into a detectable disturbance, because measuring a quantum signal changes it, and Europe's EAGLE-1 satellite, built by a consortium of more than 20 companies led by SES and slated by ESA for launch in February 2027, is designed to test this approach from orbit.

This paper applies CISSP Domain 3 to explain what satellite QKD can and cannot do, why the NSA and the UK's NCSC still do not recommend it on its own for their most sensitive systems, and why a hybrid of quantum keys and post-quantum cryptography, governed by qualified people, is the most realistic path to quantum-safe space links.

---
### 1. When Listening Leaves a Trace
The Physics Behind Eavesdropping Detection:

* **Measurement Disturbs Quantum States**: In QKD, keys are encoded in single photons or weak laser pulses, and an eavesdropper who measures them introduces errors that the legitimate parties can detect when they compare a sample of their results.
* **Space Extends the Distance**: Optical fibers absorb photons over long distances, so satellites can carry quantum signals between distant ground stations, a capability first demonstrated at scale by China's Micius satellite, launched in 2016, in experiments reported in 2017.
* **Europe Is Moving Toward Operations**: ESA describes EAGLE-1 as an end-to-end system with a satellite, optical ground stations, and key-management networks linked to national quantum communication infrastructure, intended to give governments and critical services operational experience.

### 2. What QKD Cannot Do
Limits Recognized by Security Agencies:

* **QKD Does Not Authenticate the Other Party**: The NSA's guidance, restated in 2026, notes that QKD is only a partial solution because it generates keys but still needs classical authentication to confirm who is on the other end.
* **Trusted Relays and Special Hardware Add Risk**: QKD networks often depend on trusted relay nodes and dedicated equipment, which the NSA warns increases infrastructure cost and insider-threat exposure, and real devices can have implementation flaws that theory does not cover.
* **Disturbance Can Become Denial of Service**: Because any interference raises the error rate, an attacker who cannot steal the key may still stop key exchange by adding noise, so QKD links need fallback key paths.

### 3. A Hybrid, Human-Governed Approach
Combining Quantum Keys, Post-Quantum Cryptography, and Oversight:

* **Layer QKD With Post-Quantum Algorithms**: NIST's FIPS 203, 204, and 205, published in August 2024, provide quantum-resistant key establishment and signatures, and combining them with QKD-derived keys means an attacker must defeat both methods to read protected traffic.
* **AI Monitors Error Rates, People Decide on Keys**: AI can watch quantum bit error rates, link conditions, and key-generation rates across many passes and flag unusual patterns, but suspending a link, discarding keys, or switching to a fallback key source is approved by an accountable key custodian.
* **Proposed Key Governance Rule**: Key-management policies under CISSP Domain 3 define dual control for master keys, documented reasons for every key revocation, and regular audits by people who are independent of daily operations.

### 4. The Quantum-Ready Workforce
New Skills, Inclusive Training, and Long-Term Security:

* **Quantum Security Needs Many Trained People**: Operating quantum links, managing hybrid keys, and auditing their implementations require physicists, engineers, cryptographers, and security operators, and this work cannot be reserved for a few elite laboratories.
* **Transition Deadlines Create Demand for Skills**: The NSA states that new commercial National Security Systems must support quantum-resistant algorithms starting in 2027, so organizations need staff who can plan migrations now rather than relying on vendors or AI tools to do it for them.
* **CISSP Anchors Cryptographic Judgment**: CISSP Domain 3 teaches how to choose, combine, and govern cryptographic controls, giving professionals a stable foundation as the technology shifts from classical to post-quantum and quantum methods.

### 5. Conclusion
Quantum key distribution offers a rare advantage, making eavesdropping detectable by the laws of physics, but it does not authenticate parties, depends on specialized hardware, and can be disrupted by noise.

Space links will be safest when quantum keys and post-quantum cryptography work together, when AI monitors the signals while qualified people govern the keys, and when organizations invest in a broad workforce ready for the quantum era.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-002-5

## 宇宙の不協和音を感知する — 量子鍵配送、物理法則に基づく盗聴の検知、および耐量子の鍵の人による統治

### サマリー・ダイジェスト
量子鍵配送（QKD）は、盗聴という行為を検知できる乱れに変えます。量子の信号は、測定するとその状態が変わるためです。SESが率いる20社以上の企業連合が開発し、ESAが2027年2月の打ち上げを予定している欧州の衛星EAGLE-1は、この方式を軌道上で試すために設計されています。

本論文はCISSPのドメイン3を適用して、衛星QKDにできることとできないこと、米国のNSAと英国のNCSCがなお最も機密性の高いシステムにQKD単独での使用を推奨していない理由を説明します。そして、量子鍵と耐量子暗号を組み合わせ、有資格の人が統治する複合型の方式こそが、耐量子の宇宙リンクへの最も現実的な道であることを示します。

---
### 1. 聞くことが痕跡を残すとき
盗聴の検知を支える物理法則:

* **測定は量子状態を乱す**: QKDでは、鍵は単一光子や弱いレーザーパルスに符号化されます。盗聴者がそれを測定すると誤りが生じ、正規の当事者は結果の一部を照合することでその誤りを検知できます。
* **宇宙が距離を延ばす**: 光ファイバーは長い距離で光子を吸収してしまうため、衛星を使えば離れた地上局の間で量子信号を運べます。この能力は、2016年に打ち上げられた中国の衛星「墨子（Micius）」が、2017年に報告された実験で初めて大規模に実証しました。
* **運用へと進む欧州**: ESAは、EAGLE-1を、衛星、光地上局、各国の量子通信インフラにつながる鍵管理ネットワークからなる一貫したシステムと説明しています。政府や重要なサービスに運用の経験を積ませることを目的としています。

### 2. QKDにできないこと
安全保障機関が認める限界:

* **QKDは相手を認証しない**: NSAが2026年に改めて示した指針は、QKDは鍵を生成するものの、相手が誰かを確かめるには従来型の認証が必要なため、部分的な解決策にすぎないと指摘しています。
* **信頼された中継点と専用機器がリスクを加える**: QKDのネットワークは、信頼された中継ノードと専用の機器に頼ることが多く、NSAはそれがインフラの費用と内部不正のリスクを高めると警告しています。また実際の機器には、理論では扱われない実装上の欠陥があり得ます。
* **乱れがサービス妨害になり得る**: どんな干渉でも誤り率が上がるため、鍵を盗めない攻撃者でも、雑音を加えることで鍵の交換を止められることがあります。そのためQKDのリンクには、代替の鍵の経路が必要です。

### 3. 複合型で人が統治する方式
量子鍵、耐量子暗号、および監督の組み合わせ:

* **QKDに耐量子アルゴリズムを重ねる**: 2024年8月に公表されたNISTのFIPS 203、204、205は、量子計算機に耐える鍵の確立と署名を提供します。これをQKDで得た鍵と組み合わせれば、攻撃者が守られた通信を読むには両方の方式を破らなければなりません。
* **誤り率はAIが見張り、鍵は人が決める**: AIは多くの通過にわたって量子ビット誤り率、リンクの状態、鍵の生成速度を見張り、普段と違うパターンを知らせることができます。しかし、リンクの停止、鍵の破棄、代替の鍵の供給源への切り替えは、説明責任を負う鍵管理者が承認します。
* **鍵の統治の規則（提案）**: CISSPのドメイン3に基づく鍵管理の方針では、マスター鍵の二者による管理、すべての鍵の失効についての理由の記録、日々の運用から独立した人による定期的な監査を定めます。

### 4. 量子時代に備える人材
新しい技能、誰もが学べる訓練、および長期的な安全:

* **量子セキュリティには訓練された多くの人が必要**: 量子リンクの運用、複合型の鍵の管理、その実装の監査には、物理学者、技術者、暗号の専門家、セキュリティの運用者が必要です。この仕事を一握りの精鋭の研究所だけのものにしてはなりません。
* **移行の期限が技能の需要を生む**: NSAは、新しい商用の国家安全保障システムは2027年から耐量子アルゴリズムに対応しなければならないとしています。組織は、ベンダーやAIツールに任せきりにするのではなく、今のうちから移行を計画できる人材を必要としています。
* **CISSPが暗号の判断の土台になる**: CISSPのドメイン3は、暗号による統制をどう選び、組み合わせ、統治するかを教えます。技術が従来型から耐量子、そして量子の方式へと移っていく中でも、専門家に安定した土台を与えます。

### 5. 結論
量子鍵配送は、物理法則によって盗聴を検知できるようにするという、まれな利点を持っています。しかし、相手を認証せず、専用の機器に頼り、雑音によって妨げられることもあります。

宇宙リンクが最も安全になるのは、量子鍵と耐量子暗号が協力して働き、AIが信号を見張る一方で有資格の人が鍵を統治し、組織が量子時代に備えた幅広い人材に投資するときです。
