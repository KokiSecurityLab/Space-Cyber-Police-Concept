# Koki's Technical Paper — Space Cyber Defense Series SCD-005

## The Cosmic Sweeper — Space Debris, Orbital Denial of Service, and Trustworthy Collision Avoidance Under Human Command

### Summary Digest
Low Earth orbit is becoming crowded: ESA's 2026 Space Environment Report counted more than 300 launches in 2025 placing over 4,000 new payloads into orbit, and Starlink satellites alone performed 207,152 collision-avoidance maneuvers between December 2025 and May 2026.

This paper applies CISSP Domains 1 and 7 to debris and orbital denial of service, treating collision-avoidance data, maneuver commands, and debris-creating events as security concerns, and it argues that automated avoidance must be protected from manipulation while people keep authority over decisions that could create new debris.

---
### 1. Debris as a Shared Security Problem
Why Orbital Safety and Cybersecurity Meet:

* **One Event Can Threaten Everyone**: Russia's destructive anti-satellite test in November 2021 generated more than 1,500 pieces of trackable debris and is likely to produce hundreds of thousands of smaller pieces, putting every operator in that region at risk.
* **Avoidance Has Become Constant**: Each Starlink satellite now performs dozens of avoidance maneuvers a year, so the safety of the orbit depends on accurate tracking data and reliable automated maneuver systems.
* **Data Integrity Becomes Physical Safety**: If conjunction warnings, tracking data, or maneuver commands are falsified, satellites may move into danger or fail to move away from it, turning a data attack into a collision risk.

### 2. Protecting the Collision-Avoidance Chain
From Tracking Data to Thruster Firing:

* **Authenticate Tracking and Warning Data**: Conjunction messages and orbit data from services such as the U.S. Traffic Coordination System for Space are received over authenticated channels and cross-checked against independent sources before they trigger maneuvers.
* **Check Maneuvers Against the Wider Picture**: Before a satellite moves, its new path is screened against all known objects, so that avoiding one hazard does not create a new conjunction with another.
* **Watch for Patterns of Manipulation**: A sudden increase in warnings for one operator, or warnings that independent trackers cannot confirm, may indicate spoofed data intended to waste propellant or push satellites into unsafe orbits.

### 3. Automation With Human Authority
Where AI Helps and Where People Decide:

* **AI Is Essential at This Scale**: Hundreds of thousands of maneuvers a year cannot be planned by hand, so AI and automated systems assess risk and plan routine avoidance far faster than people could.
* **Automated Avoidance Is a Target**: Attackers could poison the data that risk models learn from or craft inputs that make dangerous situations appear safe, the poisoning and evasion risks described in NIST AI 100-2e2025, so automated decisions stay within fixed safety limits.
* **Proposed Debris-Risk Rule**: Routine avoidance maneuvers may run automatically within preapproved limits, but any action that could create debris, such as close approaches to other objects, deliberate deorbiting near crewed stations, or overriding a collision warning, requires approval from a qualified flight dynamics lead.

### 4. The People Who Keep Orbits Clean
Flight Dynamics, Tracking, and Shared Stewardship:

* **Space Safety Depends on Skilled Analysts**: Flight dynamics engineers, tracking specialists, and security analysts interpret warnings, resolve conflicting data, and coordinate with other operators, work that requires human judgment and cooperation.
* **Many Contributors Protect a Shared Resource**: Clean orbits benefit everyone, so training analysts in many countries and organizations, rather than relying on a few large operators or automated systems, strengthens global safety.
* **CISSP Frames Safety as Risk Management**: CISSP Domain 1 helps leaders treat debris and collision risk as business and mission risk, and Domain 7 supports the operational discipline needed for continuous avoidance.

### 5. Conclusion
As orbits fill with satellites and debris, collision avoidance has become a continuous, automated process whose data and commands must be protected as carefully as any critical system.

Authenticated tracking data, maneuver screening, AI that operates within fixed safety limits, and qualified people who decide on any action that could create debris together keep the cosmic sweeper working for everyone.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-005

## 宇宙の掃除人 — 宇宙ごみ、軌道上のサービス妨害、および人の指揮のもとでの信頼できる衝突回避

### サマリー・ダイジェスト
低軌道は混み合ってきています。ESAの2026年版「宇宙環境報告書」は、2025年に300回を超える打ち上げで4,000基以上の新しい衛星などが軌道に投入されたと数えました。Starlinkの衛星だけでも、2025年12月から2026年5月までに207,152回の衝突回避の軌道変更を行いました。

本論文はCISSPのドメイン1と7を宇宙ごみと軌道上のサービス妨害に適用し、衝突回避のデータ、軌道変更の指令、ごみを生む出来事を、セキュリティの問題として扱います。そして、自動の衝突回避を操作から守る一方で、新しいごみを生み得る判断については人が権限を持ち続けるべきだと論じます。

---
### 1. みんなのセキュリティ問題としての宇宙ごみ
軌道の安全とサイバーセキュリティが交わる理由:

* **1つの出来事が皆を脅かす**: 2021年11月にロシアが行った衛星を破壊する兵器の実験は、追跡できる宇宙ごみを1,500個以上生み出し、さらに何十万もの小さなごみを生む恐れがあります。その領域にいるすべての事業者が危険にさらされました。
* **回避は絶え間ない作業になった**: Starlinkの衛星は今や1基あたり年に何十回も回避の軌道変更を行っています。そのため軌道の安全は、正確な追跡データと信頼できる自動の軌道変更システムにかかっています。
* **データの完全性が物理的な安全になる**: 接近の警告、追跡データ、軌道変更の指令が偽造されると、衛星は危険な場所へ動いたり、危険から離れられなかったりします。データへの攻撃が衝突のリスクに変わるのです。

### 2. 衝突回避の流れを守る
追跡データから推進器の噴射まで:

* **追跡と警告のデータを認証する**: 米国の宇宙交通調整システム（TraCSS）などから届く接近の通知と軌道のデータは、認証された経路で受け取り、軌道変更のきっかけにする前に独立した情報源と照合します。
* **軌道変更を全体像と照らし合わせる**: 衛星が動く前に、新しい経路をすべての既知の物体と照合します。1つの危険を避けたことで、別の物体との新しい接近を生まないためです。
* **操作のパターンを見張る**: ある事業者への警告が急に増えたり、独立した追跡者が確認できない警告が届いたりするときは、推進剤を無駄にさせたり、衛星を危険な軌道に追いやったりするための偽のデータである可能性があります。

### 3. 人の権限のもとでの自動化
AIが助ける場面と、人が決める場面:

* **この規模ではAIが欠かせない**: 年に何十万回もの軌道変更を手で計画することはできません。そのためAIと自動のシステムが、人よりはるかに速くリスクを評価し、日常の回避を計画します。
* **自動の回避は標的になる**: 攻撃者は、リスクのモデルが学ぶデータを汚染したり、危険な状況を安全に見せる入力を作ったりするかもしれません。これはNIST AI 100-2e2025が示す汚染と回避のリスクです。そのため、自動の判断は固定の安全の限界の内側にとどめます。
* **ごみのリスクについての規則（提案）**: 日常的な回避の軌道変更は、事前に承認された範囲内で自動で行ってかまいません。しかし、ほかの物体への接近、有人の宇宙ステーションの近くでの意図的な軌道離脱、衝突の警告を無視することなど、ごみを生み得る行動には、有資格の軌道力学の責任者の承認を必須とします。

### 4. 軌道をきれいに保つ人々
軌道力学、追跡、および共有の管理責任:

* **宇宙の安全は熟練の分析担当者にかかっている**: 軌道力学の技術者、追跡の専門家、セキュリティの分析担当者は、警告を読み解き、食い違うデータを整理し、ほかの事業者と調整します。これは人の判断と協力を必要とする仕事です。
* **多くの担い手が共有の資源を守る**: きれいな軌道は皆のためになります。少数の大きな事業者や自動のシステムに頼るのではなく、多くの国や組織で分析担当者を育てることが、世界全体の安全を強くします。
* **CISSPが安全をリスク管理として捉える**: CISSPのドメイン1は、経営者が宇宙ごみと衝突のリスクを事業とミッションのリスクとして扱う助けとなり、ドメイン7は絶え間ない回避に必要な運用の規律を支えます。

### 5. 結論
軌道が衛星とごみで満ちていくにつれ、衝突回避は絶え間なく続く自動の作業となり、そのデータと指令は、どんな重要なシステムとも同じくらい注意深く守らなければなりません。

認証された追跡データ、軌道変更の照合、固定の安全の限界の中で動くAI、そしてごみを生み得るあらゆる行動を決める有資格の人がそろって、宇宙の掃除人は皆のために働き続けます。
