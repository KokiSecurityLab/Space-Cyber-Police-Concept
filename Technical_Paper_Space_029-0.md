# Koki's Technical Paper — Space Cyber Defense Series SCD-029

## Signal Volume Control — Defending Against Floods of Data, Alerts, Requests, and False Information

### Summary Digest
Some attacks do not try to break in; they try to drown defenders. Network floods keep growing: in December 2025, a botnet built largely from hijacked home routers and other connected devices launched a distributed denial-of-service attack that peaked at 31.4 terabits per second, the largest publicly disclosed at the time, and one major provider mitigated 935 network-layer attacks exceeding 1 terabit per second in the first half of 2026. Floods also target people and AI: a March 2026 survey found that security teams received an average of 4,330 alerts per day and investigated only 37%, and the OWASP guidance on unbounded consumption warns that attackers can overload AI models to cause outages or drive up costs. False information can also be injected into shared threat intelligence, wasting defenders' effort.

This main paper of SCD-029 introduces volume control for space cyber defense. It applies CISSP Domains 4, 7, and 1, explains how alert floods, AI resource exhaustion, rate limiting, trusted-source prioritization, and poisoned intelligence feeds fit together, and shows why people must decide what matters most.

---
### 1. Why Volume Is a Weapon
Overwhelm Instead of Break In:

* **Floods Hide Real Attacks**: When systems and analysts are busy with noise, a real intrusion or command attempt can slip through unnoticed.
* **Floods Exhaust Limited Resources**: Ground station links, analysis capacity, AI compute budgets, and human attention are all finite, and attackers aim to use them up.
* **Space Systems Have Narrow Windows**: Contact passes with satellites are short, so even a brief flood at the wrong moment can block critical commands or data.

### 2. Five Foundations of Volume Control
A Structure for the SCD-029 Series:

* **Recognize Floods Against People and AI**: SCD-029-1 describes alert flooding against security teams, and SCD-029-2 describes resource exhaustion against AI models.
* **Control the Flow**: SCD-029-3 explains rate limiting and prioritization that protect the most important traffic and tasks.
* **Trust the Right Sources**: SCD-029-4 describes listening selectively to trusted sources, and SCD-029-5 describes defenses against poisoned threat intelligence feeds.

### 3. AI as a Filter Under Human Priorities
Sorting Signal From Noise:

* **AI Can Triage at Machine Speed**: AI can group duplicate alerts, filter obvious noise, and summarize large volumes of data so people can focus.
* **AI Filters Can Be Gamed or Overloaded**: Attackers may craft traffic that AI filters misjudge, or flood the AI itself, consistent with NIST AI 100-2e2025.
* **Proposed Volume Control Rule**: AI may filter, deduplicate, and prioritize data and alerts within rules set by people, but suppressing entire categories of alerts, blocking major sources, or changing priorities for mission-critical traffic is decided by qualified staff, and samples of filtered items are reviewed regularly.

### 4. People Who Decide What Matters
Judgment Under Pressure:

* **Adequate Staffing Prevents Overload**: Studies of security operations show that human analysts remain highly valued as a final line of defense, and teams need enough people to review what matters.
* **Mission Knowledge Guides Priorities**: Operators who understand which commands, passes, and data streams are critical can set priorities that automated tools follow.
* **CISSP Supports Volume Control**: CISSP Domain 4 covers network protection against floods, Domain 7 covers alert handling and incident response, and Domain 1 covers risk-based prioritization.

### 5. Conclusion
When attackers try to overwhelm rather than break in, the ability to control volume and focus on what matters becomes a key defense.

Recognizing floods against networks, people, and AI, limiting and prioritizing traffic, trusting verified sources, checking intelligence before acting on it, using AI to filter within human-set rules, and staffing teams adequately together let space missions stay focused on real threats even in a storm of noise.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-029

## 信号の量の管理 — データ、警報、要求、偽の情報のあふれから守る

### サマリー・ダイジェスト
攻撃の中には、侵入しようとするのではなく、守る側をおぼれさせようとするものがあります。ネットワークのあふれさせる攻撃は大きくなり続けています。2025年12月、主に乗っ取られた家庭用のルーターやほかのつながった機器で作られたボットネットが、ピークで毎秒31.4テラビットに達する分散型サービス妨害（DDoS）攻撃を行い、その時点で公表されたなかで最大となりました。ある大手の提供者は、2026年の前半に、毎秒1テラビットを超えるネットワーク層の攻撃を935件防ぎました。あふれさせる攻撃は人とAIも狙います。2026年3月の調査では、セキュリティのチームが一日に平均4,330件の警報を受け、調べられたのは37%だけでした。また、OWASPの「際限のない消費」の手引きは、攻撃者がAIのモデルに負荷をかけすぎて、止めたり費用を押し上げたりできると警告しています。偽の情報が共有の脅威の情報に差し込まれ、守る側の労力をむだにさせることもあります。

SCD-029の本編である本論文は、宇宙のサイバー防衛のための量の管理を紹介します。CISSPのドメイン4、7、1を適用し、警報のあふれ、AIの資源を使い果たさせる攻撃、流量の制限、信頼できる源の優先、汚された脅威の情報がどう組み合わさるかを説明し、何がいちばん大切かを人が決めなければならない理由を示します。

---
### 1. 量が武器になる理由
侵入するのではなく、圧倒する:

* **あふれは本当の攻撃を隠す**: システムと分析担当者が雑音で忙しいとき、本当の侵入や指令の試みが、気づかれずにすり抜けることがあります。
* **あふれは限られた資源を使い果たさせる**: 地上局のリンク、分析の力、AIの計算の予算、人の注意はどれも限りがあり、攻撃者はそれを使い切らせようとします。
* **宇宙のシステムには狭い時間の窓がある**: 衛星との交信の通過は短いため、悪いときの短いあふれでさえ、大事な指令やデータをふさいでしまうことがあります。

### 2. 量の管理の5つの土台
SCD-029シリーズの構成:

* **人とAIへのあふれを見分ける**: SCD-029-1はセキュリティのチームへの警報のあふれを、SCD-029-2はAIのモデルの資源を使い果たさせる攻撃を説明します。
* **流れを管理する**: SCD-029-3は、いちばん大切な通信と仕事を守る、流量の制限と優先順位付けを説明します。
* **正しい源を信じる**: SCD-029-4は信頼できる源を選んで聞くことを、SCD-029-5は汚された脅威の情報への守りを説明します。

### 3. 人の優先順位の下でのふるいとしてのAI
合図と雑音を分ける:

* **AIは機械の速さで振り分けられる**: AIは重複した警報をまとめ、明らかな雑音をふるい落とし、大量のデータを要約して、人が集中できるようにします。
* **AIのふるいはごまかされたり、圧倒されたりしうる**: 攻撃者は、AIのふるいが見誤る通信を作り込んだり、AIそのものをあふれさせたりするかもしれません。これはNIST AI 100-2e2025と同じ趣旨です。
* **量の管理の規則（提案）**: AIは、人が決めた規則の中で、データと警報をふるい分け、重複を除き、優先順位を付けてかまいません。しかし、ある種類の警報を丸ごと抑えること、大きな源をふさぐこと、ミッションに欠かせない通信の優先順位を変えることは、有資格の担当者が決め、ふるい落とされたものの一部は定期的に確かめます。

### 4. 何が大切かを決める人々
圧力の下での判断:

* **十分な人数が圧倒を防ぐ**: セキュリティの運用の研究は、人の分析担当者が最後の守りとして今も高く評価されていることを示しており、チームには大切なものを確かめられるだけの人が必要です。
* **ミッションの知識が優先順位を導く**: どの指令、通過、データの流れが欠かせないかを理解する運用者が、自動の道具が従う優先順位を決められます。
* **CISSPが量の管理を支える**: CISSPのドメイン4はあふれからのネットワークの保護を、ドメイン7は警報の取り扱いとインシデント対応を、ドメイン1はリスクにもとづく優先順位付けを扱います。

### 5. 結論
攻撃者が侵入するのではなく圧倒しようとするとき、量を管理し、大切なことに集中する力が、大事な守りになります。

ネットワーク、人、AIへのあふれを見分け、通信を制限して優先順位を付け、確かめられた源を信じ、行動する前に情報を確かめ、人が決めた規則の中でAIにふるい分けさせ、チームに十分な人数をそろえることで、宇宙のミッションは、雑音の嵐の中でも、本当の脅威に集中し続けられます。
