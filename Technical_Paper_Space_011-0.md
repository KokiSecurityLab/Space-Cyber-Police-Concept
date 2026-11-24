# Koki's Technical Paper — Space Cyber Defense Series SCD-011

## The Early Warning Line — Detecting Reconnaissance Before an Attack on Space Systems

### Summary Digest
Most serious attacks begin with quiet preparation: mapping exposed systems, collecting public information, and testing defenses. A 2025 threat landscape report identified 407 attacks targeting the space sector, and none of them hit a satellite in orbit; they affected company IT environments, ground stations, and user modems on Earth, which are exactly the places where reconnaissance happens first.

This main paper of SCD-011 introduces reconnaissance detection as an early warning line for space systems. It applies CISSP Domains 1, 6, and 7, explains how exposure mapping, scan detection, open-source intelligence review, deception, and information sharing work together, and shows why trained analysts must decide what early warnings mean.

---
### 1. Why Reconnaissance Is the Best Moment to Act
Seeing the Attacker Before the Attack:

* **Attacks Follow Preparation**: Attackers usually identify targets, learn their technology, and find weak points before they act, so detecting this stage gives defenders time to close gaps.
* **The Ground Segment Is the Front Door**: Because recent attacks on the space sector have affected ground stations, company networks, and user terminals rather than satellites in orbit, reconnaissance against these systems deserves close attention.
* **Early Detection Costs Less**: Stopping an attacker during reconnaissance avoids the far larger cost of responding to a breach, restoring systems, and rebuilding trust.

### 2. Five Layers of the Early Warning Line
A Structure for the SCD-011 Series:

* **Know Your Own Exposure**: Organizations map which ground systems are visible on the internet, as described in SCD-011-1, because attackers use the same public scanning tools.
* **Watch for Probing and Gather Public Clues**: Patterns of scanning, covered in SCD-011-2, and information that leaks through public sources, covered in SCD-011-3, reveal what an attacker may already know.
* **Use Deception and Share Warnings**: Decoy systems, covered in SCD-011-4, expose intruders early, and shared threat intelligence, covered in SCD-011-5, lets one organization's warning protect many others.

### 3. AI-Assisted Detection Under Human Judgment
Faster Signals, Careful Interpretation:

* **AI Sorts the Noise**: The internet is full of automated scanning, and AI can group millions of events to highlight the small number that look targeted at space systems.
* **Attackers Use AI Too**: One industry review reported more than 22,000 AI-assisted malware samples identified between February 2025 and February 2026, and detection models must also be protected from poisoning and evasion as described in NIST AI 100-2e2025.
* **Proposed Early Warning Rule**: AI may raise alerts, block obvious scanning sources, and suggest priorities, but declaring that an organization is being targeted, sharing intelligence externally, or changing mission operations is decided by qualified analysts.

### 4. Analysts Who Read the Early Signs
Human Insight at the Edge of the Network:

* **Context Turns Data Into Warning**: Only people who understand the mission, the technology, and current events can judge whether a scan is routine background noise or the start of a campaign.
* **Reducing Analysts Removes the Warning Line**: Organizations that cut security staff and rely only on automation may collect warnings that no one reads in time.
* **CISSP Frames the Work**: CISSP Domain 1 covers threat modeling and risk, Domain 6 covers assessment and vulnerability scanning, and Domain 7 covers monitoring, threat intelligence, and incident detection.

### 5. Conclusion
Reconnaissance is the stage at which attackers are most visible and defenders have the most options, and in the space sector it most often targets ground systems on Earth.

By mapping exposure, watching for probing, reviewing public information, using deception, sharing warnings, and keeping skilled analysts in charge of interpretation, the space community can build an early warning line that lets people respond calmly before harm occurs.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-011

## 早期警戒線 — 宇宙システムへの攻撃の前に、偵察を見つける

### サマリー・ダイジェスト
深刻な攻撃のほとんどは、静かな準備から始まります。外から見えるシステムを調べ上げ、公開されている情報を集め、防御を試すことです。2025年の脅威の状況についての報告は、宇宙分野を狙った407件の攻撃を確認しましたが、軌道上の衛星に当たったものは1件もなく、影響を受けたのは企業のIT環境、地上局、地上の利用者のモデムでした。これらはまさに、偵察が最初に行われる場所です。

SCD-011の本編である本論文は、宇宙システムの早期警戒線としての偵察の検知を紹介します。CISSPのドメイン1、6、7を適用し、露出の把握、スキャンの検知、公開情報の点検、おとり、情報共有がどう組み合わさるかを説明し、早期の警告が何を意味するかは、訓練を受けた分析担当者が判断しなければならない理由を示します。

---
### 1. 偵察の段階こそ動くべき時である理由
攻撃の前に、攻撃者を見る:

* **攻撃は準備の後に来る**: 攻撃者はふつう、行動する前に標的を決め、その技術を調べ、弱いところを探します。そのため、この段階を見つければ、守る側には穴をふさぐ時間ができます。
* **地上部分が玄関口**: 最近の宇宙分野への攻撃は、軌道上の衛星ではなく、地上局、企業のネットワーク、利用者の端末に影響を与えてきたため、これらのシステムへの偵察には特に注意が必要です。
* **早く見つけるほど費用が少ない**: 偵察の段階で攻撃者を止めれば、侵害への対応、システムの復旧、信頼の立て直しにかかる、ずっと大きな費用を避けられます。

### 2. 早期警戒線の5つの層
SCD-011シリーズの構成:

* **自分の露出を知る**: 攻撃者も同じ公開のスキャンの道具を使うため、組織は、SCD-011-1で述べるように、どの地上のシステムがインターネットから見えているかを把握します。
* **探りを見張り、公開の手がかりを集める**: SCD-011-2で扱うスキャンの傾向と、SCD-011-3で扱う公開の情報から漏れているものは、攻撃者がすでに何を知っているかを明らかにします。
* **おとりを使い、警告を分け合う**: SCD-011-4で扱うおとりのシステムは侵入者を早くあらわにし、SCD-011-5で扱う脅威情報の共有によって、ひとつの組織の警告が多くの組織を守ります。

### 3. 人の判断の下でのAIによる検知
より速い信号、慎重な読み解き:

* **AIが雑音をふるい分ける**: インターネットは自動のスキャンであふれており、AIは何百万もの出来事をまとめて、宇宙システムを狙っているように見える少数のものを浮かび上がらせられます。
* **攻撃者もAIを使う**: ある業界の振り返りは、2025年2月から2026年2月までに、AIを使ったマルウェアの検体が22,000以上見つかったと報告しています。検知のモデルも、NIST AI 100-2e2025が述べる汚染と回避から守らなければなりません。
* **早期警戒の規則（提案）**: AIは警報を出し、明らかなスキャンの発信元をブロックし、優先順位を提案してかまいません。しかし、組織が狙われているという判断、外部への情報の共有、ミッションの運用の変更は、有資格の分析担当者が決めます。

### 4. 早いしるしを読む分析担当者
ネットワークの端での人の洞察:

* **背景がデータを警告に変える**: スキャンがいつもの背景の雑音なのか、攻撃活動の始まりなのかは、ミッション、技術、最近の出来事を理解している人にしか判断できません。
* **分析担当者を減らすと警戒線がなくなる**: セキュリティの人員を削り、自動化だけに頼る組織は、誰も間に合うように読まない警告を集めるだけになるかもしれません。
* **CISSPが仕事の枠組みをつくる**: CISSPのドメイン1は脅威のモデル化とリスクを、ドメイン6は評価と脆弱性のスキャンを、ドメイン7は監視、脅威情報、インシデントの検知を扱います。

### 5. 結論
偵察は、攻撃者がもっとも見えやすく、守る側にもっとも多くの選択肢がある段階であり、宇宙分野ではそれが地上のシステムに向けられることがもっとも多いのです。

露出を把握し、探りを見張り、公開の情報を点検し、おとりを使い、警告を分け合い、そして技能のある分析担当者に読み解きを任せることで、宇宙の世界は、被害が起きる前に人が落ち着いて対応できる早期警戒線を築けます。
