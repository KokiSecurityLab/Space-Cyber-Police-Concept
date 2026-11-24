# Koki's Technical Paper — Space Cyber Defense Series SCD-001-3

## Sustained Vigilance — Continuous Monitoring Discipline, Analyst Sustainability, and Human-AI Teaming in Round-the-Clock Operations

### Summary Digest
Orbital computing never closes for the night, since satellites such as Google's Project Suncatcher test platform are placed in sun-synchronous orbits to receive almost constant sunlight, so their defense must also run continuously, yet vigilance that depends on exhausted people fails as surely as a monitoring tool that silently stops.

This paper treats sustained vigilance under CISSP Domain 7 as an engineered capability, in which AI performs tireless first-line monitoring, rested and well-supported professionals make the decisions, and the commitment to protect people becomes a clear mission rather than an unending personal burden.

---
### 1. Why Continuous Defense Breaks Down
Common Failure Points in 24/7 Operations:

* **Monitoring Gaps Nobody Notices**: Log sources stop sending, sensors lose contact during ground-station handovers, or a rule silently fails, and without health checks the absence of alerts is mistaken for the absence of attacks.
* **Alert Fatigue Erodes Attention**: Analysts facing thousands of low-value alerts each shift begin to dismiss them by habit, which is precisely when a quiet, genuine intrusion slips through.
* **Understaffing Turns Vigilance Into Burnout**: ISC2's 2025 Workforce Study found that 95 percent of respondents reported at least one skills gap on their teams and 88 percent had suffered a significant security consequence from skills shortages, showing that thin teams cannot sustain round-the-clock attention.

### 2. Engineering Persistent Monitoring
Health Checks, Coverage, and Escalation Paths:

* **Monitor the Monitors**: Every telemetry feed, sensor, and detection rule has an expected heartbeat and volume, and a drop raises its own alert so that blind spots are discovered within minutes rather than after an incident.
* **Coverage Across Orbital Contact Windows**: Satellites store security telemetry during gaps in ground contact and transmit it at the next pass, while onboard rules handle urgent events autonomously within limits set in advance by human operators.
* **Clear Escalation by Severity**: Defined thresholds determine when an event moves from automated handling to an analyst and from an analyst to an incident commander, so no one must guess at three in the morning whether to wake a decision maker.

### 3. Human-AI Teaming on Every Shift
Dividing Work by Strength:

* **AI as the Tireless First Line**: Defensive AI watches every feed without fatigue, clusters duplicates, enriches alerts with context, and drafts a summary for each case, removing the repetitive work that drains human attention.
* **People Make the Consequential Calls**: Analysts confirm what AI surfaces, investigate the ambiguous cases, and decide on containment, keeping accountability with a qualified professional as CISSP Domain 7 expects for incident handling.
* **Handover Discipline Between Shifts**: Each shift ends with a documented handover of open cases, pending decisions, and unusual signals, and AI-generated summaries are reviewed by the outgoing analyst before they are relied on.

### 4. Sustaining the People Who Keep Watch
Staffing, Rest, and a Purpose Worth Keeping:

* **Staff for Sustainability, Not Heroics**: Rotations, fair on-call limits, and enough trained people on each team keep alertness high, because vigilance that depends on a few overworked individuals collapses when they leave.
* **Reinvest Automation Gains in People**: Time saved by AI is used for training, threat hunting, and rest rather than for reducing headcount, so automation raises the skill of the team instead of thinning it.
* **A Mission That Protects People on Both Sides of the Screen**: The motivation to protect communities that depend on orbital services is a real strength of security teams, and honoring it with reasonable workloads, respect, and careers that grow alongside AI points toward a future in which capable professionals thrive rather than fear replacement.

### 5. Conclusion
Persistent vigilance is not a matter of willpower but of design, combining monitored monitoring, coverage that survives orbital contact gaps, and escalation paths that tell each person what to do and when.

AI that watches without tiring, CISSP-qualified professionals who decide, and organizations that staff and support those professionals for the long term turn the commitment to protect into round-the-clock defense that orbital AI systems can depend on.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-001-3

## 持続する警戒 — 継続的監視の規律、分析担当者の持続可能性、および24時間運用における人とAIの協働

### サマリー・ダイジェスト
GoogleのProject Suncatcherの試験機のような衛星は、ほぼ絶え間なく太陽光を受けるために太陽同期軌道に置かれ、軌道上の計算基盤が夜に閉まることはありません。そのため防御も継続して動き続けなければなりませんが、疲れ切った人に頼る警戒は、知らないうちに止まる監視ツールと同じように必ず失敗します。

本論文は、CISSPのドメイン7のもとで、持続する警戒を設計された能力として扱います。AIが疲れを知らない第一線の監視を担い、十分に休み支援を受けた専門家が判断を下し、人々を守るという思いを、終わりのない個人の重荷ではなく明確な任務とします。

---
### 1. 継続的な防御が崩れる理由
24時間運用でよく起きる破綻の箇所:

* **誰も気づかない監視の空白**: ログの送信元が送信を止めたり、地上局の切り替えの間にセンサーが接続を失ったり、規則が気づかれないまま機能しなくなったりします。健全性の確認がなければ、アラートがないことが攻撃がないことと取り違えられます。
* **注意力を削るアラート疲れ**: 勤務ごとに何千件もの価値の低いアラートに向き合う分析担当者は、習慣的にそれを退けるようになり、まさにそのときに静かで本物の侵入がすり抜けます。
* **人手不足が警戒を燃え尽きに変える**: ISC2の2025年版人材調査では、回答者の95％がチームに少なくとも一つの技能不足を報告し、88％が技能不足による重大なセキュリティ上の影響を受けていました。手薄なチームでは24時間の注意を保てないことを示しています。

### 2. 持続する監視の設計
健全性の確認、網羅範囲、および段階的な引き上げの経路:

* **監視するものを監視する**: すべてのテレメトリの流れ、センサー、検知規則に想定される死活の信号と量を定め、それが下がれば独自のアラートを上げて、死角をインシデントの後ではなく数分以内に見つけます。
* **軌道上の通信可能時間をまたぐ網羅**: 衛星は地上との通信が途切れる間もセキュリティのテレメトリを保存して次の通過時に送信し、緊急の事象には、人間の運用担当者が事前に定めた範囲内で機上の規則が自律的に対応します。
* **重大度に応じた明確な引き上げ**: 定めた閾値により、事象が自動処理から分析担当者へ、分析担当者からインシデントの指揮者へ移る時点を決め、午前3時に判断者を起こすべきかを誰も迷わなくて済むようにします。

### 3. すべての勤務での人とAIの協働
強みに応じた作業の分担:

* **疲れを知らない第一線としてのAI**: 防御のAIは疲れることなくすべての流れを見守り、重複をまとめ、アラートに文脈を補い、案件ごとに要約を起案して、人の注意力を奪う繰り返しの作業を取り除きます。
* **重大な判断を下すのは人**: 分析担当者は、AIが示したものを確認し、あいまいな案件を調査し、封じ込めを決定します。CISSPのドメイン7がインシデント対応に求めるとおり、説明責任を有資格の専門家に保ちます。
* **勤務の交代の規律**: 各勤務は、未解決の案件、保留中の判断、普段と違う兆候を文書で引き継いで終わり、AIが作った要約は、頼る前に交代する分析担当者が確認します。

### 4. 見張りを続ける人々を支える
人員配置、休息、および守り続ける価値のある目的:

* **英雄的努力ではなく持続可能性のための人員配置**: 交代制、公正な待機の上限、各チームに十分な訓練済みの人数をそろえることで注意力を高く保ちます。働きすぎの少数の人に頼る警戒は、その人たちが去れば崩れるためです。
* **自動化の成果を人に再投資する**: AIで節約した時間を人員の削減ではなく、教育、脅威ハンティング、休息に使い、自動化がチームを薄くするのではなく、チームの技能を高めるようにします。
* **画面の両側の人々を守る任務**: 軌道上のサービスに頼る地域社会を守りたいという思いは、セキュリティチームの本当の強みです。それを、無理のない業務量、敬意、AIとともに伸びるキャリアで報いることが、有能な専門家が置き換えを恐れずに力を発揮できる未来につながります。

### 5. 結論
持続する警戒は意志の力ではなく設計の問題であり、監視そのものの監視、軌道上の通信の空白を乗り越える網羅範囲、そして誰が何をいつすべきかを示す引き上げの経路を組み合わせることで成り立ちます。

疲れずに見守るAI、判断を下すCISSP資格の専門家、そしてその専門家を長く配置し支える組織により、人々を守るという思いを、軌道上のAIシステムが頼りにできる24時間の防御へと変えます。
