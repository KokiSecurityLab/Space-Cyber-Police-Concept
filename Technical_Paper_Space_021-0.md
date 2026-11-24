# Koki's Technical Paper — Space Cyber Defense Series SCD-021

## Geopolitical Neutrality — Tamper-Evident Records and Shared Registries for a Trusted Space Commons

### Summary Digest
When tensions rise between countries, the facts about what happened in space and cyberspace become contested. Records that anyone can verify, and that no single party can secretly change, help people agree on what is true. The internet already relies on such records: Certificate Transparency logs record billions of web certificates every year, and the Sigstore project's transparency log, whose redesigned version became generally available in October 2025, records software signatures so that a signature cannot be produced and then hidden. In space, the United Nations has maintained a Register of Objects Launched into Outer Space since 1962, and approximately 88% of satellites and other spacecraft launched into Earth orbit or beyond have been registered.

This main paper of SCD-021 introduces tamper-evident records and shared registries as foundations for trust across borders. It applies CISSP Domains 1, 3, and 7, explains how transparency logs, host-based detection, registries, shared data, and evidence standards work together, and shows why people must govern these records fairly.

---
### 1. Why Neutral Records Matter
Shared Facts Reduce Conflict:

* **Disputed Facts Fuel Tension**: When an incident occurs, parties may tell different stories, and without verifiable records it becomes difficult to separate accidents from deliberate acts.
* **Tamper-Evident Records Build Trust**: Append-only logs that anyone can check make it very hard to rewrite history quietly, giving all parties the same evidence.
* **Claims Need Verification**: A 2026 analysis of cyber activity during an armed conflict noted that some claimed attacks on satellite networks could not be confirmed, showing why independent evidence matters.

### 2. Five Foundations of a Trusted Space Commons
A Structure for the SCD-021 Series:

* **Record and Detect**: SCD-021-1 describes append-only transparency logs, and SCD-021-2 describes host-based detection on ground nodes that produces trustworthy evidence.
* **Register and Share**: SCD-021-3 explains registries of space objects, and SCD-021-4 describes a neutral commons for space situational awareness data.
* **Judge Fairly**: SCD-021-5 explains evidence standards for attributing cyber incidents responsibly.

### 3. AI and Neutral Records Under Human Governance
Automation That Serves Everyone Equally:

* **AI Helps Monitor Logs and Registries**: AI can watch transparency logs for unexpected entries, compare registries with tracking data, and highlight inconsistencies for review.
* **AI Can Be Biased or Manipulated**: Models trained on incomplete or one-sided data may favor some actors, and adversaries may try to poison shared datasets, consistent with NIST AI 100-2e2025.
* **Proposed Neutral Record Rule**: AI may detect anomalies and prepare evidence summaries, but decisions to publish findings about other organizations or states, to correct registry entries, or to exclude participants from shared data are made by qualified people under transparent rules.

### 4. Professionals Who Serve the Commons
Fairness as a Professional Value:

* **Neutral Stewards Earn Trust**: People who maintain shared records must act consistently for all participants, regardless of nationality or commercial interest.
* **International Cooperation Needs Experts**: Building and governing shared registries requires engineers, lawyers, diplomats, and security professionals from many countries working together.
* **CISSP Supports Trustworthy Records**: CISSP Domain 1 covers ethics and international legal considerations, Domain 3 covers cryptographic integrity, and Domain 7 covers evidence handling and logging.

### 5. Conclusion
In a world of competing narratives, tamper-evident records and shared registries give everyone a common basis for understanding what happened in space and cyberspace.

By combining transparency logs, trustworthy detection on ground systems, international registries, neutral shared data, careful evidence standards, AI that helps monitor without taking sides, and fair-minded professionals, the space community can build a commons where trust is based on facts that anyone can verify.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-021

## 地政学的な中立 — 信頼できる宇宙の共有地のための、改ざんが見える記録と共有の登録簿

### サマリー・ダイジェスト
国と国の間の緊張が高まると、宇宙とサイバー空間で何が起きたかという事実そのものが争われるようになります。誰でも確かめられ、どの当事者もひそかに変えることができない記録は、人々が何が本当かについて合意する助けになります。インターネットはすでにこうした記録に頼っています。証明書の透明性（CT）のログは毎年何十億ものウェブの証明書を記録し、Sigstoreという取り組みの透明性ログ（作り直した版は2025年10月に一般公開）は、ソフトウェアの署名を記録して、署名を作ってから隠すことができないようにしています。宇宙では、国連が1962年から「宇宙空間に打ち上げられた物体の登録簿」を保っており、地球の軌道やその先に打ち上げられた衛星などの約88%が登録されています。

SCD-021の本編である本論文は、国境を越えた信頼の土台としての、改ざんが見える記録と共有の登録簿を紹介します。CISSPのドメイン1、3、7を適用し、透明性ログ、ホスト型の検知、登録簿、共有のデータ、証拠の基準がどう組み合わさるかを説明し、これらの記録を人が公平に治めなければならない理由を示します。

---
### 1. 中立な記録が大切な理由
共有の事実が争いを減らす:

* **争われる事実は緊張をあおる**: インシデントが起きると、当事者どうしが違う話をすることがあり、確かめられる記録がなければ、事故と意図的な行為を分けるのは難しくなります。
* **改ざんが見える記録が信頼を築く**: 誰でも確かめられる追記専用のログは、歴史をひそかに書き換えることをとても難しくし、すべての当事者に同じ証拠を与えます。
* **主張には確認が要る**: 武力紛争の間のサイバー活動についての2026年の分析は、衛星のネットワークへの攻撃だと主張されたものの一部が確認できなかったと指摘しており、独立した証拠が大切な理由を示しています。

### 2. 信頼できる宇宙の共有地の5つの土台
SCD-021シリーズの構成:

* **記録し、見つける**: SCD-021-1は追記専用の透明性ログを、SCD-021-2は信頼できる証拠を生む地上のノードでのホスト型の検知を説明します。
* **登録し、分け合う**: SCD-021-3は宇宙物体の登録簿を、SCD-021-4は宇宙の状況把握のデータのための中立な共有地を説明します。
* **公平に判断する**: SCD-021-5は、サイバーのインシデントの帰属を責任をもって判断するための証拠の基準を説明します。

### 3. 人のガバナンスの下での、AIと中立な記録
みんなに等しく役立つ自動化:

* **AIがログと登録簿の見張りを助ける**: AIは、透明性ログに予想外の記録がないか見張り、登録簿を追跡のデータと比べ、確認のために食い違いを浮かび上がらせられます。
* **AIは偏ったり操作されたりすることがある**: 不完全な、あるいは一方に偏ったデータで学習したモデルは、一部の当事者をひいきするかもしれず、相手が共有のデータを汚そうとするかもしれません。これはNIST AI 100-2e2025と同じ趣旨です。
* **中立な記録の規則（提案）**: AIは異常を見つけ、証拠のまとめを準備してかまいません。しかし、ほかの組織や国についての結果を公表すること、登録簿の記載を直すこと、参加者を共有のデータから外すことは、透明な規則の下で、有資格の人が決めます。

### 4. 共有地に仕える専門家
職業の価値としての公平さ:

* **中立な管理者が信頼を得る**: 共有の記録を保つ人は、国籍や商業上の利益にかかわらず、すべての参加者に対して一貫してふるまわなければなりません。
* **国際協力には専門家が要る**: 共有の登録簿を築いて治めるには、多くの国の技術者、法律家、外交官、セキュリティの専門家の協力が必要です。
* **CISSPが信頼できる記録を支える**: CISSPのドメイン1は倫理と国際的な法の配慮を、ドメイン3は暗号による完全性を、ドメイン7は証拠の取り扱いとログを扱います。

### 5. 結論
語りがぶつかり合う世界で、改ざんが見える記録と共有の登録簿は、宇宙とサイバー空間で何が起きたかを理解するための共通の土台を、みんなに与えます。

透明性ログ、地上のシステムでの信頼できる検知、国際的な登録簿、中立な共有のデータ、注意深い証拠の基準、どちらの側にもつかずに見張りを助けるAI、そして公平な考えを持つ専門家を組み合わせることで、宇宙の世界は、誰でも確かめられる事実にもとづいて信頼が成り立つ共有地を築けます。
