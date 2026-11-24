# Koki's Technical Paper — Space Cyber Defense Series SCD-015

## Dark Data Scrubbing — Keeping Shared Orbital Computing Clean of Residual Data, Hidden Channels, and Poison

### Summary Digest
Computing is moving into orbit. In November 2025, the first data-center-class GPU was launched into space and used to train a small language model, in January 2026 the first two orbital data center nodes reached low Earth orbit, and a commercial cloud module is planned to offer GPU capacity from orbit to customers by early 2027. When many customers share the same orbital hardware, data left behind, hidden communication paths, and poisoned training data become serious risks.

This main paper of SCD-015 introduces data hygiene for shared orbital computing. It applies CISSP Domains 2, 3, and 8, explains how residual data, covert channels, data poisoning, and unnecessary retention threaten tenants, and shows why people must decide how data is cleaned, kept, and deleted.

---
### 1. Why Shared Orbital Computing Needs Data Hygiene
Many Tenants, One Machine:

* **Leftover Data Can Leak**: In 2024, researchers disclosed a GPU vulnerability in which one process could read data left in local memory by another, enough to reconstruct another user's AI chatbot responses.
* **Hidden Channels Can Bypass Isolation**: Research in 2025 and 2026 showed that shared GPU caches, interconnects, and power-saving features can create covert channels through which separated workloads exchange information.
* **Small Poison Has Large Effects**: An October 2025 study by an AI company with UK government and academic partners found that as few as 250 malicious documents could create a backdoor in language models from 600 million to 13 billion parameters.

### 2. Four Practices of Dark Data Scrubbing
A Structure for the SCD-015 Series:

* **Separate Noise From Poison**: SCD-015-1 explains how to distinguish natural sensor noise in space from deliberately poisoned data.
* **Clear Residual Data and Watch Hidden Channels**: SCD-015-2 covers clearing memory between tenants, and SCD-015-3 covers detecting covert channels in shared hardware.
* **Purify and Minimize**: SCD-015-4 describes pipelines that clean training data, and SCD-015-5 explains why keeping less data for less time reduces risk.

### 3. AI Data Hygiene Under Human Authority
Automated Cleaning, Human Responsibility:

* **AI Helps Find Hidden Problems**: AI can scan large datasets for unusual patterns, detect abnormal resource contention between tenants, and verify that memory has been cleared.
* **Cleaning Tools Can Be Fooled**: Poisoned data may be crafted to look normal, and detection models can be manipulated, consistent with NIST AI 100-2e2025, so data cleaning combines statistical checks with provenance records.
* **Proposed Data Hygiene Rule**: Automated systems may clear memory, quarantine suspicious data, and enforce retention schedules, but placing tenants with different trust levels on the same hardware, releasing quarantined training data, or extending retention of sensitive data is approved by qualified data stewards and security staff.

### 4. People Who Keep the Data Clean
Responsibility That Stays Human:

* **Workplace Guidance Points to Human Control**: A November 2026 report summarizing advice from cybersecurity leaders, including the head of ISC2, recommended limiting AI access to data, accounts, and systems, checking AI outputs every time, and keeping a named person accountable even when AI agents do the work.
* **Demand for Skilled People Is Rising**: The same report noted growing demand for cybersecurity, information security, AI project management, and ethics and governance roles, and recommended redesigning roles so that no one is left behind.
* **CISSP Supports Data Stewardship**: CISSP Domain 2 covers data classification, retention, and secure deletion, Domain 3 covers isolation in shared systems, and Domain 8 covers secure handling of data in AI development.

### 5. Conclusion
Shared orbital computing brings great opportunity, but it also brings old data problems to a new place, where residual data, hidden channels, and poisoned inputs can quietly undermine trust.

Clearing memory between tenants, watching for covert channels, purifying training data, keeping only what is needed, using AI to find hidden problems, and giving trained people final responsibility together let orbital computing grow into a clean and trustworthy service for everyone who relies on it.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-015

## 暗いデータの掃除 — 共有の軌道上の計算環境を、残ったデータ、隠れた通信路、汚染から守る

### サマリー・ダイジェスト
計算の場は軌道上に移りつつあります。2025年11月、データセンター級のGPUが初めて宇宙に打ち上げられ、小さな言語モデルの学習に使われました。2026年1月には最初の2つの軌道上データセンターのノードが低軌道に届き、2027年の初めまでには、商用のクラウドの区画が、軌道上のGPUの計算能力を顧客に提供する計画です。多くの顧客が同じ軌道上のハードウェアを分け合うと、後に残ったデータ、隠れた通信路、汚された学習データが深刻なリスクになります。

SCD-015の本編である本論文は、共有の軌道上の計算環境のための「データの衛生」を紹介します。CISSPのドメイン2、3、8を適用し、残ったデータ、隠れた通信路、データの汚染、不要な保存がどのように利用者をおびやかすかを説明し、データをどうきれいにし、保ち、消すかを人が決めなければならない理由を示します。

---
### 1. 共有の軌道上の計算にデータの衛生が必要な理由
多くの利用者、ひとつの機械:

* **残ったデータは漏れることがある**: 2024年、研究者は、あるプロセスが、別のプロセスがローカルメモリーに残したデータを読めてしまうGPUの脆弱性を公表しました。ほかの利用者のAIチャットボットの応答を組み立て直せるほどの量でした。
* **隠れた通信路が隔離をすり抜けることがある**: 2025年と2026年の研究は、共有のGPUのキャッシュ、GPUどうしをつなぐ経路、省電力の機能が、分けられているはずの処理どうしが情報をやりとりできる、隠れた通信路を生みうることを示しました。
* **小さな汚染が大きな影響を持つ**: AI企業が英国政府や学術機関と行った2025年10月の研究では、わずか250の悪意のある文書で、6億から130億のパラメーターを持つ言語モデルに裏口（バックドア）を作れることがわかりました。

### 2. 暗いデータの掃除の4つの実践
SCD-015シリーズの構成:

* **雑音と汚染を分ける**: SCD-015-1は、宇宙での自然なセンサーの雑音と、わざと汚されたデータを見分ける方法を説明します。
* **残ったデータを消し、隠れた通信路を見張る**: SCD-015-2は利用者の間でメモリーを消すことを、SCD-015-3は共有のハードウェアの中の隠れた通信路を見つけることを扱います。
* **きれいにし、最小限にする**: SCD-015-4は学習データをきれいにする流れを、SCD-015-5はデータをより少なく、より短く持つことがなぜリスクを減らすのかを説明します。

### 3. 人の権限の下での、AIによるデータの衛生
自動の掃除、人の責任:

* **AIが隠れた問題を見つける助けになる**: AIは大量のデータの中から普段と違う型を探し、利用者どうしの間の異常な資源の取り合いを見つけ、メモリーが消されたことを確かめられます。
* **掃除の道具はだまされることがある**: 汚されたデータは普通に見えるよう作られていることがあり、検知のモデルは操作されることがあります。これはNIST AI 100-2e2025と同じ趣旨です。そのため、データの掃除では、統計による確認と、出どころの記録を組み合わせます。
* **データの衛生の規則（提案）**: 自動のシステムは、メモリーを消し、疑わしいデータを隔離し、保存期間の予定を守らせてかまいません。しかし、信頼の度合いの違う利用者を同じハードウェアに置くこと、隔離した学習データを解き放つこと、機密のデータの保存期間を延ばすことは、有資格のデータの管理者とセキュリティの担当者が承認します。

### 4. データをきれいに保つ人々
人に残る責任:

* **職場への助言は人による制御を指している**: ISC2のトップを含むサイバーセキュリティの指導者たちの助言をまとめた2026年11月の記事は、AIがアクセスできるデータ、アカウント、システムを絞ること、AIの出力を毎回確かめること、AIエージェントが作業をしても説明責任を持つ担当者をはっきりさせておくことを勧めました。
* **技能のある人の需要は高まっている**: 同じ記事は、サイバーセキュリティ、情報セキュリティ、AIのプロジェクト管理、倫理とガバナンスの職種の需要が高まっていると伝え、誰も取り残されないよう組織の中の役割を設計し直すことを勧めました。
* **CISSPがデータの管理を支える**: CISSPのドメイン2はデータの分類、保存、安全な消去を、ドメイン3は共有システムの中での隔離を、ドメイン8はAIの開発でのデータの安全な扱いを扱います。

### 5. 結論
共有の軌道上の計算は大きな機会をもたらしますが、古くからのデータの問題も新しい場所に持ち込みます。そこでは、残ったデータ、隠れた通信路、汚された入力が、静かに信頼を損なうことがあります。

利用者の間でメモリーを消し、隠れた通信路を見張り、学習データをきれいにし、必要なものだけを持ち、隠れた問題を見つけるためにAIを使い、訓練を受けた人に最終的な責任を持たせることで、軌道上の計算は、それに頼るすべての人のための、きれいで信頼できるサービスへと育っていけます。
