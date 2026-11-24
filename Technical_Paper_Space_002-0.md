# Koki's Technical Paper — Space Cyber Defense Series SCD-002

## The Invisible Shield — Securing Laser Communications Through Layered Authentication, Physical-Layer Monitoring, and Human-Governed Response

### Summary Digest
Laser links are becoming the backbone of space networks: NASA's Artemis II mission used the O2O optical terminal in April 2026 to send 4K video from lunar distance at up to 260 Mbps, Google's Project Suncatcher demonstrated 1.6 Tbps on a bench-scale optical link between two nodes, and the U.S. Space Development Agency is building a military mesh of satellites joined by optical inter-satellite links.

This paper applies CISSP Domains 3 and 4 to show that a narrow beam is harder to intercept but is not secure by itself, and it proposes a layered defense that combines cryptographic authentication, physical-layer monitoring, and AI-assisted detection under the authority of qualified people, supported by a broad workforce that understands both optics and security.

---
### 1. Why Laser Links Change the Threat Model
New Capabilities, Narrow Beams, and New Weak Points:

* **Throughput Is Rising Fast**: NASA's TBIRD payload on a 6U CubeSat downlinked 4.8 terabytes in a single five-minute pass at 200 Gbps in 2023, and orbital AI clusters such as Suncatcher will depend on links far faster than any radio system.
* **A Narrow Beam Reduces Interception, Not All Risk**: An eavesdropper must stand almost inside the beam, so optical links offer a low probability of intercept, yet ground terminals, pointing and tracking software, key management, and the networks behind each station remain exposed.
* **Integration Is the Hardest Part**: The Space Development Agency reported in March 2026 that it had not yet established the optical mesh for its first operational tranche, and Aviation Week reported that the mesh was still proving elusive with more than 80 transport satellites in orbit, showing that link management, not only the laser, is where faults and attacks hide.

### 2. A Layered Defense for Optical Links
Cryptography, Physical-Layer Evidence, and Ground Hardening:

* **Authenticate Every Frame**: The CCSDS Space Data Link Security protocol provides authentication and encryption at the data-link layer, and pairing it with the post-quantum standards NIST published in August 2024 (FIPS 203, 204, and 205) protects keys and commands for the long lifetime of a spacecraft.
* **Use the Physics as a Second Witness**: Received power, pointing error, bit-error rate, and timing jitter form a baseline for each link, so a sudden change that the encrypted payload cannot explain is recorded as evidence and investigated rather than ignored.
* **Harden the Ground, Where Most Attacks Begin**: Optical ground stations need site diversity for clouds, protection against dazzling or jamming of their receivers, and the same identity, patching, and segmentation controls as any critical data center.

### 3. Human-Governed Detection and Response
AI Speed, Model Security, and Accountable Decisions:

* **AI Watches the Signals at Machine Speed**: Machine-learning models compare thousands of link measurements per second against the baseline and flag the small deviations that a person could not track across a whole constellation.
* **The Detector Is Itself a Target**: NIST AI 100-2e2025 classifies poisoning and evasion attacks against machine-learning systems, so detection models are trained on controlled data, tested against manipulated inputs, and versioned like flight software under CISSP Domain 8.
* **People Decide on Mission-Affecting Actions**: Dropping a link, rerouting traffic, or revoking a station's keys can isolate a satellite cluster, so the AI recommends and a named, qualified professional approves, consistent with the human oversight duty in Article 14 of the EU AI Act.

### 4. The Workforce Behind the Beam
Hybrid Skills, Fair Opportunity, and Shared Benefits:

* **Optical Security Needs Hybrid Professionals**: Defending laser links requires people who understand photonics, network protocols, cryptography, and incident response together, a mix that no single genius or automated tool can supply across hundreds of satellites and ground stations.
* **Change Should Create Roles, Not Discard People**: The World Economic Forum's Future of Jobs Report 2025 projects 170 million jobs created and 92 million displaced by 2030 and names upskilling as employers' top strategy, which argues for retraining experienced radio and network engineers into optical security rather than replacing them with automation.
* **CISSP as a Common Language**: The CISSP body of knowledge gives engineers, operators, and managers a shared vocabulary for risk, architecture, and accountability, so that capable people from many backgrounds can contribute and advance.

### 5. Conclusion
Laser communications make space networks faster and harder to intercept, but their security depends on authentication, physical-layer evidence, hardened ground stations, and well-defended AI detectors working together.

When AI handles speed and scale while qualified people hold final authority, and when organizations invest in the many professionals who keep these links running, the invisible shield becomes a real one.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-002

## 見えない盾 — 多層の認証、物理層の監視、および人が統治する対応によるレーザー通信の保護

### サマリー・ダイジェスト
レーザー通信は宇宙ネットワークの基幹になりつつあります。NASAのアルテミスII計画は2026年4月、光通信端末O2Oを使い、月の距離から最大260 Mbpsで4K映像を送りました。GoogleのProject Suncatcherは2つの端末間の実験台規模の光リンクで1.6 Tbpsを実証し、米国宇宙開発庁（SDA）は光の衛星間リンクで結ばれた軍事用の衛星網を構築しています。

本論文はCISSPのドメイン3と4を適用し、細いビームは傍受されにくいものの、それだけで安全ではないことを示します。そして、暗号による認証、物理層の監視、AIによる検知支援を、有資格の人の権限のもとで組み合わせる多層防御を提案します。その土台となるのは、光学とセキュリティの両方を理解する幅広い人材です。

---
### 1. レーザー通信が脅威モデルを変える理由
新しい能力、細いビーム、および新しい弱点:

* **急速に高まる通信容量**: NASAのTBIRDは2023年、6UのCubeSatから200 Gbpsで、1回約5分の通過の間に4.8テラバイトを地上へ送りました。Suncatcherのような軌道上のAIクラスタは、どの電波通信よりもはるかに速いリンクに依存することになります。
* **細いビームが減らすのは傍受であって、すべてのリスクではない**: 盗聴者はほぼビームの中に入らなければならないため、光リンクは傍受されにくい性質を持ちます。しかし、地上端末、指向・追尾のソフトウェア、鍵の管理、各局の背後にあるネットワークは、依然として攻撃にさらされています。
* **最も難しいのは統合**: SDAは2026年3月、最初の運用トランシェの光メッシュ網をまだ確立できていないと報告し、Aviation Weekは80基を超える輸送衛星が軌道上にある段階でも、メッシュ網の確立は難航していると伝えました。不具合や攻撃が潜むのはレーザーそのものだけではなく、リンクの管理であることを示しています。

### 2. 光リンクのための多層防御
暗号、物理層の証拠、および地上の強化:

* **すべてのフレームを認証する**: CCSDSのSpace Data Link Securityプロトコルは、データリンク層で認証と暗号化を提供します。これを、NISTが2024年8月に公表した耐量子暗号の標準（FIPS 203、204、205）と組み合わせることで、宇宙機の長い運用期間にわたって鍵と指令を守ります。
* **物理現象を2人目の証人にする**: 受信電力、指向誤差、ビット誤り率、タイミングの揺らぎは、リンクごとのベースラインになります。暗号化された中身では説明できない急な変化は、見過ごさずに証拠として記録し、調査します。
* **攻撃の多くが始まる地上を強化する**: 光地上局には、雲に備えた複数拠点の分散、受信機への眩惑や妨害からの保護、そしてあらゆる重要データセンターと同じID管理、パッチ適用、ネットワーク分離の統制が必要です。

### 3. 人が統治する検知と対応
AIの速度、モデルのセキュリティ、および説明責任のある判断:

* **機械の速度で信号を見張るAI**: 機械学習モデルは毎秒数千のリンク測定値をベースラインと比べ、衛星群全体にわたって人が追い切れない小さなずれを知らせます。
* **検知器そのものが標的になる**: NIST AI 100-2e2025は、機械学習システムへの汚染（ポイズニング）攻撃や回避攻撃を分類しています。そのため検知モデルは、管理されたデータで学習させ、操作された入力に対して試験し、CISSPのドメイン8に沿って飛行ソフトウェアと同じように版を管理します。
* **ミッションに影響する措置は人が決める**: リンクの切断、通信の迂回、地上局の鍵の失効は、衛星群を孤立させかねません。そこで、AIが推奨し、名前を特定された有資格の専門家が承認します。これはEU AI法第14条が定める人による監督の義務とも整合します。

### 4. ビームを支える人材
複合的な技能、公正な機会、および恩恵の共有:

* **光通信のセキュリティには複合型の専門家が必要**: レーザーリンクを守るには、フォトニクス、ネットワークプロトコル、暗号、インシデント対応をあわせて理解する人が必要です。何百もの衛星と地上局にわたるこの組み合わせを、一人の天才や自動化ツールだけで補うことはできません。
* **変化は人を切り捨てるのではなく、役割を生むべき**: 世界経済フォーラムの「仕事の未来レポート2025」は、2030年までに1億7,000万の仕事が生まれ、9,200万が失われると予測し、企業の最優先の戦略にリスキリングを挙げています。これは、経験のある無線やネットワークの技術者を自動化で置き換えるのではなく、光通信のセキュリティへと育て直すべきことを示しています。
* **共通言語としてのCISSP**: CISSPの知識体系は、技術者、運用者、管理者に、リスク、アーキテクチャ、説明責任についての共通の語彙を与えます。それにより、さまざまな経歴を持つ有能な人々が貢献し、成長できるようになります。

### 5. 結論
レーザー通信は宇宙ネットワークを速く、傍受されにくくしますが、その安全は、認証、物理層の証拠、強化された地上局、そして十分に守られたAI検知器が一体となって働くことにかかっています。

AIが速度と規模を担い、有資格の人が最終権限を持ち、組織がこれらのリンクを動かし続ける多くの専門家に投資するとき、見えない盾は本物の盾になります。
