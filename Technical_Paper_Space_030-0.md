# Koki's Technical Paper — Space Cyber Defense Series SCD-030

## Mission Integrity — Human-Led Space Defense at the Midpoint of the Series

### Summary Digest
The first thirty papers of this series have covered threats, links, power, swarms, debris, orbital computing, supply chains, timing, authentication, incident response, mesh networks, ethics, resilience, neutrality, disinformation, fairness, data truth, authentic imagery, AI supply chains, human judgment, agent authority, and floods of noise. One theme connects them all: mission integrity, the assurance that a space mission does what its people intend, and nothing else, even under attack. AI is now powerful on both sides. In November 2026, one AI developer described an automated pipeline that found, validated, and generated patches for Linux kernel vulnerabilities, with human researchers reviewing every fix before submission, while an August 2026 study found that the expected value of fully AI-generated patches without human review was negative.

This main paper of SCD-030 summarizes the first half of the series and defines mission integrity. It applies CISSP Domains 1, 7, and 8, explains how measurement, the risks of AI self-healing, patch poisoning, and human authority over change fit together, and outlines the road to the second half.

---
### 1. What Mission Integrity Means
Doing What People Intend, and Nothing Else:

* **Integrity of Commands and Software**: Only authorized, verified commands and software run on spacecraft and ground systems, as described in SCD-014 and SCD-026.
* **Integrity of Data and Decisions**: Data is genuine, as described in SCD-024 and SCD-025, and decisions remain human-led, as described in SCD-027 and SCD-028.
* **Integrity Over Time**: Missions stay trustworthy through changes, updates, and recoveries, which is where many hidden risks appear.

### 2. Five Foundations of Mission Integrity
A Structure for the SCD-030 Series:

* **Measure and Understand**: SCD-030-1 explains how to measure mission integrity, and SCD-030-2 examines the risks of letting AI repair systems on its own.
* **Guard Every Change**: SCD-030-3 describes how advanced AI could poison patches, and SCD-030-4 describes human authority over all significant changes.
* **Look Ahead**: SCD-030-5 outlines the second half of the series, SCD-031 to SCD-050.

### 3. AI Across the Mission Under Human Authority
Powerful Help, Clear Limits:

* **AI Finds and Fixes Faster Than Ever**: AI can discover vulnerabilities, propose patches, and monitor systems at a speed people cannot match.
* **AI Fixes Can Be Wrong or Weaponized**: Studies show many AI patches are incomplete or change behavior, and adversaries may use AI to create malicious fixes, consistent with NIST AI 100-2e2025.
* **Proposed Mission Integrity Rule**: AI may find problems, propose fixes, and verify results, but changes to flight software, command systems, keys, and safety rules are approved by qualified people after independent testing, and the final decision always rests with humans.

### 4. The People Who Keep Missions Whole
A Profession That Grows With AI:

* **AI Changes the Work, Not the Need for People**: An ISC2 survey in May 2026 of 856 professionals who use AI found that AI is reshaping cybersecurity roles and increasing human oversight, and ISC2's leadership stated that AI is not replacing cybersecurity professionals.
* **Skills Matter More Than Ever**: The 2025 ISC2 workforce study of more than 16,000 professionals found that 88% had experienced at least one significant security event because of skills shortages.
* **CISSP Connects the Whole Series**: CISSP Domain 1 covers governance and ethics, Domain 7 covers operations and response, and Domain 8 covers secure software and change, the three pillars of mission integrity.

### 5. Conclusion
Mission integrity is the promise that a space mission serves the people who built it, and that promise must hold through every attack, update, and recovery.

By measuring integrity, treating AI self-healing with care, guarding against poisoned patches, keeping human authority over change, and investing in skilled professionals, the space community can enter the second half of this series with a clear purpose: AI that strengthens human-led missions, never one that replaces the people who lead them.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-030

## ミッションの完全性 — シリーズの折り返し点での、人が主導する宇宙防衛

### サマリー・ダイジェスト
このシリーズの最初の30本は、脅威、リンク、電力、群れ、デブリ、軌道上の計算、サプライチェーン、時刻、本人確認、インシデント対応、メッシュのネットワーク、倫理、しなやかな強さ、中立、偽情報、公平さ、データの真実、本物の画像、AIのサプライチェーン、人の判断、エージェントの権限、雑音のあふれを扱ってきました。それらすべてをつなぐひとつのテーマがあります。ミッションの完全性、つまり、攻撃を受けているときでも、宇宙のミッションがその人々の意図することをし、それ以外は何もしないという保証です。AIは今、両方の側で強力です。2026年11月、あるAIの開発者は、Linuxのカーネルの脆弱性を見つけ、確かめ、修正を作る自動の流れを説明し、人の研究者が提出の前にすべての修正を確かめたと述べました。一方、2026年8月の研究は、人の確認なしに完全にAIが作った修正の期待値はマイナスだと見いだしました。

SCD-030の本編である本論文は、シリーズの前半をまとめ、ミッションの完全性を定めます。CISSPのドメイン1、7、8を適用し、測り方、AIによる自己修復のリスク、修正（パッチ）の汚染、変更に対する人の権限がどう組み合わさるかを説明し、後半への道筋を示します。

---
### 1. ミッションの完全性とは
人の意図することをし、それ以外は何もしない:

* **指令とソフトウェアの完全性**: SCD-014とSCD-026で述べたように、許可され確かめられた指令とソフトウェアだけが、宇宙機と地上のシステムで動きます。
* **データと判断の完全性**: SCD-024とSCD-025で述べたようにデータは本物で、SCD-027とSCD-028で述べたように判断は人が主導し続けます。
* **時間を通じた完全性**: ミッションは変更、更新、回復を通じて信頼できるままでいなければならず、多くの隠れたリスクはそこに現れます。

### 2. ミッションの完全性の5つの土台
SCD-030シリーズの構成:

* **測り、理解する**: SCD-030-1はミッションの完全性の測り方を説明し、SCD-030-2はAIに自分でシステムを直させることのリスクを調べます。
* **すべての変更を守る**: SCD-030-3は高度なAIが修正をどう汚しうるかを、SCD-030-4はすべての大事な変更に対する人の権限を説明します。
* **先を見る**: SCD-030-5はシリーズの後半、SCD-031からSCD-050の道筋を示します。

### 3. 人の権限の下での、ミッション全体のAI
強力な助けと、はっきりした限度:

* **AIはかつてなく速く見つけて直す**: AIは、人がかなわない速さで、脆弱性を見つけ、修正を提案し、システムを見張れます。
* **AIの修正は間違ったり武器にされたりしうる**: 研究は多くのAIの修正が不完全だったり、ふるまいを変えたりすることを示しており、相手はAIを使って悪意ある修正を作るかもしれません。これはNIST AI 100-2e2025と同じ趣旨です。
* **ミッションの完全性の規則（提案）**: AIは問題を見つけ、修正を提案し、結果を確かめてかまいません。しかし、飛行ソフトウェア、指令のシステム、鍵、安全の規則の変更は、独立した試験の後に有資格の人が承認し、最終の判断はいつも人にあります。

### 4. ミッションを丸ごと守る人々
AIとともに育つ職業:

* **AIは仕事を変えるが、人の必要はなくさない**: AIを使う856人の専門家への2026年5月のISC2の調査は、AIがサイバーセキュリティの役割を形づくり直し、人による見守りを増やしていることを見いだし、ISC2の指導者は、AIがサイバーセキュリティの専門家を置き換えているのではないと述べました。
* **技能はこれまで以上に大切**: 1万6,000人を超える専門家への2025年のISC2の働き手の調査は、88%が技能の不足のために少なくとも一度は大きなセキュリティの出来事を経験していたことを見いだしました。
* **CISSPがシリーズ全体をつなぐ**: CISSPのドメイン1はガバナンスと倫理を、ドメイン7は運用と対応を、ドメイン8は安全なソフトウェアと変更を扱い、それがミッションの完全性の3本の柱です。

### 5. 結論
ミッションの完全性とは、宇宙のミッションがそれを築いた人々に仕えるという約束であり、その約束は、すべての攻撃、更新、回復を通じて守られなければなりません。

完全性を測り、AIによる自己修復を注意深く扱い、汚された修正から守り、変更に対する人の権限を保ち、技能のある専門家に投資することで、宇宙の世界は、はっきりした目的を持ってこのシリーズの後半に進めます。それは、人が主導するミッションを強めるAIであり、決してミッションを率いる人々を置き換えるAIではありません。
