# Koki's Technical Paper — Space Cyber Defense Series SCD-019

## The Last Resilience — Preparing for Solar Storms and Cyberattacks at the Same Time

### Summary Digest
Space systems must survive nature as well as attackers. Between May 10 and 12, 2024, Earth experienced its largest geomagnetic storm in more than 20 years, which caused the largest mass migration of satellites in history as operators maneuvered to counter atmospheric drag. Severe storms followed in January, June, and November 2025, and the U.S. Geological Survey has warned that more severe storms remain likely in the years after the solar maximum. If a cyberattack struck during such a storm, operators would face two crises at once, with less time, less data, and less margin for error.

This main paper of SCD-019 introduces resilience for the worst case, when space weather and cyber threats overlap. It applies CISSP Domains 1, 7, and 3, explains simplified safe modes, protected backups, hibernation, and verified restart, and shows why calm, experienced people are the last line of resilience.

---
### 1. Why Space Weather and Cyber Threats Must Be Planned Together
Two Storms, One Response Team:

* **Storms Increase Workload and Confusion**: During the 2024 storm, sudden drag disrupted orbit predictions, and experts noted that conjunction assessment had to be restarted after mass maneuvers, a time when operators are already stretched.
* **Natural Effects Can Hide Attacks**: Radiation errors, communication outages, and navigation degradation caused by storms look similar to some cyber effects, making it harder to recognize malicious activity.
* **Attackers May Exploit Chaos**: Adversaries could choose a period of severe space weather to act, knowing that defenders are distracted and systems are already under stress.

### 2. Four Layers of Last Resilience
A Structure for the SCD-019 Series:

* **Surviving Dual Storms**: SCD-019-1 explains how to prepare for simultaneous space weather and cyber incidents.
* **Simplify and Preserve**: SCD-019-2 describes minimal safe-mode logic, and SCD-019-3 explains offline reference images and protected backups.
* **Sleep and Restart Safely**: SCD-019-4 covers deep hibernation for survival, and SCD-019-5 explains verified restart sequences.

### 3. AI Support Under Human Leadership in Crises
Better Forecasts, Careful Decisions:

* **AI Improves Forecasting and Triage**: AI can combine space weather data with telemetry and security alerts to estimate whether anomalies are natural or suspicious.
* **AI Can Be Confused in Extreme Conditions**: Models trained on normal conditions may fail during rare storms, and they can be manipulated, consistent with NIST AI 100-2e2025, so their outputs are treated as advice during crises.
* **Proposed Dual-Crisis Rule**: AI may recommend protective configurations and prioritize alerts, but placing fleets in safe mode, attributing anomalies to attacks, or restarting systems after a storm is decided by qualified operators and incident leaders.

### 4. Calm People as the Final Layer
Experience That Holds Steady:

* **Crisis Experience Is Precious**: Operators who have lived through storms and incidents know how systems behave under stress and can make steady decisions when automation struggles.
* **Rested, Rotated Teams Matter**: Long crises require enough trained staff to work in shifts, so cutting teams to minimum size increases risk in exactly the moments that matter most.
* **CISSP Supports Resilience**: CISSP Domain 1 covers business continuity planning, Domain 7 covers disaster recovery and incident response, and Domain 3 covers resilient architecture.

### 5. Conclusion
The last resilience is the ability to survive when nature and attackers strike together, with limited information and little time.

By planning for dual crises, simplifying safe modes, protecting backups, preparing for hibernation and verified restart, using AI as an advisor, and keeping experienced, rested teams ready, the space community can make sure that even the worst day becomes one that systems and people can recover from.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-019

## 最後の回復力 — 太陽嵐とサイバー攻撃が同時に来たときへの備え

### サマリー・ダイジェスト
宇宙システムは、攻撃者だけでなく自然にも耐えなければなりません。2024年5月10日から12日、地球は20年以上ぶりの大きな磁気嵐に見舞われ、運用者たちが大気の抵抗に対抗して軌道を変えたため、歴史上最大の衛星の「大移動」が起きました。2025年の1月、6月、11月にも強い嵐が続き、米国地質調査所は、太陽活動のピークを過ぎた後の数年も、強い嵐が起きる可能性は高いと警告しています。もしこうした嵐の最中にサイバー攻撃が起きたら、運用者は、時間も、データも、間違いの余裕も少ない中で、2つの危機に同時に向き合うことになります。

SCD-019の本編である本論文は、宇宙天気とサイバーの脅威が重なる最悪の場合のための回復力を紹介します。CISSPのドメイン1、7、3を適用し、簡単にしたセーフモード、守られたバックアップ、休眠、確かめられた再起動を説明し、落ち着いた経験のある人々こそが、最後の回復力であることを示します。

---
### 1. 宇宙天気とサイバーの脅威を一緒に計画しなければならない理由
2つの嵐、ひとつの対応チーム:

* **嵐は仕事量と混乱を増やす**: 2024年の嵐では、急な大気の抵抗が軌道の予測を乱し、専門家は、大量の軌道の変更の後に接近の評価をやり直さなければならなかったと指摘しました。それは運用者がすでに手いっぱいの時です。
* **自然の影響が攻撃を隠すことがある**: 嵐による放射線の誤り、通信の途切れ、航法の乱れは、一部のサイバーの影響と似て見えるため、悪意のある活動に気づきにくくなります。
* **攻撃者は混乱を利用するかもしれない**: 攻撃者は、守る側の気がそれていて、システムがすでに負担を受けていると知って、強い宇宙天気の時期を選んで動くかもしれません。

### 2. 最後の回復力の4つの層
SCD-019シリーズの構成:

* **2つの嵐を生き延びる**: SCD-019-1は、宇宙天気とサイバーのインシデントが同時に起きる場合にどう備えるかを説明します。
* **簡単にし、守り残す**: SCD-019-2は最小限のセーフモードの仕組みを、SCD-019-3はオフラインの基準のイメージと守られたバックアップを説明します。
* **安全に眠り、安全に再起動する**: SCD-019-4は生き残るための深い休眠を、SCD-019-5は確かめられた再起動の順序を扱います。

### 3. 危機の中での、人が率いるAIの支援
よりよい予報、慎重な判断:

* **AIが予報と振り分けをよくする**: AIは、宇宙天気のデータをテレメトリやセキュリティの警報と組み合わせ、異常が自然のものか疑わしいものかを見積もれます。
* **極端な条件ではAIが混乱することがある**: 普段の条件で学習したモデルは、まれな嵐の間は失敗することがあり、操作されることもあります。これはNIST AI 100-2e2025と同じ趣旨です。そのため、危機の間は、その出力を助言として扱います。
* **2つの危機の規則（提案）**: AIは身を守るための設定を勧め、警報に優先順位を付けてかまいません。しかし、機体の群れをセーフモードに入れること、異常を攻撃によるものと判断すること、嵐の後にシステムを再起動することは、有資格の運用担当者とインシデントの責任者が決めます。

### 4. 最後の層としての、落ち着いた人々
しっかりと踏みとどまる経験:

* **危機の経験は貴重**: 嵐やインシデントを経験してきた運用担当者は、負担がかかったときにシステムがどうふるまうかを知っており、自動化がうまく働かないときにも、しっかりした判断を下せます。
* **休み、交代できるチームが大切**: 長い危機には、交代で働ける十分な訓練を受けた人員が必要です。そのため、チームを最小限まで削ると、まさにいちばん大切な時にリスクが高まります。
* **CISSPが回復力を支える**: CISSPのドメイン1は事業継続の計画を、ドメイン7は災害復旧とインシデント対応を、ドメイン3は回復力のある設計を扱います。

### 5. 結論
最後の回復力とは、限られた情報と少ない時間の中で、自然と攻撃者が一緒に襲ってきても生き延びる力です。

2つの危機に備えて計画し、セーフモードを簡単にし、バックアップを守り、休眠と確かめられた再起動に備え、AIを助言役として使い、経験のある、休息のとれたチームを備えておくことで、宇宙の世界は、最悪の日でさえ、システムと人が立ち直れる日にできます。
