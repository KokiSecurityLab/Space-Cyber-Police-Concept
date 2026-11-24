# Koki's Technical Paper — Space Cyber Defense Series SCD-002-2

## Detecting the Digital Fingerprint — Physical-Layer Authentication, Its Limits, and Human Review Before Rejecting a Trusted Source

### Summary Digest
Every transmitter has tiny hardware imperfections that leave a measurable signature in its signal, and researchers at the University of Oxford showed in their SatIQ work, presented at ACM CCS 2023, that a neural network trained on 1,705,202 Iridium messages could use these signatures to help authenticate satellite downlinks and resist replay attacks.

This paper applies CISSP Domains 4 and 5 to explain how physical-layer fingerprinting adds a second factor of identity to space links, where it fails, and why a person should review the evidence before a ground system rejects a satellite it has trusted for years.

---
### 1. Identity Below the Data
Why Cryptography Alone Is Not Always Available:

* **Many Satellites Cannot Be Patched**: Legacy spacecraft often have no cryptographic authentication and cannot be upgraded in orbit, so a ground station may have no reliable way to tell a real downlink from a spoofed or replayed one.
* **Hardware Leaves a Fingerprint**: Small manufacturing differences in oscillators, amplifiers, and modulators create impairments in the signal, and high-sample-rate measurements can turn these into an identifying signature that is difficult to forge without similar high-end transmitting hardware.
* **Optical Terminals Have Signatures Too**: Laser transmitters show characteristic pulse shapes, timing behavior, and power profiles, so the same principle can extend to optical links as research matures, adding a check that does not depend on any secret key.

### 2. Where Fingerprinting Works and Where It Fails
Evidence, Limits, and Layered Use:

* **Evidence of Value**: In the CCS 2023 study, the SatIQ system was tested against messages replayed with a software-defined radio and achieved an equal error rate of 0.120, and the researchers reported that the model remained stable over time and could enroll new transmitters without retraining.
* **Noise Is the Main Limitation**: Atmospheric noise and multipath scattering blur the signature, and a 2024 follow-up study from the same research area warned that an attacker can cause denial of service simply by disrupting the fingerprint so that legitimate messages are rejected.
* **A Second Factor, Not a Replacement**: Fingerprinting works best as one signal among several, combined with frame authentication such as CCSDS Space Data Link Security wherever it is available and with orbital tracking data that confirms where the satellite actually is.

### 3. Human Review Before Rejection
Securing the Model and Deciding Who Is Trusted:

* **The Fingerprint Model Is an AI Asset to Protect**: If an attacker could poison the enrollment data, a forged transmitter could be accepted as genuine, so training sets, model files, and enrollment changes are controlled and logged under CISSP Domain 8, following the attack categories in NIST AI 100-2e2025.
* **False Rejections Have a Cost**: Blocking a genuine satellite because noise distorted its signature can interrupt weather data, navigation, or emergency communications, so a mismatch triggers investigation rather than immediate permanent rejection.
* **Proposed Trust-Decision Rule**: The AI may quarantine suspicious traffic for review, but removing a long-trusted transmitter from the allow list, or enrolling a new one, requires approval by a qualified analyst who compares the fingerprint with tracking, timing, and operator records.

### 4. The People Who Read the Signals
Signal Analysts, Identity Engineers, and Shared Skills:

* **Signal Intelligence Skills Are Scarce and Valuable**: Interpreting physical-layer evidence requires knowledge of radio and optical engineering, statistics, and security, and the ISC2 2024 Cybersecurity Workforce Study estimated a global gap of 4.8 million security professionals.
* **Investing in Many Analysts Protects Everyone**: Filling that gap requires training many capable people from engineering, operations, and academic backgrounds, not concentrating expertise in a few highly paid specialists or in automated tools that no one fully understands.
* **CISSP Domain 5 Applies to Machines**: Identity and access management covers how satellites and ground stations are identified and trusted, and CISSP-qualified professionals can design enrollment, revocation, and review processes that treat a transmitter's identity with the same care as a user's.

### 5. Conclusion
A transmitter's physical fingerprint gives defenders a second witness to identity, especially for legacy satellites that cannot use modern cryptography, but noise and deliberate disruption mean that it must be combined with other evidence.

By protecting the fingerprint models as AI assets and keeping trust decisions with qualified people, defenders can catch impostors without cutting off the genuine systems that people depend on.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-002-2

## デジタル指紋の検知 — 物理層の認証、その限界、および信頼してきた送信源を拒否する前の人による確認

### サマリー・ダイジェスト
どの送信機にも、信号の中に測定可能な特徴を残すわずかなハードウェアの不完全さがあります。オックスフォード大学の研究者は、ACM CCS 2023で発表したSatIQの研究で、1,705,202件のイリジウムのメッセージで学習させたニューラルネットワークが、この特徴を使って衛星のダウンリンクの認証を助け、再送攻撃に耐えられることを示しました。

本論文はCISSPのドメイン4と5を適用して、物理層の指紋が宇宙リンクにどのように2つ目の本人確認の要素を加えるのか、どこで失敗するのか、そして地上システムが長年信頼してきた衛星を拒否する前に、なぜ人が証拠を確認すべきなのかを説明します。

---
### 1. データの下にある本人性
暗号が常に使えるとは限らない理由:

* **多くの衛星はパッチを当てられない**: 古い宇宙機には暗号による認証がないことが多く、軌道上で更新することもできません。そのため地上局には、本物のダウンリンクと、偽装や再送されたものとを見分ける確かな方法がないことがあります。
* **ハードウェアは指紋を残す**: 発振器、増幅器、変調器の製造上の小さな違いが信号にゆがみを生みます。高いサンプリングレートで測定すると、これを識別用の特徴に変えることができ、同等の高性能な送信機器がなければ偽造は困難です。
* **光端末にも特徴がある**: レーザー送信機には、特有のパルスの形、タイミングのふるまい、出力の特性があります。研究が進めば同じ原理を光リンクにも広げられ、秘密鍵に依存しない確認を加えられます。

### 2. 指紋が有効な場面と失敗する場面
証拠、限界、および多層での活用:

* **有効性の証拠**: CCS 2023の研究では、SatIQはソフトウェア無線で再送されたメッセージに対して試験され、等誤り率0.120を達成しました。研究者は、モデルが時間がたっても安定しており、再学習なしで新しい送信機を登録できたと報告しています。
* **主な限界は雑音**: 大気の雑音や多重経路の散乱は特徴をぼかします。また、同じ研究分野の2024年の追加研究は、攻撃者が指紋を乱すだけで正規のメッセージが拒否され、サービス妨害を起こせると警告しました。
* **置き換えではなく2つ目の要素**: 指紋は、いくつかある信号の1つとして使うときに最も効果を発揮します。CCSDSのSpace Data Link Securityのようなフレーム認証が使える場合はそれと組み合わせ、衛星が実際にどこにいるかを確かめる軌道追跡データとも組み合わせます。

### 3. 拒否する前の人による確認
モデルの保護と、誰を信頼するかの判断:

* **指紋モデルは守るべきAI資産**: 攻撃者が登録データを汚染できれば、偽の送信機が本物として受け入れられてしまいます。そのため、学習データ、モデルファイル、登録の変更は、NIST AI 100-2e2025の攻撃分類に沿い、CISSPのドメイン8のもとで管理し、記録します。
* **誤った拒否には代償がある**: 雑音で特徴がゆがんだために本物の衛星を遮断すると、気象データ、測位、緊急通信が途切れかねません。そのため不一致は、即座の恒久的な拒否ではなく、調査のきっかけとします。
* **信頼判断の規則（提案）**: AIは疑わしい通信を確認のために隔離してかまいません。しかし、長く信頼してきた送信機を許可リストから外すことや、新しい送信機を登録することには、指紋を追跡、タイミング、運用者の記録と照らし合わせる有資格の分析担当者の承認を必須とします。

### 4. 信号を読み解く人々
信号分析担当者、ID技術者、および共有される技能:

* **信号情報の技能は希少で価値が高い**: 物理層の証拠を読み解くには、電波と光の工学、統計、セキュリティの知識が必要です。ISC2の2024年版サイバーセキュリティ人材調査は、世界で480万人のセキュリティ専門家が不足していると推計しました。
* **多くの分析担当者への投資が皆を守る**: この不足を埋めるには、工学、運用、学術などさまざまな背景を持つ多くの有能な人を育てる必要があります。専門知識を、高給の少数の専門家や、誰も十分に理解していない自動化ツールに集中させるべきではありません。
* **CISSPのドメイン5は機械にも当てはまる**: IDとアクセスの管理は、衛星や地上局をどう識別し、信頼するかにも及びます。CISSP資格を持つ専門家は、送信機の本人性を利用者の本人性と同じ慎重さで扱う登録、失効、確認の手順を設計できます。

### 5. 結論
送信機の物理的な指紋は、とくに最新の暗号を使えない古い衛星について、防御側に本人性の2人目の証人を与えます。しかし雑音や意図的な妨害があるため、ほかの証拠と組み合わせなければなりません。

指紋モデルをAI資産として守り、信頼の判断を有資格の人に委ねることで、防御側は、人々が頼っている本物のシステムを断ち切ることなく、なりすましを見抜くことができます。
