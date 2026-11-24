# Koki's Technical Paper — Space Cyber Defense Series SCD-024

## Sovereign Truth Anchoring — Proving Where Space Data Came From and That It Has Not Changed

### Summary Digest
Decisions about disasters, farming, navigation, climate, and security increasingly depend on data from space, so people need to know that the data is genuine. Satellite navigation already offers a public example: Galileo's Open Service Navigation Message Authentication (OSNMA), declared operational on July 24, 2025, embeds a digital signature in the open signal so that compatible receivers can verify that navigation data comes from Galileo and has not been tampered with, and it is provided free of charge. For Earth observation, European Space Agency projects are developing services that sign satellite imagery and trace each processing step so that users can "walk back" the history of a data product. Ground calibration networks add another anchor by comparing satellite measurements with independent measurements taken on the ground.

This main paper of SCD-024 introduces truth anchoring for space data. It applies CISSP Domains 3, 2, and 7, explains how provenance, signing at the source, ground-truth checks, chain of custody, and trust levels work together, and shows why people must interpret and govern data trust.

---
### 1. Why Space Data Needs Proof
Decisions Depend on Trustworthy Data:

* **Tampering Can Happen Anywhere**: Data can be altered on the satellite, during downlink, in ground processing, in storage, or during distribution to users.
* **Fake Data Can Look Real**: Injected or modified data may pass basic checks, leading users to make wrong decisions about safety, resources, or responses to incidents.
* **Proof Supports Trust Across Borders**: When data can be verified independently, users in different countries and organizations can rely on it without simply trusting the provider.

### 2. Five Anchors of Data Truth
A Structure for the SCD-024 Series:

* **Know the History and the Origin**: SCD-024-1 describes provenance from sensor to user, and SCD-024-2 describes signing data at the source.
* **Compare With Reality**: SCD-024-3 explains how ground-truth measurements and cross-checks detect errors and manipulation.
* **Preserve and Communicate Trust**: SCD-024-4 describes chain of custody, and SCD-024-5 describes trust levels that help data consumers decide how much to rely on data.

### 3. AI-Derived Data and Human Responsibility
Verifying What Machines Produce:

* **AI Creates More Derived Data**: AI models turn raw satellite data into maps, detections, and forecasts, adding steps where errors or manipulation can enter.
* **AI Outputs Need Provenance Too**: Records should show which model version, input data, and settings produced a result, because models can be poisoned or drift, consistent with NIST AI 100-2e2025.
* **Proposed Data Truth Rule**: AI may process, verify, and score data automatically, but declaring data authentic for legal or public use, correcting published datasets, or rejecting a provider's data as untrustworthy is decided by qualified people who review the evidence.

### 4. People Who Anchor the Truth
Trust Requires Expertise:

* **Calibration and Validation Specialists**: Scientists who measure ground conditions and compare them with satellite data keep data accurate over many years.
* **Security and Data Professionals Work Together**: Protecting data integrity requires both cryptography experts and people who understand how the data is collected and used.
* **CISSP Supports Data Integrity**: CISSP Domain 3 covers cryptography and integrity mechanisms, Domain 2 covers data ownership and lifecycle, and Domain 7 covers evidence handling.

### 5. Conclusion
As more of the world's decisions depend on space data, proving that data is genuine becomes a foundation for safety and trust.

Recorded provenance, signatures at the source, comparisons with ground truth, careful chain of custody, clear trust levels, AI processing that is itself traceable, and skilled people who interpret the evidence together anchor space data to the truth.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-024

## 真実のつなぎとめ — 宇宙のデータがどこから来て、変えられていないことを証明する

### サマリー・ダイジェスト
災害、農業、測位、気候、安全保障についての判断は、ますます宇宙からのデータにかかっています。そのため、人々にはデータが本物だと知る必要があります。衛星測位には、すでに公の例があります。ガリレオの「オープンサービスの航法メッセージ認証（OSNMA）」は、2025年7月24日に運用を宣言され、開かれた信号の中にデジタル署名を埋め込んで、対応した受信機が、航法のデータがガリレオから来て、改ざんされていないことを確かめられるようにしています。しかも無料で提供されています。地球観測では、欧州宇宙機関（ESA）の取り組みが、衛星画像に署名し、処理の一段階ずつを記録するサービスを開発しており、利用者がデータの製品の歴史を「さかのぼって」確かめられるようにしています。地上の較正のネットワークは、衛星の測定を地上で取った独立の測定と比べることで、もうひとつのつなぎとめを加えます。

SCD-024の本編である本論文は、宇宙のデータの真実のつなぎとめを紹介します。CISSPのドメイン3、2、7を適用し、来歴、発生源での署名、地上の実測との照合、証拠保全の連鎖、信頼度がどう組み合わさるかを説明し、データの信頼を人が読み解き、治めなければならない理由を示します。

---
### 1. 宇宙のデータに証明が必要な理由
判断は信頼できるデータにかかっている:

* **改ざんはどこででも起こりうる**: データは、衛星の上で、地上への送信の途中で、地上の処理の中で、保存の中で、利用者への配布の途中で、変えられることがあります。
* **偽のデータは本物に見えることがある**: 送り込まれたり変えられたりしたデータが基本の確認を通り、利用者が安全、資源、事件への対応について間違った判断をしてしまうかもしれません。
* **証明が国境を越えた信頼を支える**: データを独立に確かめられれば、違う国や組織の利用者が、提供者をただ信じるのではなく、それに頼れます。

### 2. データの真実の5つのつなぎとめ
SCD-024シリーズの構成:

* **歴史と出どころを知る**: SCD-024-1はセンサーから利用者までの来歴を、SCD-024-2は発生源でのデータの署名を説明します。
* **現実と比べる**: SCD-024-3は、地上の実測と照らし合わせが、誤りと操作をどう見つけるかを説明します。
* **信頼を保ち、伝える**: SCD-024-4は証拠保全の連鎖を、SCD-024-5はデータの利用者がどれだけ頼るかを決める助けになる信頼度を説明します。

### 3. AIから生まれるデータと、人の責任
機械が作るものを確かめる:

* **AIはより多くの加工データを生む**: AIのモデルは、衛星の生のデータを地図、検出、予測に変え、誤りや操作が入り込みうる段階を増やします。
* **AIの出力にも来歴が要る**: モデルは汚されたり、性能がずれたりすることがあるため、どのモデルの版、入力のデータ、設定が結果を生んだかを記録に残すべきです。これはNIST AI 100-2e2025と同じ趣旨です。
* **データの真実の規則（提案）**: AIはデータを自動で処理し、確かめ、点数を付けてかまいません。しかし、法律や公の場で使うためにデータを本物と宣言すること、公開したデータの集まりを直すこと、提供者のデータを信頼できないとして退けることは、証拠を確かめる有資格の人が決めます。

### 4. 真実をつなぎとめる人々
信頼には専門性が要る:

* **較正と検証の専門家**: 地上の状態をはかり、それを衛星のデータと比べる科学者が、長い年月にわたってデータを正確に保ちます。
* **セキュリティとデータの専門家が協力する**: データの完全性を守るには、暗号の専門家と、データがどう集められ使われるかを理解する人の両方が必要です。
* **CISSPがデータの完全性を支える**: CISSPのドメイン3は暗号と完全性の仕組みを、ドメイン2はデータの持ち主とライフサイクルを、ドメイン7は証拠の取り扱いを扱います。

### 5. 結論
世界の判断の多くが宇宙のデータにかかるようになるにつれ、データが本物だと証明することは、安全と信頼の土台になります。

記録された来歴、発生源での署名、地上の実測との比較、注意深い証拠保全の連鎖、はっきりした信頼度、それ自体もたどれるAIの処理、そして証拠を読み解く技能のある人々が合わさることで、宇宙のデータを真実につなぎとめられます。
