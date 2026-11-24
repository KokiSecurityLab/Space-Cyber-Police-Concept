# Koki's Technical Paper — Space Cyber Defense Series SCD-002-3

## Beyond Signature Detection — Behavioral Baselines for Unknown Attacks, Defending the Detector, and Analyst-Led Triage

### Summary Digest
Signature-based tools recognize only attacks that someone has already seen, yet space systems face novel techniques against command links, ground software, and onboard AI, and NIST's March 2025 report AI 100-2e2025 shows that the machine-learning detectors meant to catch those techniques can themselves be poisoned or evaded.

This paper applies CISSP Domains 7 and 8 to build behavioral baselines that can reveal unknown attacks, harden the detection models against manipulation, and keep trained analysts at the center of triage, so that AI widens what defenders can see without deciding alone what is real.

---
### 1. The Limits of Known Patterns
Why Space Systems Need More Than Signatures:

* **Signatures Lag Behind New Techniques**: A signature describes a past attack, so a zero-day exploit against ground-station software or a novel command sequence sent to a satellite passes unnoticed until someone writes a new rule.
* **Space Systems Are Rarely Updated Quickly**: Spacecraft software is patched slowly and carefully, which gives attackers longer windows to use new techniques and makes early detection of unusual behavior especially valuable.
* **Frameworks Show the Range of Unknowns**: The Aerospace Corporation's SPARTA matrix catalogs spacecraft-specific techniques such as command-link intrusion and payload manipulation, many of which have no public signature at all.

### 2. Behavioral Baselines That Reveal the Unexpected
Normal Patterns, Meaningful Deviations, and Context:

* **Learn What Normal Looks Like**: Command rates, telemetry ranges, link timing, operator login patterns, and data volumes are measured over time to form a baseline for each satellite, station, and user role.
* **Score Deviations, Not Just Matches**: A command sent outside an approved pass window, a sudden change in battery or attitude telemetry, or an unusual data transfer from a ground server is scored against that baseline even when no known signature matches.
* **Add Context to Reduce False Alarms**: Space weather data, maintenance schedules, and planned maneuvers explain many anomalies, so correlating them with alerts keeps analysts focused on the deviations that no legitimate activity can explain.

### 3. Defending the Detector and Keeping People in Charge
Adversarial Machine Learning and Accountable Triage:

* **Attackers Target the Model**: NIST AI 100-2e2025 describes poisoning, in which corrupted training data teaches a model to ignore an attack, and evasion, in which inputs are crafted to slip past it, so detectors are trained on curated data, tested with red-team inputs, and monitored for drift.
* **Explainable Alerts Support Human Judgment**: Each alert shows which measurements deviated, by how much, and compared with what baseline, so an analyst can verify the reasoning instead of trusting an unexplained score.
* **Proposed Triage Rule**: AI may rank, group, and enrich alerts automatically, but closing a high-severity alert as benign or declaring an incident requires a qualified analyst, whose decisions are also used to retrain the model under change control.

### 4. Analysts as the Strategic Advantage
Skills, Fair Careers, and the Danger of Over-Automation:

* **Unknown Attacks Need Human Reasoning**: When an alert does not match any known pattern, deciding whether it is an attack requires knowledge of the mission, the hardware, and the adversary, which is why AI-assisted operations still depend on experienced analysts.
* **Cutting Analysts to Save Costs Raises Risk**: Replacing junior and mid-level analysts with automation removes the people who would have become tomorrow's senior experts, leaving organizations unable to investigate novel attacks or audit their own AI.
* **CISSP Supports the Career Path**: CISSP Domain 7 covers investigations, logging, and incident management, giving analysts from many backgrounds a recognized path from alert triage to incident leadership, and organizations a reason to develop rather than replace them.

### 5. Conclusion
Signature detection remains useful, but space systems need behavioral baselines to reveal attacks no one has seen before, and those baselines are only as trustworthy as the protected, tested models that compute them.

Pairing explainable AI detection with qualified analysts who decide what counts as an incident lets defenders see further without surrendering judgment, and investing in those analysts secures both the mission and the future of the profession.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-002-3

## シグネチャ検知を超えて — 未知の攻撃のための挙動ベースライン、検知器の防御、および分析担当者が主導する選別

### サマリー・ダイジェスト
シグネチャに基づくツールは、誰かがすでに見た攻撃しか認識できません。しかし宇宙システムは、指令リンク、地上のソフトウェア、搭載AIに対する新しい手法にさらされています。そしてNISTが2025年3月に公表したAI 100-2e2025は、そうした手法を見つけるはずの機械学習の検知器自体が、汚染されたり回避されたりし得ることを示しています。

本論文はCISSPのドメイン7と8を適用して、未知の攻撃を明らかにできる挙動のベースラインを築き、検知モデルを操作から守り、訓練された分析担当者を選別の中心に置き続けます。AIが防御側の見える範囲を広げつつも、何が本物かを単独で決めないようにするためです。

---
### 1. 既知のパターンの限界
宇宙システムにシグネチャ以上のものが必要な理由:

* **シグネチャは新しい手法に遅れる**: シグネチャは過去の攻撃を記述したものです。そのため、地上局のソフトウェアを狙うゼロデイ攻撃や、衛星に送られる新しい指令の並びは、誰かが新しい規則を書くまで気づかれずに通り抜けます。
* **宇宙システムはめったに素早く更新されない**: 宇宙機のソフトウェアは、ゆっくりと慎重にパッチが当てられます。そのため攻撃者は新しい手法を長い期間使うことができ、普段と違うふるまいを早く見つけることがとりわけ重要になります。
* **フレームワークが示す未知の広がり**: Aerospace CorporationのSPARTAマトリクスは、指令リンクへの侵入やペイロードの操作など、宇宙機に特有の手法をまとめています。その多くには、公開されたシグネチャがまったくありません。

### 2. 予期しないものを明らかにする挙動のベースライン
平常のパターン、意味のある逸脱、および文脈:

* **平常の姿を学ぶ**: 指令の頻度、テレメトリの範囲、リンクのタイミング、運用者のログインのパターン、データ量を継続して測定し、衛星、地上局、利用者の役割ごとにベースラインを作ります。
* **一致だけでなく逸脱を評価する**: 承認された通過時間帯の外で送られた指令、電池や姿勢のテレメトリの急な変化、地上サーバーからの普段と違うデータ転送は、既知のシグネチャに一致しなくても、ベースラインと照らして評価します。
* **文脈を加えて誤報を減らす**: 宇宙天気のデータ、保守の予定、計画された軌道制御は、多くの異常を説明します。これらをアラートと突き合わせることで、分析担当者は、正規の活動では説明できない逸脱に集中できます。

### 3. 検知器を守り、人が主導権を持ち続ける
敵対的機械学習と説明責任のある選別:

* **攻撃者はモデルを狙う**: NIST AI 100-2e2025は、汚染された学習データによってモデルに攻撃を見逃すよう覚えさせる「ポイズニング」と、すり抜けるように入力を細工する「回避」を説明しています。そのため検知器は、精選したデータで学習させ、レッドチームの入力で試験し、性能のずれを監視します。
* **説明できるアラートが人の判断を支える**: 各アラートには、どの測定値が、どれだけ、どのベースラインと比べて逸脱したかを示します。分析担当者は、説明のない点数を信じるのではなく、その理由を検証できます。
* **選別の規則（提案）**: AIはアラートの順位付け、グループ化、情報の追加を自動で行ってかまいません。しかし、深刻度の高いアラートを無害として閉じることや、インシデントを宣言することは有資格の分析担当者が行い、その判断は変更管理のもとでモデルの再学習にも使います。

### 4. 戦略的な強みとしての分析担当者
技能、公正なキャリア、および自動化しすぎることの危険:

* **未知の攻撃には人の推論が必要**: アラートが既知のどのパターンにも一致しないとき、それが攻撃かどうかを判断するには、ミッション、ハードウェア、攻撃者についての知識が必要です。AIに支えられた運用でも、経験のある分析担当者に頼り続けるのはこのためです。
* **費用削減のための分析担当者の削減はリスクを高める**: 初級や中堅の分析担当者を自動化で置き換えると、将来の上級専門家になるはずだった人々がいなくなります。その結果、組織は新しい攻撃を調査することも、自らのAIを監査することもできなくなります。
* **CISSPがキャリアの道筋を支える**: CISSPのドメイン7は、調査、ログ管理、インシデント管理を扱います。これはさまざまな経歴を持つ分析担当者に、アラートの選別からインシデント対応の指揮へと進む認められた道筋を与え、組織には人を置き換えるのではなく育てる理由を与えます。

### 5. 結論
シグネチャ検知は今も役に立ちますが、宇宙システムには、誰も見たことのない攻撃を明らかにする挙動のベースラインが必要です。そして、そのベースラインの信頼性は、それを計算する、守られ試験されたモデルの信頼性で決まります。

説明できるAIによる検知と、何をインシデントとするかを決める有資格の分析担当者を組み合わせれば、防御側は判断を手放すことなく、より遠くまで見通せます。そしてその分析担当者への投資は、ミッションと、この職業の未来の両方を守ります。
