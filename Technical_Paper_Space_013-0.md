# Koki's Technical Paper — Space Cyber Defense Series SCD-013

## Biological Logic Healing — Designing Safe Self-Repair and Recovery for Space Systems

### Summary Digest
Living organisms heal because they can detect damage, isolate it, and restore normal function from a trusted blueprint. Space systems need the same ability, but self-repair that is poorly designed can turn one fault into a disaster. In July 2024, a faulty security software update crashed about 8.5 million Windows devices worldwide, while in April 2024 engineers restored a spacecraft launched in 1977 by carefully relocating code around a failed memory chip from billions of kilometers away.

This main paper of SCD-013 introduces safe self-repair for space systems. It applies CISSP Domains 3, 7, and 8, explains how rollback, safe modes, roots of trust, containment, and recovery testing work together, and shows why people must remain in charge of how systems heal.

---
### 1. What Healing Means for Space Systems
Detect, Isolate, Restore:

* **Detection Comes First**: A system can heal only if it knows something is wrong, so health monitoring of software, memory, power, and attitude is the foundation of recovery.
* **Isolation Prevents Spreading**: Biological healing contains damage before repairing it, and space systems likewise limit a fault or intrusion to the smallest possible area.
* **Restoration Needs a Trusted Blueprint**: Recovery returns the system to a known good state, using protected software images and configuration rather than whatever is currently running.

### 2. Lessons From Recent Events
Both Success and Failure Teach:

* **Updates Without Safeguards Spread Harm**: The 2024 faulty update was distributed to all affected devices simultaneously and reverted 78 minutes later, yet many systems needed manual recovery for days, showing why staged rollout and automatic fallback matter.
* **Patient Human Repair Can Succeed**: Engineers traced a spacecraft's garbled data to a single failed chip, divided the affected code into pieces, moved it elsewhere in memory, and confirmed success after a round trip of nearly two days.
* **Safe Mode Itself Can Fail**: In February 2026, an anomaly on a European formation-flying satellite caused a loss of orientation and prevented its expected entry into safe mode, and the spacecraft was recovered only after weeks of careful work.

### 3. AI-Assisted Healing Under Human Authority
Fast Detection, Careful Repair:

* **AI Speeds Diagnosis**: AI can compare telemetry with normal baselines, suggest likely causes, and propose recovery steps far faster than manual review.
* **Self-Repair Can Be Exploited**: An attacker who understands automatic recovery might trigger it repeatedly or trick it into restoring a malicious image, consistent with the manipulation risks in NIST AI 100-2e2025, so recovery always relies on signed, protected images.
* **Proposed Healing Authority Rule**: Onboard systems may automatically enter safe mode and fall back to a verified image, but uploading new code, changing recovery logic, or leaving safe mode for normal operations is approved by qualified operators.

### 4. Healers Who Understand the Whole System
Experience That Cannot Be Downloaded:

* **Deep Knowledge Saves Missions**: The 2024 spacecraft recovery relied on engineers who understood decades-old hardware and software, showing that institutional knowledge is a security asset.
* **Cutting Experienced Staff Weakens Recovery**: Organizations that remove experienced engineers in favor of automation may find no one able to repair the automation when it fails.
* **CISSP Supports Resilient Design**: CISSP Domain 3 covers secure architecture and roots of trust, Domain 7 covers recovery and resilience, and Domain 8 covers secure software change and deployment.

### 5. Conclusion
Self-repair can keep space systems alive through faults and attacks, but only when it is designed to detect carefully, isolate firmly, and restore from trusted sources.

By combining staged updates, reliable safe modes, protected roots of trust, AI that speeds diagnosis, and skilled people who guide every major repair, the space community can build systems that heal like living things and keep serving people for many years.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-013

## 生物のような論理の治癒 — 宇宙システムのための安全な自己修復と回復の設計

### サマリー・ダイジェスト
生き物が傷を治せるのは、傷に気づき、それを閉じ込め、信頼できる設計図から普段の働きを取り戻せるからです。宇宙システムにも同じ力が必要ですが、設計の悪い自己修復は、ひとつの不具合を大きな災害に変えてしまうことがあります。2024年7月、欠陥のあるセキュリティ・ソフトウェアの更新が世界中で約850万台のWindowsの機器を止めました。一方、2024年4月には、技術者たちが、何十億キロも離れたところから、壊れたメモリーのチップを避けてプログラムを慎重に移し替え、1977年に打ち上げられた探査機を立て直しました。

SCD-013の本編である本論文は、宇宙システムのための安全な自己修復を紹介します。CISSPのドメイン3、7、8を適用し、元に戻す仕組み（ロールバック）、セーフモード、信頼の基点、封じ込め、回復の試験がどう組み合わさるかを説明し、システムがどう治るかを、人が主導し続けなければならない理由を示します。

---
### 1. 宇宙システムにとって「治る」とは
見つける、閉じ込める、取り戻す:

* **まず見つけること**: システムは、何かがおかしいと知って初めて治ることができます。そのため、ソフトウェア、メモリー、電力、姿勢の健康の監視が、回復の土台になります。
* **閉じ込めが広がりを防ぐ**: 生き物の治癒は直す前に傷を閉じ込めます。宇宙システムも同じように、不具合や侵入を、できるだけ小さな範囲にとどめます。
* **取り戻すには信頼できる設計図が要る**: 回復では、今動いているものではなく、守られたソフトウェアのイメージと設定を使って、システムを正しく動いていたとわかっている状態に戻します。

### 2. 最近の出来事からの教訓
成功からも失敗からも学べる:

* **安全策のない更新は害を広げる**: 2024年の欠陥のある更新は、影響を受けたすべての機器に同時に配られ、78分後に取り消されましたが、多くのシステムは何日も手作業での復旧が必要でした。段階的な配布と自動で元に戻る仕組みが大切な理由を示しています。
* **人の忍耐強い修理は成功しうる**: 技術者たちは、探査機の意味をなさないデータの原因を、壊れたひとつのチップにまでたどりました。そして影響を受けたプログラムをいくつもの部分に分け、メモリーの別の場所に移し、片道1日近く、往復で2日近くかかる通信を待って成功を確かめました。
* **セーフモードそのものが働かないこともある**: 2026年2月、ヨーロッパの編隊飛行の衛星で起きた異常が向きの喪失を引き起こし、予定されていたセーフモードへの移行を妨げました。この宇宙機は、何週間もの注意深い作業の末に、ようやく立て直されました。

### 3. 人の権限の下でのAIによる治癒の支援
素早い発見、慎重な修理:

* **AIが診断を速くする**: AIは、テレメトリを普段の基準と比べ、ありそうな原因を示し、回復の手順を、手作業の確認よりずっと速く提案できます。
* **自己修復は悪用されることがある**: 自動の回復の仕組みを理解した攻撃者は、それを何度も起こさせたり、悪意のあるイメージを元に戻させたりするかもしれません。これはNIST AI 100-2e2025が述べる操作のリスクと同じ趣旨です。そのため回復では、いつも署名された、守られたイメージを使います。
* **治癒の権限の規則（提案）**: 搭載のシステムは自動でセーフモードに入り、確かめられたイメージに戻ってかまいません。しかし、新しいプログラムの送信、回復の仕組みの変更、セーフモードから普段の運用に戻ることは、有資格の運用担当者が承認します。

### 4. システム全体を理解する治し手
ダウンロードできない経験:

* **深い知識がミッションを救う**: 2024年の探査機の回復は、何十年も前のハードウェアとソフトウェアを理解する技術者たちに支えられており、組織の中に積み重なった知識がセキュリティの資産であることを示しています。
* **経験のある人を削ると回復が弱くなる**: 自動化を理由に経験のある技術者を減らす組織は、自動化そのものが壊れたときに、それを直せる人が誰もいないことに気づくかもしれません。
* **CISSPが回復力のある設計を支える**: CISSPのドメイン3は安全な設計と信頼の基点を、ドメイン7は復旧と回復力を、ドメイン8は安全なソフトウェアの変更と配布を扱います。

### 5. 結論
自己修復は、不具合や攻撃を乗り越えて宇宙システムを生かし続けられます。ただしそれは、慎重に見つけ、しっかり閉じ込め、信頼できる源から取り戻すように設計されているときだけです。

段階的な更新、頼れるセーフモード、守られた信頼の基点、診断を速くするAI、そして大きな修理のすべてを導く技能のある人々を組み合わせることで、宇宙の世界は、生き物のように治り、何年も人々の役に立ち続けるシステムを築けます。
