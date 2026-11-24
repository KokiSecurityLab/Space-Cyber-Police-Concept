# Koki's Technical Paper — Space Cyber Defense Series SCD-003

## The Eternal Guardian — Securing Orbital Power Systems and Servicing Robots Where Cyber Commands Become Physical Motion

### Summary Digest
Orbital infrastructure is becoming physical and serviceable: Northrop Grumman's Mission Extension Vehicle docked with the Intelsat 901 satellite in February 2020 and returned it to service, and planned orbital AI clusters will depend on large solar arrays, power controllers, and robotic arms that act on software commands.

This paper applies CISSP Domains 3 and 7 to treat power and robotics as cyber-physical systems, where a malicious command can drain energy, damage hardware, or cause a collision, and it requires that AI-assisted control be bounded by physical safety limits and approved by qualified people for any irreversible motion.

---
### 1. When Data Turns Into Motion
Why Power and Robotics Raise the Stakes:

* **Energy Is the First Dependency**: Every computer, radio, and thruster on a satellite depends on its solar arrays, batteries, and power controller, so an attacker who disrupts power management can disable a spacecraft without touching its data.
* **Servicing Brings Machines Into Contact**: Life-extension vehicles, inspection craft, and robotic arms operate within meters of other satellites, so a manipulated command or navigation input could turn a repair mission into a collision.
* **Cyber-Physical Lessons Already Exist on Earth**: NIST SP 800-82 Revision 3, the 2023 guide to operational technology security, shows that industrial control systems need safety interlocks, segmentation, and monitoring that differ from ordinary IT, and orbital robots and power systems share these needs.

### 2. Designing Physical Safety Into the System
Interlocks, Segmentation, and Command Validation:

* **Hardware Interlocks That Software Cannot Override**: Battery protection, current limits, and arm-motion limits are enforced in independent hardware, so even a fully compromised flight computer cannot drive a battery into damage or swing an arm beyond a safe envelope.
* **Separate Control Paths for Power and Payload**: Power management and robotic control run on segmented networks with their own authentication, preventing a compromised payload or AI workload from issuing power or motion commands.
* **Validate Every Command Against Physics**: Before execution, each command is checked against the current orbit, attitude, battery state, and proximity data, and any command that would violate a physical limit is rejected and reported.

### 3. AI in the Loop, Humans on the Switch
Autonomy for Speed, People for Irreversible Actions:

* **AI Manages Routine Energy and Motion**: AI can balance power loads, predict battery health, and plan fine arm movements faster than ground operators, especially during short communication windows.
* **Learning Systems Must Not Learn Unsafe Behavior**: Training data and control policies are protected against poisoning, following NIST AI 100-2e2025, and every model update is tested in simulation before upload because a single bad policy can cause physical damage.
* **Proposed Irreversible-Action Rule**: Docking, capture, release, propellant transfer, and deliberate power shutdown of a payload require confirmation from a qualified operator, with a second person reviewing any action that could affect another operator's spacecraft.

### 4. The People Who Keep Machines Safe
Engineers, Operators, and Shared Responsibility:

* **Cyber-Physical Security Needs Hybrid Skills**: Protecting orbital power and robotics requires electrical engineers, robotics specialists, control-system experts, and security professionals working together, a team that AI supports but cannot replace.
* **Experience Prevents Accidents**: Operators who have run real docking and power-recovery procedures recognize warning signs that are absent from training data, so organizations that cut experienced staff in favor of automation lose a key layer of safety.
* **CISSP for Physical and Logical Controls**: CISSP Domain 3 covers secure design principles and physical security together, giving engineers and security teams a shared basis for deciding where hardware interlocks, software checks, and human approvals belong.

### 5. Conclusion
As satellites gain robotic arms, serviceable components, and power systems that feed orbital AI, cyber attacks gain the ability to cause physical harm, and defenses must be built into hardware, network design, and command validation.

AI can operate these systems at the speed space requires, while qualified people approve every irreversible motion, and together they form an eternal guardian that keeps the energy flowing and the machines safe.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-003

## 永遠の守護者 — サイバー指令が物理的な動きに変わる軌道上の電力システムと保守ロボットの保護

### サマリー・ダイジェスト
軌道上のインフラは、物理的に手を加えて保守できるものになりつつあります。Northrop Grummanの寿命延長機MEV-1は2020年2月に衛星Intelsat 901とドッキングし、運用に復帰させました。計画中の軌道上のAIクラスタも、大きな太陽電池パネル、電力制御装置、そしてソフトウェアの指令で動くロボットアームに頼ることになります。

本論文はCISSPのドメイン3と7を適用し、電力とロボットを「サイバーフィジカルシステム」として扱います。そこでは、悪意のある指令がエネルギーを奪い、機器を壊し、衝突を引き起こし得ます。そのため、AIを活用した制御を物理的な安全の限界の内側にとどめ、元に戻せない動作には有資格の人の承認を必須とします。

---
### 1. データが動きに変わるとき
電力とロボットがリスクを高める理由:

* **最初の依存先はエネルギー**: 衛星のあらゆるコンピューター、無線機、推進装置は、太陽電池パネル、バッテリー、電力制御装置に依存しています。そのため、電力管理を乱す攻撃者は、データに触れることなく宇宙機を機能停止にできます。
* **保守が機械同士を接触させる**: 寿命延長機、点検機、ロボットアームは、ほかの衛星から数メートルの距離で動作します。操作された指令や航法の入力によって、修理のミッションが衝突に変わる恐れがあります。
* **地上にはすでに教訓がある**: 運用技術（OT）のセキュリティについての2023年の指針であるNIST SP 800-82 第3版は、産業制御システムには通常のITとは異なる安全インターロック、ネットワーク分離、監視が必要だと示しています。軌道上のロボットと電力システムにも同じことが当てはまります。

### 2. 物理的な安全を設計に組み込む
インターロック、分離、および指令の検証:

* **ソフトウェアでは解除できないハードウェアのインターロック**: バッテリーの保護、電流の上限、アームの動作範囲の制限は独立したハードウェアで守ります。たとえ飛行用コンピューターが完全に乗っ取られても、バッテリーを損傷させたり、アームを安全な範囲の外へ振り回したりはできません。
* **電力とペイロードの制御経路を分ける**: 電力管理とロボットの制御は、それぞれ独自の認証を持つ分離されたネットワークで動かします。乗っ取られたペイロードやAIの処理が、電力や動作の指令を出せないようにするためです。
* **すべての指令を物理法則と照らし合わせる**: 実行の前に、各指令を現在の軌道、姿勢、バッテリーの状態、近くの物体のデータと照合します。物理的な限界を超える指令は拒否し、報告します。

### 3. AIは制御の中に、スイッチは人の手に
速さのための自律と、元に戻せない動作のための人:

* **日常的なエネルギーと動作はAIが管理する**: AIは、とくに短い通信時間の間に、地上の運用者よりも速く電力の負荷を調整し、バッテリーの状態を予測し、アームの細かな動きを計画できます。
* **学習するシステムに危険なふるまいを覚えさせない**: 学習データと制御方針は、NIST AI 100-2e2025に沿って汚染から守ります。1つの悪い方針が物理的な損傷を起こし得るため、モデルの更新はすべて、送信する前にシミュレーションで試験します。
* **元に戻せない動作の規則（提案）**: ドッキング、捕獲、切り離し、推進剤の移送、ペイロードの意図的な電源遮断には有資格の運用者の確認を必須とし、他の事業者の宇宙機に影響し得る動作は、さらにもう1人が確認します。

### 4. 機械の安全を守る人々
技術者、運用者、および共有される責任:

* **サイバーフィジカルのセキュリティには複合的な技能が必要**: 軌道上の電力とロボットを守るには、電気技術者、ロボット工学の専門家、制御システムの専門家、セキュリティの専門家が力を合わせる必要があります。AIはこのチームを支えますが、置き換えることはできません。
* **経験が事故を防ぐ**: 実際のドッキングや電力の復旧の手順を経験した運用者は、学習データにない危険の兆しに気づきます。自動化を理由に経験のある人員を削る組織は、安全の重要な層を失います。
* **物理的な統制と論理的な統制のためのCISSP**: CISSPのドメイン3は、安全な設計の原則と物理的なセキュリティをあわせて扱います。それにより技術者とセキュリティチームは、ハードウェアのインターロック、ソフトウェアの確認、人の承認をそれぞれどこに置くべきかを、共通の基盤の上で決められます。

### 5. 結論
衛星がロボットアーム、保守できる部品、軌道上のAIに電力を送るシステムを備えるにつれて、サイバー攻撃は物理的な被害を起こす力を持つようになります。防御は、ハードウェア、ネットワーク設計、指令の検証に組み込まなければなりません。

AIは宇宙が求める速さでこれらのシステムを動かし、有資格の人は元に戻せないすべての動作を承認します。両者がそろって初めて、エネルギーを流し続け、機械を安全に保つ「永遠の守護者」となります。
