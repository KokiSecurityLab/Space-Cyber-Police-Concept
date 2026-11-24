# Koki's Technical Paper — Space Cyber Defense Series SCD-002-1

## Laser as the New Pulse — Radio Versus Optical Threat Models, Hybrid Link Resilience, and Human Control of Fallback Decisions

### Summary Digest
Space communication is moving from radio waves, which spread widely and can be heard far from the transmitter, to laser beams only a few meters wide at the receiver, a shift shown when Artemis II carried the first laser terminal used on a crewed mission at lunar distance in April 2026 while still relying on NASA's radio networks as its primary link.

This paper applies CISSP Domain 4 to compare the threat models of radio and optical links, explains why the most resilient design combines both, and argues that the decision to switch between them during an incident belongs to trained operators supported by AI, not to automation alone.

---
### 1. From Broadcasting to Pointing
How the Medium Shapes the Attack Surface:

* **Radio Is Easy to Hear and Easy to Jam**: A radio signal spreads over a wide area, so anyone with an antenna and a software-defined radio in the footprint can record, replay, or jam it, which is why the 2022 attack on Viasat's KA-SAT network and many GPS jamming incidents affected users across whole regions.
* **Optical Links Must Be Pointed Precisely**: A laser terminal uses pointing, acquisition, and tracking to hold a beam on a moving target, so an outsider cannot simply listen from the side and must place equipment almost inside the beam path to intercept it.
* **Precision Brings New Failure Modes**: Clouds block optical ground links, pointing errors break the connection, and the software that steers the telescope becomes a target, so the strengths of lasers come with dependencies that defenders must monitor.

### 2. Why Hybrid Links Are More Resilient
Diversity of Medium, Site, and Path:

* **Radio and Light Back Each Other Up**: Artemis II sent 4K video over its O2O laser terminal at up to 260 Mbps while NASA's Near Space Network and Deep Space Network carried the primary radio communications, a design in which losing one medium does not end the mission.
* **Site Diversity Defeats Weather and Local Attacks**: Distributing optical ground stations across regions with different weather patterns keeps at least one station clear, and it also means that a dazzling or jamming attack against one site does not cut the whole network.
* **Different Media Need Different Monitoring**: Radio links are watched for interference and spoofed signals, while optical links are watched for pointing loss, unexpected drops in received power, and unusual reacquisition attempts, and both feed a single security operations view.

### 3. People Control the Switch
AI Recommendations and Accountable Fallback:

* **AI Detects Degradation First**: Models that track signal quality across hundreds of links can tell a passing cloud from a pattern of failures that moves from station to station, and they propose a fallback route within seconds.
* **Fallback Can Itself Be the Attack**: An adversary may degrade the laser path precisely to force traffic onto a radio channel that is easier to intercept or jam, so switching media is treated as a security decision with risk to evaluate, not an automatic reflex.
* **Proposed Fallback Rule**: Routine weather switching may run automatically within preapproved limits, but any fallback during a suspected attack, or any switch that lowers the encryption or authentication level, requires approval from a qualified operator who records the reason.

### 4. Operators Who Understand Both Worlds
Cross-Training, Career Paths, and Human Judgment:

* **Radio Expertise Remains Valuable**: Engineers who spent careers on radio links understand interference, link budgets, and spectrum, knowledge that transfers directly to optical systems and should be developed through retraining rather than discarded.
* **A Broad Bench, Not a Few Specialists**: Round-the-clock operations across many ground stations need many trained operators and analysts, and concentrating the knowledge in a handful of experts or in one automated system creates a single point of failure.
* **CISSP Connects Engineering and Risk**: CISSP Domain 4 frames link design as a security architecture decision, helping engineers and managers agree on when resilience, cost, and risk justify a second medium or another ground station.

### 5. Conclusion
Laser links narrow the attack surface for interception but add new dependencies on pointing, weather, and ground software, while radio remains easier to intercept but essential as a backup.

Hybrid designs, monitored as one system and switched under the control of trained people who can recognize when a fallback is itself the attack, give space networks a pulse that keeps beating under pressure.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-002-1

## 新たな鼓動としてのレーザー — 電波と光の脅威モデル、複合リンクの回復力、および切り替え判断の人による管理

### サマリー・ダイジェスト
宇宙通信は、広く広がり送信源から遠く離れても受信できる電波から、受信点で幅わずか数メートルのレーザーへと移りつつあります。2026年4月、アルテミスIIは有人ミッションとして初めて月の距離でレーザー端末を使いましたが、主な通信は引き続きNASAの電波ネットワークが担いました。

本論文はCISSPのドメイン4を適用して、電波と光のリンクの脅威モデルを比べ、両方を組み合わせる設計が最も回復力が高い理由を説明します。そして、インシデントの最中に両者を切り替える判断は、自動化だけに任せるのではなく、AIの支援を受けた訓練された運用者が担うべきだと論じます。

---
### 1. 放送から照準へ
媒体が攻撃面をどう形づくるか:

* **電波は聞かれやすく、妨害されやすい**: 電波は広い範囲に広がるため、その範囲内でアンテナとソフトウェア無線を持つ人は誰でも、記録、再送、妨害ができます。2022年のViasatのKA-SAT網への攻撃や、多くのGPS妨害の事例が地域全体の利用者に影響したのはこのためです。
* **光リンクは正確に向けなければならない**: レーザー端末は、指向・捕捉・追尾によって動く相手にビームを当て続けます。部外者は横から聞くことができず、傍受するにはほぼビームの通り道の中に機器を置かなければなりません。
* **精密さが生む新しい故障の形**: 雲は光の地上リンクを遮り、指向の誤差は接続を切り、望遠鏡を動かすソフトウェアは標的になります。レーザーの強みには、防御側が監視すべき依存関係が伴います。

### 2. 複合リンクの回復力が高い理由
媒体、拠点、経路の多様性:

* **電波と光が互いを支える**: アルテミスIIはO2Oのレーザー端末で最大260 Mbpsの4K映像を送り、主な電波通信はNASAのNear Space NetworkとDeep Space Networkが担いました。片方の媒体を失ってもミッションが終わらない設計です。
* **拠点の分散が天候と局所的な攻撃に勝つ**: 天候の傾向が異なる地域に光地上局を分散させれば、少なくとも1局は晴れた状態を保てます。また、1か所への眩惑や妨害の攻撃でネットワーク全体が切れることもなくなります。
* **媒体が違えば監視も違う**: 電波リンクでは干渉と偽装信号を、光リンクでは指向の喪失、予期しない受信電力の低下、不自然な再捕捉の試みを監視し、両方を1つのセキュリティ運用の画面にまとめます。

### 3. 切り替えは人が管理する
AIの推奨と説明責任のある切り替え:

* **劣化を最初に見つけるのはAI**: 何百ものリンクの信号品質を追うモデルは、通り過ぎる雲と、局から局へと移っていく故障のパターンとを見分け、数秒のうちに代替経路を提案します。
* **切り替えそのものが攻撃になり得る**: 攻撃者は、傍受や妨害がしやすい電波の回線へ通信を移させるために、あえてレーザーの経路を劣化させることがあります。そのため媒体の切り替えは、反射的な自動動作ではなく、リスクを評価すべきセキュリティ上の判断として扱います。
* **切り替えの規則（提案）**: 日常的な天候による切り替えは、事前に承認された範囲内で自動で行ってかまいません。しかし、攻撃が疑われる最中の切り替えや、暗号化や認証の水準を下げる切り替えには、有資格の運用者の承認と理由の記録を必須とします。

### 4. 両方の世界を理解する運用者
複数分野の訓練、キャリアの道筋、および人の判断:

* **電波の専門知識は今も価値がある**: 長年電波リンクに携わってきた技術者は、干渉、回線設計、周波数を理解しています。その知識は光システムにそのまま生かせるため、捨てるのではなく、学び直しによって伸ばすべきです。
* **少数の専門家ではなく、厚い人材の層**: 多くの地上局で24時間運用を続けるには、訓練された運用者と分析担当者が大勢必要です。知識を一握りの専門家や1つの自動化システムに集中させると、単一障害点が生まれます。
* **CISSPが技術とリスクを結ぶ**: CISSPのドメイン4はリンクの設計をセキュリティアーキテクチャの判断として捉えます。それにより技術者と管理者は、回復力、費用、リスクの観点から、2つ目の媒体や追加の地上局がいつ正当化されるかについて合意できます。

### 5. 結論
レーザーリンクは傍受に対する攻撃面を狭めますが、指向、天候、地上のソフトウェアへの新しい依存を加えます。一方で電波は、傍受されやすいものの、予備として欠かせません。

1つのシステムとして監視され、切り替えそのものが攻撃である場合を見抜ける訓練された人の管理のもとで切り替えられる複合設計こそが、圧力の下でも脈打ち続ける鼓動を宇宙ネットワークに与えます。
