# Koki's Technical Paper — Space Cyber Defense Series SCD-001-4

## Mitigation Over Perfect Prevention — Assume-Breach Design, Root-of-Trust Recovery, and Learning Loops for Systems No Technician Can Reach

### Summary Digest
No defense prevents every attack, and in orbit the cost of that truth is higher because, as reporting on Google's Project Suncatcher has emphasized, failed parts cannot be replaced by a technician and radiation can flip bits in memory, so a system that only knows how to block collapses at the first breach it cannot undo.

Applying CISSP Domain 7 and the protect, detect, and recover model of NIST SP 800-193, this paper designs orbital AI systems to contain damage, recover from a hardware root of trust, and learn from every incident, with AI accelerating recovery and humans approving each step that cannot be reversed.

---
### 1. The Trap of the Perfect Wall
Why Prevention Alone Is Fragile:

* **Assumed Invulnerability Hides Weak Recovery**: Teams confident that attackers cannot enter often have no tested plan for when they do, so a single successful intrusion through a zero-day flaw or a deceived operator becomes a mission-ending failure.
* **Space Removes the Usual Safety Nets**: A ground data center can send staff to replace a disk or reinstall a server, while a satellite must recover remotely, so every recovery path has to be built and proven before launch.
* **Faults and Attacks Look Alike at First**: A radiation-induced bit flip, a failing component, and malicious tampering can produce similar symptoms, so the response must contain the problem safely before its cause is known.

### 2. Designing for Containment and Recovery
Assume-Breach Architecture for Orbital Systems:

* **Segmentation That Limits Spread**: Payload computing, flight control, and communications run in isolated domains with strictly defined interfaces, so a compromise of an AI workload cannot reach the systems that keep the spacecraft safe.
* **Hardware Root of Trust and Verified Boot**: Each node starts only from firmware and software whose signatures are checked by a protected root of trust, and keeps a known-good image to which it can return, as NIST SP 800-193 describes for platform firmware resiliency.
* **Graceful Degradation**: When a node is isolated or rebuilt, its tasks move to healthy nodes or pause in a safe state, so the constellation continues its essential mission at reduced capacity instead of failing entirely.

### 3. Recovery With AI Speed and Human Approval
Fast Containment, Deliberate Restoration:

* **AI Detects and Proposes**: Defensive AI compares node behavior with baselines, isolates clearly anomalous workloads within pre-approved limits, and proposes a recovery plan with the evidence behind it.
* **Humans Approve Irreversible Steps**: Wiping a node, rotating cryptographic keys across a constellation, or reloading flight software is approved by a qualified operator, because these actions cannot be undone and can endanger the mission if the diagnosis is wrong.
* **Restore From Trusted State, Then Reconnect**: Recovered nodes are rebuilt from signed images, checked for integrity, and returned to service only after the cause is understood, so the attacker is not restored along with the system.

### 4. Learning Loops and the People Who Run Them
Post-Incident Review, Shared Lessons, and Workforce Investment:

* **Every Incident Improves the Design**: A blameless review after each event records what happened, how quickly it was contained, and which control failed, and the resulting changes are tracked to completion rather than filed away.
* **Shared Lessons Across the Industry**: Operators share anonymized findings through bodies such as the Space Information Sharing and Analysis Center, so one organization's recovery becomes every organization's prevention.
* **Recovery Skill Is Human Capital**: The ability to diagnose an unfamiliar failure and restore a remote system safely grows through experience and practice, so keeping and training skilled engineers, rather than replacing them with automation, is what makes resilient design work when it is tested.

### 5. Conclusion
Perfect prevention is an illusion, and in orbit, where no technician can be sent and radiation adds its own faults, the decisive capability is the speed and safety with which a system contains damage and returns to a trusted state.

Segmented design, recovery from a hardware root of trust, AI that detects and proposes, and CISSP-qualified people who approve irreversible actions and learn from each incident make orbital AI systems strong not because they never fail but because they always recover.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-001-4

## 完全な防止より緩和を — 侵害を前提とした設計、信頼の基点からの復旧、および技術者が行けないシステムのための学習の循環

### サマリー・ダイジェスト
あらゆる攻撃を防げる防御は存在せず、軌道上ではその代償がさらに大きくなります。GoogleのProject Suncatcherについての報道が強調しているように、故障した部品を技術者が交換することはできず、放射線はメモリのビットを反転させ得るため、遮断することしか知らないシステムは、元に戻せない最初の侵害で崩れてしまいます。

本論文は、CISSPのドメイン7と、NIST SP 800-193の保護・検知・復旧のモデルを適用し、軌道上のAIシステムを、被害を封じ込め、ハードウェアの信頼の基点から復旧し、あらゆるインシデントから学ぶように設計します。AIが復旧を速め、取り消せない各段階は人間が承認します。

---
### 1. 完璧な壁という落とし穴
防止だけでは脆い理由:

* **難攻不落の思い込みが隠す弱い復旧**: 攻撃者は入れないと確信しているチームは、入られたときの試験済みの計画を持たないことが多く、ゼロデイの欠陥やだまされた運用担当者を通じた一度の侵入が、ミッションを終わらせる失敗になります。
* **宇宙では通常の安全網がない**: 地上のデータセンターなら、職員を送ってディスクを交換したりサーバを再インストールしたりできますが、衛星は遠隔で復旧しなければならず、あらゆる復旧の経路を打ち上げ前に構築し、実証しておく必要があります。
* **最初は区別がつかない故障と攻撃**: 放射線によるビット反転、故障しかけた部品、悪意ある改ざんは似た症状を示すことがあるため、原因が分かる前に、まず安全に問題を封じ込める対応が必要です。

### 2. 封じ込めと復旧のための設計
軌道上のシステムにおける侵害前提のアーキテクチャ:

* **広がりを抑える分割**: ペイロードの計算、飛行制御、通信を、厳密に定義した接点を持つ隔離された領域で動かし、AIの処理が侵害されても、宇宙機の安全を保つシステムには届かないようにします。
* **ハードウェアの信頼の基点と検証付き起動**: 各ノードは、保護された信頼の基点が署名を確認したファームウェアとソフトウェアからのみ起動し、戻ることのできる既知の正常なイメージを保持します。これはNIST SP 800-193がプラットフォームのファームウェアのレジリエンスとして説明するものです。
* **機能を縮退させながらの継続**: ノードを隔離または再構築する際は、その作業を健全なノードへ移すか、安全な状態で一時停止し、衛星群が全体として止まるのではなく、能力を落としながら本質的なミッションを続けられるようにします。

### 3. AIの速度と人間の承認による復旧
素早い封じ込めと慎重な復元:

* **検知し提案するAI**: 防御のAIは、ノードの振る舞いを基準と比べ、明らかに異常な処理を事前に承認された範囲内で隔離し、根拠となる証拠を添えて復旧計画を提案します。
* **取り消せない段階は人間が承認**: ノードの消去、衛星群全体での暗号鍵の更新、飛行ソフトウェアの再読み込みは有資格の運用担当者が承認します。これらは元に戻せず、診断が誤っていればミッションを危険にさらすためです。
* **信頼できる状態から復元し、その後に再接続する**: 復旧したノードは署名済みのイメージから再構築し、完全性を確認し、原因を理解した後にのみ運用に戻して、システムとともに攻撃者まで復元してしまわないようにします。

### 4. 学習の循環とそれを回す人々
インシデント後の振り返り、教訓の共有、および人材への投資:

* **あらゆるインシデントで設計を改善する**: 各事象の後に責任追及をしない振り返りを行い、何が起き、どれだけ速く封じ込め、どの統制が機能しなかったかを記録します。その結果の変更は、書類として保管するのではなく、完了まで追跡します。
* **業界全体での教訓の共有**: 運用事業者は、Space Information Sharing and Analysis Center（Space ISAC）などの組織を通じて匿名化した知見を共有し、一つの組織の復旧を、すべての組織の予防に変えます。
* **人的資本としての復旧の技能**: 見慣れない故障を診断し、遠隔のシステムを安全に復元する力は経験と練習によって育ちます。そのため、熟練した技術者を自動化に置き換えるのではなく、とどめて育てることこそが、試されたときにレジリエンスのある設計を機能させます。

### 5. 結論
完全な防止は幻想であり、技術者を送れず放射線が独自の故障を加える軌道上では、システムが被害を封じ込め、信頼できる状態へ戻る速さと安全さこそが決定的な能力となります。

分割された設計、ハードウェアの信頼の基点からの復旧、検知し提案するAI、そして取り消せない操作を承認し各インシデントから学ぶCISSP資格の人々により、軌道上のAIシステムは、決して失敗しないからではなく、必ず復旧するからこそ強くなります。
