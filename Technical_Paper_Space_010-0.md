# Koki's Technical Paper — Space Cyber Defense Series SCD-010

## The Stellar Choreography — Protecting the Integrity of Time, Position, and Formation Flight

### Summary Digest
Satellites, aircraft, ships, power grids, and financial networks all depend on accurate positioning, navigation, and timing (PNT). That dependence is now under open attack: an industry workgroup reported a 500% increase in GPS spoofing in 2024, with about 1,500 flights per day affected, while future orbital data centers will fly dozens of satellites only a few hundred meters apart.

This main paper of SCD-010 introduces the security of time, position, and formation flight. It applies CISSP Domains 3, 4, and 7, explains how cryptographic authentication such as Galileo OSNMA and checks based on physical laws work together, and shows why trained people must remain responsible for decisions when navigation data cannot be trusted.

---
### 1. Why Time and Position Are Security Assets
The Hidden Rhythm Behind Modern Infrastructure:

* **PNT Is an Invisible Utility**: U.S. Executive Order 13905, signed on February 12, 2020, describes space-based PNT services as a largely invisible utility on which technology and critical infrastructure depend.
* **Wrong Time Breaks Systems Quietly**: Satellite constellations, ground stations, and data centers rely on synchronized clocks to schedule links, order logs, and validate cryptographic certificates, so manipulated time can cause failures that look like ordinary faults.
* **Wrong Position Breaks Formations**: Satellites that fly in close formation must know their relative positions precisely, and false navigation data could push them toward unsafe distances or waste limited propellant.

### 2. The Threat Landscape in 2026
From Occasional Interference to Daily Pressure:

* **Spoofing Has Become Routine**: The 2024 GPS Spoofing Workgroup reported an average of about 1,500 spoofed flights per day, compared with 300 in the first half of 2024.
* **Regional Interference Is Persistent**: A joint report by Sweden, Finland, Estonia, Lithuania, Latvia, and Poland found that about 122,600 flights in northern Europe were affected by satellite navigation interference from January to April 2025.
* **Close Formations Raise the Stakes**: Concepts for orbital data centers describe clusters of 81 satellites within a 1 km radius at separations of about 100 to 200 meters, where navigation errors leave little room for recovery.

### 3. A Layered Defense With AI and Human Approval
Authentication, Cross-Checks, and Clear Authority:

* **Authenticate the Navigation Message**: Galileo OSNMA, declared operational on July 24, 2025, lets receivers verify that ephemeris and clock data come from the Galileo system and have not been modified.
* **Check Against Physics and Other Sources**: Positions and times are compared with orbital mechanics, inertial sensors, other constellations, and terrestrial systems, so a single false signal cannot redefine reality.
* **Proposed Navigation Trust Rule**: AI may detect navigation anomalies and switch a system to backup sources, but declaring a spoofing incident, changing a formation, or performing a maneuver based on disputed data is approved by a qualified operator, consistent with the attention NIST AI 100-2e2025 gives to manipulated inputs.

### 4. People Who Keep the Rhythm
A Workforce That Understands Both Physics and Security:

* **PNT Security Needs Mixed Skills**: Protecting time and position requires people who understand radio signals, orbital mechanics, cryptography, and incident response, a combination that cannot be replaced by a single automated tool.
* **CISSP Provides the Framework**: CISSP Domain 3 covers cryptography and secure architecture, Domain 4 covers communication and network security, and Domain 7 covers monitoring and incident response, all of which apply to PNT defense.
* **Experience Prevents Overreaction**: Experienced operators can tell the difference between natural interference, equipment faults, and deliberate attacks, preventing unnecessary maneuvers and false alarms.

### 5. Conclusion
Time and position are the rhythm that keeps satellites, aircraft, and infrastructure in step, and that rhythm is now a daily target for spoofing and jamming.

By combining authenticated signals, cross-checks based on physical laws, AI that detects anomalies quickly, and skilled people who make the final decisions, the space community can keep this choreography safe and build a future where every satellite knows where and when it is with confidence.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-010

## 星々の振り付け — 時刻、位置、編隊飛行の完全性を守る

### サマリー・ダイジェスト
衛星、航空機、船、電力網、金融のネットワークは、どれも正確な測位・航法・時刻（PNT）に頼っています。その依存が、今は公然と攻撃されています。業界の作業部会は、2024年にGPSのなりすまし（スプーフィング）が500%増え、1日に約1,500便が影響を受けたと報告しました。一方、将来の軌道上のデータセンターでは、何十機もの衛星がわずか数百メートルの間隔で飛ぶことになります。

SCD-010の本編である本論文は、時刻、位置、編隊飛行のセキュリティを紹介します。CISSPのドメイン3、4、7を適用し、Galileo OSNMAのような暗号による認証と、物理法則にもとづく確認がどう組み合わさるかを説明します。そして、航法のデータが信頼できないときに、訓練を受けた人が判断の責任を持ち続けなければならない理由を示します。

---
### 1. 時刻と位置がセキュリティの資産である理由
現代のインフラを支える見えないリズム:

* **PNTは見えない公共インフラ**: 2020年2月12日に署名された米国の大統領令13905は、宇宙からのPNTサービスを、技術と重要インフラが頼る、ほとんど目に見えない公共のサービスだと述べています。
* **間違った時刻は静かにシステムを壊す**: 衛星コンステレーション、地上局、データセンターは、通信の予定を組み、ログの順番を決め、暗号の証明書を確かめるために、そろった時計に頼っています。そのため、操作された時刻は、普通の故障に見える障害を引き起こすことがあります。
* **間違った位置は編隊を壊す**: 密集した編隊で飛ぶ衛星は、お互いの位置を正確に知っていなければなりません。偽の航法データは、衛星を危険な距離に近づけたり、限られた推進剤をむだにさせたりするおそれがあります。

### 2. 2026年の脅威の状況
ときどきの妨害から、毎日の圧力へ:

* **なりすましは日常になった**: 2024年のGPSなりすまし作業部会は、2024年前半の1日300便に対し、平均で1日約1,500便がなりすましを受けたと報告しました。
* **地域的な妨害が続いている**: スウェーデン、フィンランド、エストニア、リトアニア、ラトビア、ポーランドの共同報告は、2025年1月から4月に、北ヨーロッパで約122,600便が衛星航法への妨害の影響を受けたとしています。
* **密集した編隊では危険が大きくなる**: 軌道上のデータセンターの構想では、81機の衛星が半径1kmの中に、約100〜200メートルの間隔で集まります。そこでは航法の誤りから立ち直る余裕がほとんどありません。

### 3. AIと人の承認による多層の防御
認証、照らし合わせ、はっきりした権限:

* **航法メッセージを認証する**: 2025年7月24日に運用開始が宣言されたGalileo OSNMAでは、受信機が、軌道と時計のデータがGalileoのシステムから来たもので、書き換えられていないことを確かめられます。
* **物理法則やほかの情報源と照らし合わせる**: 位置と時刻を、軌道力学、慣性センサー、ほかの衛星測位システム、地上のシステムと比べます。そうすれば、ひとつの偽の信号が現実を書き換えることはできません。
* **航法の信頼の規則（提案）**: AIは航法の異常を見つけ、システムを予備の情報源に切り替えてかまいません。しかし、なりすましの事案の宣言、編隊の変更、疑わしいデータにもとづく軌道の変更は、有資格の運用担当者が承認します。これは、NIST AI 100-2e2025が操作された入力に注意を払っていることと同じ考え方です。

### 4. リズムを守る人々
物理とセキュリティの両方を理解する人材:

* **PNTのセキュリティには幅広い技能が要る**: 時刻と位置を守るには、電波、軌道力学、暗号、インシデント対応を理解する人が必要です。この組み合わせは、ひとつの自動化ツールでは置き換えられません。
* **CISSPが枠組みを与える**: CISSPのドメイン3は暗号と安全な設計を、ドメイン4は通信とネットワークのセキュリティを、ドメイン7は監視とインシデント対応を扱い、そのすべてがPNTの防御に当てはまります。
* **経験が行き過ぎた反応を防ぐ**: 経験のある運用担当者は、自然の電波障害、機器の故障、意図的な攻撃を見分けられ、不要な軌道変更や誤った警報を防ぎます。

### 5. 結論
時刻と位置は、衛星、航空機、インフラの歩調をそろえるリズムであり、そのリズムは今、毎日のようになりすましと妨害の標的になっています。

認証された信号、物理法則にもとづく照らし合わせ、異常を素早く見つけるAI、そして最終判断を下す技能のある人々を組み合わせることで、宇宙の世界はこの振り付けを安全に保ち、すべての衛星が自分の場所と時刻を自信をもって知ることができる未来を築けます。
