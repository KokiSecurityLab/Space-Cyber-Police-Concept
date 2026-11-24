# Koki's Technical Paper — Space Cyber Defense Series SCD-026

## The Clean Training Ground — Securing the Supply Chain of AI Models Used in Space

### Summary Digest
AI is moving into orbit. In April 2026, a satellite in low Earth orbit ran a vision-language model onboard to classify and describe live Earth imagery, which its developers described as the first such in-orbit demonstration, and other 2026 missions demonstrated onboard object detection and in-orbit updates of onboard models. Every one of these models depends on training data, open-source libraries, pretrained weights, and outside services, creating a new supply chain that attackers can target. In May 2026, the U.S. Cybersecurity and Infrastructure Security Agency (CISA) and G7 partners released joint guidance on minimum elements of a software bill of materials for AI, recognizing that AI systems introduce models, datasets, performance indicators, and AI-specific infrastructure as additional components.

This main paper of SCD-026 introduces AI supply chain security for space missions. It applies CISSP Domains 1, 3, and 8, explains how AI bills of materials, protection against data poisoning, model signing, third-party service risk, and safe in-orbit updates fit together, and shows why people must control the AI supply chain.

---
### 1. Why the AI Supply Chain Matters in Space
New Components, New Risks:

* **Models Depend on Many Sources**: A single onboard model may combine public datasets, pretrained weights, open-source code, and vendor tools, each of which could be compromised.
* **Problems Are Hard to Fix in Orbit**: A flawed or tampered model on a spacecraft may be difficult to replace, and errors may affect decisions far from human oversight.
* **Fake Models Already Appear**: In May 2026, a malicious repository impersonating an official model release on a popular model-sharing platform reached the top of its trending list before being removed.

### 2. Five Foundations of a Clean AI Supply Chain
A Structure for the SCD-026 Series:

* **Know What Is Inside**: SCD-026-1 describes the AI bill of materials, and SCD-026-2 explains how training data can be poisoned and protected.
* **Prove Integrity**: SCD-026-3 describes model signing, which lets operators verify that a model has not been altered.
* **Manage Outside Dependencies and Change**: SCD-026-4 describes risks from third-party AI services, and SCD-026-5 describes how to update models in orbit safely.

### 3. AI Supply Chain Under Human Control
Automation Requires Accountability:

* **AI Builds and Tests AI**: Automated pipelines train, evaluate, and package models quickly, making supply chain checks essential at every step.
* **Supply Chain Attacks Can Hide in Models**: Poisoned data, hidden backdoors, and malicious files in model packages can pass casual review, consistent with NIST AI 100-2e2025.
* **Proposed Clean Training Ground Rule**: AI pipelines may automatically build, scan, and test models, but approving a model for flight, accepting new training data sources, and changing third-party AI providers are decisions made by qualified people with documented review.

### 4. People Who Keep the Training Ground Clean
New Roles for a New Supply Chain:

* **AI Security Engineers Are Needed**: Professionals who understand both machine learning and supply chain security are in growing demand as AI spreads into space systems.
* **Data and Model Stewards Provide Oversight**: People who track datasets, model versions, and approvals ensure that every onboard model can be traced and trusted.
* **CISSP Supports AI Supply Chain Security**: CISSP Domain 1 covers supply chain risk management, Domain 3 covers integrity and cryptography, and Domain 8 covers secure development and testing.

### 5. Conclusion
As AI models fly aboard spacecraft, their supply chain becomes part of mission security.

Clear AI bills of materials, protection against poisoned data, signed and verified models, careful management of third-party services, safe in-orbit update procedures, automated checks under human approval, and skilled AI security professionals together create a clean training ground for the AI that will help explore and protect space.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-026

## きれいな学びの場 — 宇宙で使うAIモデルのサプライチェーンを守る

### サマリー・ダイジェスト
AIは軌道の上へ移りつつあります。2026年4月、低軌道のある衛星が、生きた地球の画像を分類して説明するために、衛星の上で視覚と言語のモデルを動かし、開発者はそれを軌道上での初めての実演だと述べました。2026年のほかのミッションでも、衛星の上での物体の検出や、搭載したモデルの軌道上での更新が実演されました。これらのモデルはどれも、学習データ、オープンソースのライブラリ、事前に学習した重み、外のサービスに頼っており、攻撃者が狙える新しいサプライチェーンを生んでいます。2026年5月、米国のサイバーセキュリティ・インフラセキュリティ庁（CISA）とG7の協力国は、AIのためのソフトウェア部品表の最小の要素についての共同の手引きを出し、AIのシステムが、モデル、データの集まり、性能の指標、AIに特有の基盤を、追加の部品として持ち込むことを認めました。

SCD-026の本編である本論文は、宇宙のミッションのためのAIのサプライチェーンのセキュリティを紹介します。CISSPのドメイン1、3、8を適用し、AI部品表、データの汚染からの守り、モデルへの署名、外部のサービスのリスク、軌道上での安全な更新がどう組み合わさるかを説明し、AIのサプライチェーンを人が管理しなければならない理由を示します。

---
### 1. 宇宙でAIのサプライチェーンが大切な理由
新しい部品、新しいリスク:

* **モデルは多くの源に頼る**: 搭載するひとつのモデルが、公開のデータの集まり、事前に学習した重み、オープンソースのコード、販売元の道具を組み合わせていることがあり、そのどれもが乗っ取られうるのです。
* **軌道の上では問題を直しにくい**: 宇宙機の上の欠陥のある、あるいは改ざんされたモデルは取り替えにくいことがあり、誤りが人の見守りから遠く離れた判断に影響するかもしれません。
* **偽のモデルはすでに現れている**: 2026年5月、人気のあるモデルの共有の場で、公式のモデルの公開になりすました悪意あるリポジトリが、取り除かれる前に注目の一覧の一位にまで達しました。

### 2. きれいなAIのサプライチェーンの5つの土台
SCD-026シリーズの構成:

* **中に何があるかを知る**: SCD-026-1はAI部品表を、SCD-026-2は学習データがどう汚され、どう守れるかを説明します。
* **完全性を証明する**: SCD-026-3は、モデルが変えられていないことを運用者が確かめられる、モデルへの署名を説明します。
* **外への依存と変更を管理する**: SCD-026-4は外部のAIサービスからのリスクを、SCD-026-5は軌道の上でモデルを安全に更新するやり方を説明します。

### 3. 人の管理の下での、AIのサプライチェーン
自動化には説明責任が要る:

* **AIがAIを作り、試す**: 自動の流れはモデルを速く学習させ、評価し、まとめるため、すべての段階でのサプライチェーンの確認が欠かせません。
* **サプライチェーンの攻撃はモデルの中に隠れうる**: 汚されたデータ、隠れた裏口、モデルのパッケージの中の悪意あるファイルは、ざっとした確認を通ってしまうことがあります。これはNIST AI 100-2e2025と同じ趣旨です。
* **きれいな学びの場の規則（提案）**: AIの流れはモデルを自動で作り、調べ、試してかまいません。しかし、モデルを飛行用として承認すること、新しい学習データの源を受け入れること、外部のAIの提供者を変えることは、記録した確認を伴って、有資格の人が決めます。

### 4. 学びの場をきれいに保つ人々
新しいサプライチェーンのための新しい役割:

* **AIのセキュリティの技術者が必要**: AIが宇宙のシステムに広がるにつれ、機械学習とサプライチェーンのセキュリティの両方を理解する専門家がますます求められています。
* **データとモデルの管理者が見守る**: データの集まり、モデルの版、承認を追いかける人が、搭載するすべてのモデルをたどれて信頼できるものにします。
* **CISSPがAIのサプライチェーンのセキュリティを支える**: CISSPのドメイン1はサプライチェーンのリスク管理を、ドメイン3は完全性と暗号を、ドメイン8は安全な開発と試験を扱います。

### 5. 結論
AIのモデルが宇宙機に載って飛ぶようになると、そのサプライチェーンはミッションのセキュリティの一部になります。

はっきりしたAI部品表、汚されたデータからの守り、署名されて確かめられたモデル、外部のサービスの注意深い管理、軌道上での安全な更新の手順、人の承認の下での自動の確認、そして技能のあるAIのセキュリティの専門家が合わさることで、宇宙を探り守る助けになるAIのための、きれいな学びの場が生まれます。
