# Koki's Technical Paper — Space Cyber Defense Series SCD-014

## Celestial Authentication — Combining Cryptography With Physical Evidence to Verify Spacecraft

### Summary Digest
Cryptographic keys are the foundation of authentication, but a stolen key lets an attacker look exactly like a legitimate user. A U.S. review board reported in April 2024 that a stolen signing key, combined with a validation flaw, allowed a state-linked group to access more than 500 mailboxes at 22 organizations, and the company involved still could not explain how the key was stolen. In space, physical evidence such as signal characteristics, timing, position, and the view of the stars can add independent proof that is far harder to steal.

This main paper of SCD-014 introduces celestial authentication, which combines cryptography with physical evidence to verify spacecraft and ground stations. It applies CISSP Domains 3, 4, and 5, and shows why people must decide what happens when cryptographic and physical evidence disagree.

---
### 1. Why One Proof Is Not Enough
The Limits of Digital Credentials Alone:

* **Stolen Keys Look Legitimate**: An attacker who holds a valid key can create messages that pass every cryptographic check, so a single factor cannot reveal the theft.
* **Compromised Ground Systems Speak the Right Language**: The SPARTA framework describes how attackers can use a compromised mission ground system to send legitimate-looking commands that blend with routine operations.
* **Physics Is Hard to Steal**: Signal fingerprints, propagation delay, Doppler shift, and the star field seen by a spacecraft depend on real hardware and geometry, which an attacker cannot copy as easily as a file.

### 2. Five Layers of Celestial Authentication
A Structure for the SCD-014 Series:

* **Understand Credential Weakness**: SCD-014-1 examines how keys are stolen and why single-factor trust fails.
* **Combine Factors and Protect Sensors**: SCD-014-2 combines cryptography with position and time, and SCD-014-3 explains how to protect star trackers that give spacecraft their sense of direction.
* **Verify Continuously and Anchor to Reality**: SCD-014-4 describes continuous verification throughout a session, and SCD-014-5 explains how ranging and signal measurements confirm where a transmitter really is.

### 3. AI-Assisted Authentication Under Human Authority
Combining Evidence, Deciding Carefully:

* **AI Learns Physical Fingerprints**: Research on satellite radio fingerprinting has shown that machine learning can identify transmitters from tiny hardware imperfections in their signals, adding a factor that does not depend on keys.
* **Physical Models Can Also Be Fooled**: Attackers may try to imitate fingerprints or feed false sensor data, consistent with the evasion risks in NIST AI 100-2e2025, so no single physical factor is trusted alone.
* **Proposed Authentication Conflict Rule**: Automated systems may reject commands that fail cryptographic checks and flag commands whose physical evidence is inconsistent, but accepting a command despite conflicting evidence, revoking a spacecraft's keys, or declaring a ground station compromised is decided by qualified operators.

### 4. People Who Weigh the Evidence
Judgment Where Digital and Physical Meet:

* **Interpreting Physical Evidence Takes Expertise**: Signal engineers and flight dynamics specialists know when a difference in Doppler or timing is natural and when it is suspicious.
* **Key Management Remains Human Work**: The 2024 review noted that key rotation had been paused at the affected company, showing how human governance decisions determine whether keys stay safe.
* **CISSP Provides the Framework**: CISSP Domain 3 covers cryptography and key management, Domain 4 covers secure communications, and Domain 5 covers identity, authentication, and multifactor approaches.

### 5. Conclusion
Cryptography proves that a message was signed with the right key, but not that the key is in the right hands, and physical evidence can fill that gap.

By combining strong cryptography with signal fingerprints, timing, position, and sensor integrity, using AI to compare evidence quickly, and keeping trained people responsible for difficult decisions, the space community can build authentication grounded in both mathematics and the physical universe.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-014

## 天空の認証 — 暗号と物理的な証拠を組み合わせて宇宙機を確かめる

### サマリー・ダイジェスト
暗号の鍵は認証の土台ですが、鍵を盗まれると、攻撃者は正当な利用者とまったく同じに見えてしまいます。米国のある審査委員会は2024年4月、盗まれた署名の鍵と確認の仕組みの欠陥が組み合わさり、国家とつながりのある集団が22の組織の500を超えるメールボックスにアクセスできたと報告しました。関係した企業は、鍵がどのように盗まれたのかを、なお説明できていませんでした。宇宙では、信号の特徴、時刻、位置、星の見え方といった物理的な証拠が、盗むのがずっと難しい、独立した証明を加えられます。

SCD-014の本編である本論文は、暗号と物理的な証拠を組み合わせて宇宙機と地上局を確かめる「天空の認証」を紹介します。CISSPのドメイン3、4、5を適用し、暗号の証拠と物理的な証拠が食い違うときにどうするかは、人が決めなければならない理由を示します。

---
### 1. ひとつの証明では足りない理由
デジタルの認証情報だけの限界:

* **盗まれた鍵は正当に見える**: 正しい鍵を持つ攻撃者は、暗号のどの確認にも合格するメッセージを作れます。そのため、ひとつの要素だけでは、盗まれたことは見抜けません。
* **乗っ取られた地上システムは正しい言葉を話す**: SPARTAの枠組みは、攻撃者が乗っ取ったミッションの地上システムを使い、いつもの運用に紛れ込む、正当に見える指令を送れることを説明しています。
* **物理は盗みにくい**: 信号の指紋、電波の届く時間の遅れ、ドップラー効果、宇宙機から見える星の並びは、本物のハードウェアと位置関係で決まるため、攻撃者がファイルのように簡単にまねすることはできません。

### 2. 天空の認証の5つの層
SCD-014シリーズの構成:

* **認証情報の弱さを理解する**: SCD-014-1は、鍵がどのように盗まれ、なぜひとつの要素への信頼が失敗するのかを調べます。
* **要素を組み合わせ、センサーを守る**: SCD-014-2は暗号と位置と時刻を組み合わせ、SCD-014-3は宇宙機に向きの感覚を与えるスタートラッカーをどう守るかを説明します。
* **絶えず確かめ、現実に錨を下ろす**: SCD-014-4は通信の間ずっと続ける確認を、SCD-014-5は測距と信号の測定で、送信元が本当にどこにいるかを確かめる方法を説明します。

### 3. 人の権限の下での、AIによる認証の支援
証拠を組み合わせ、慎重に決める:

* **AIが物理的な指紋を学ぶ**: 衛星の電波の指紋についての研究は、機械学習が、信号に表れるハードウェアのごく小さな不完全さから送信機を見分けられることを示しており、鍵に頼らない要素を加えられます。
* **物理のモデルもだまされることがある**: 攻撃者は指紋をまねたり、偽のセンサーのデータを流し込んだりしようとするかもしれません。これはNIST AI 100-2e2025が述べる回避のリスクと同じ趣旨です。そのため、物理的な要素をひとつだけで信頼することはしません。
* **認証の食い違いの規則（提案）**: 自動のシステムは、暗号の確認に失敗した指令をはねのけ、物理的な証拠が合わない指令に印を付けてかまいません。しかし、証拠が食い違うのに指令を受け入れること、宇宙機の鍵を無効にすること、地上局が乗っ取られたと宣言することは、有資格の運用担当者が決めます。

### 4. 証拠を比べてはかる人々
デジタルと物理が出会うところでの判断:

* **物理的な証拠を読み解くには専門性が要る**: 信号の技術者と軌道力学の専門家は、ドップラーや時刻の違いが自然なものか、疑わしいものかを知っています。
* **鍵の管理は人の仕事であり続ける**: 2024年の審査は、関係した企業で鍵の交換が止められていたことを指摘しており、鍵が安全なままかどうかは、人のガバナンスの判断で決まることを示しています。
* **CISSPが枠組みを与える**: CISSPのドメイン3は暗号と鍵の管理を、ドメイン4は安全な通信を、ドメイン5はID、認証、多要素の考え方を扱います。

### 5. 結論
暗号は、メッセージが正しい鍵で署名されたことは証明しますが、その鍵が正しい人の手の中にあることまでは証明しません。物理的な証拠は、そのすき間を埋められます。

強い暗号を、信号の指紋、時刻、位置、センサーの完全性と組み合わせ、証拠を素早く比べるためにAIを使い、難しい判断の責任を訓練を受けた人が持ち続けることで、宇宙の世界は、数学と物理的な宇宙の両方に根ざした認証を築けます。
