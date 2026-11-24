# Koki's Technical Paper — Space Cyber Defense Series SCD-017

## The Mesh Firewall — Separation and Routing Security for Inter-Satellite Networks

### Summary Digest
Satellites increasingly talk to each other directly through laser links, forming meshes in orbit that carry data without touching the ground. In July 2026, one large constellation operator described next-generation satellites carrying six optical inter-satellite links of 400 gigabits per second each, and in 2026 such laser meshes began to be offered to third-party spacecraft, including orbital data centers. When many missions share one mesh, the network needs firewalls in space: clear separation, trustworthy routing, and security that works despite long delays.

This main paper of SCD-017 introduces security for inter-satellite mesh networks. It applies CISSP Domains 4, 3, and 7, corrects common misunderstandings about "instant" quantum communication, and shows why people must govern how traffic flows between missions.

---
### 1. Why Orbital Meshes Need Firewalls
Shared Paths, Shared Risks:

* **Meshes Bypass Ground Controls**: Data that moves between satellites may never pass through a ground firewall, so security controls must operate in orbit.
* **Many Tenants Share One Network**: When laser meshes carry traffic for other operators and orbital data centers, a compromise in one mission must not reach others.
* **Routing Decides Who Sees Data**: Whoever can influence routes can redirect, delay, or observe traffic, making routing security as important as encryption.

### 2. Five Foundations of the Mesh Firewall
A Structure for the SCD-017 Series:

* **Security Despite Delay**: SCD-017-1 explains delay-tolerant networking and Bundle Protocol Security for links where round trips take seconds or minutes.
* **Clear Physics, Clear Expectations**: SCD-017-2 explains what quantum entanglement can and cannot do, and SCD-017-3 covers keeping a shared picture of network state across distributed nodes.
* **Trusted Paths and Strong Boundaries**: SCD-017-4 covers routing security in the mesh, and SCD-017-5 covers segmentation between missions.

### 3. AI-Managed Meshes Under Human Policy
Dynamic Routing Within Fixed Rules:

* **AI Can Optimize Routing**: With thousands of laser links forming and breaking every day, AI can choose efficient paths and predict congestion.
* **Routing Intelligence Can Be Misled**: False link reports or manipulated performance data could steer traffic through compromised nodes, consistent with NIST AI 100-2e2025, so routing decisions are constrained by policy and verified identities.
* **Proposed Mesh Policy Rule**: AI may select routes within approved boundaries and isolate misbehaving links, but changing which missions may share links, opening new cross-mission paths, or relaxing encryption requirements is approved by qualified network security staff.

### 4. Network Engineers for a Network in the Sky
People Who Design and Defend the Mesh:

* **New Skills Are Needed**: Orbital meshes combine optical communications, routing, and cybersecurity, creating demand for engineers who understand all three.
* **Standards Need Human Cooperation**: The ITU Radiocommunication Sector has begun studies on how optical inter-satellite links can be standardized alongside radio systems, work that depends on experts from many countries.
* **CISSP Supports Network Security**: CISSP Domain 4 covers secure network architecture and segmentation, Domain 3 covers cryptography, and Domain 7 covers monitoring and response.

### 5. Conclusion
Inter-satellite meshes are becoming the backbone of space communications, and they need firewalls that work in orbit, across delays, and between many missions.

Delay-tolerant security, realistic understanding of quantum technology, synchronized network awareness, secure routing, strong segmentation, AI that optimizes within rules, and skilled engineers who set those rules together will make the network in the sky as trustworthy as the best networks on Earth.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-017

## メッシュのファイアウォール — 衛星どうしのネットワークの分離と経路のセキュリティ

### サマリー・ダイジェスト
衛星は、ますますレーザーの回線で直接話し合うようになり、地上に触れずにデータを運ぶ網の目（メッシュ）を軌道上につくっています。2026年7月、ある大手のコンステレーションの運用者は、毎秒400ギガビットの光の衛星間回線を6本ずつ載せた次の世代の衛星について説明しました。そして2026年には、こうしたレーザーのメッシュが、軌道上のデータセンターを含む、ほかの会社の宇宙機にも提供され始めました。多くのミッションがひとつのメッシュを分け合うと、ネットワークには宇宙の中のファイアウォールが必要になります。はっきりした分離、信頼できる経路、そして長い遅れがあっても働くセキュリティです。

SCD-017の本編である本論文は、衛星どうしのメッシュ・ネットワークのセキュリティを紹介します。CISSPのドメイン4、3、7を適用し、「瞬時」の量子通信についてのよくある誤解を正し、ミッションの間で通信がどう流れるかを人が治めなければならない理由を示します。

---
### 1. 軌道上のメッシュにファイアウォールが必要な理由
分け合う道、分け合うリスク:

* **メッシュは地上の統制を通らない**: 衛星の間を動くデータは、地上のファイアウォールを一度も通らないかもしれないため、セキュリティの統制は軌道上で働かなければなりません。
* **多くの利用者がひとつのネットワークを分け合う**: レーザーのメッシュがほかの運用者や軌道上のデータセンターの通信を運ぶとき、あるミッションの乗っ取りが、ほかのミッションに届いてはなりません。
* **経路が、誰がデータを見るかを決める**: 経路に影響を与えられる者は、通信の向きを変え、遅らせ、のぞき見ることができるため、経路のセキュリティは暗号と同じくらい大切です。

### 2. メッシュのファイアウォールの5つの土台
SCD-017シリーズの構成:

* **遅れがあっても働くセキュリティ**: SCD-017-1は、往復に数秒から数分かかる回線のための、遅延耐性ネットワークとバンドル・プロトコル・セキュリティを説明します。
* **はっきりした物理、はっきりした期待**: SCD-017-2は量子もつれにできることとできないことを説明し、SCD-017-3は散らばったノードにまたがってネットワークの状態の共通の姿を保つことを扱います。
* **信頼できる道と、強い境界**: SCD-017-4はメッシュの中の経路のセキュリティを、SCD-017-5はミッションの間の分離を扱います。

### 3. 人の方針の下で、AIが管理するメッシュ
固定した規則の中での、動的な経路の選択:

* **AIが経路を最適にできる**: 何千ものレーザーの回線が毎日つながっては切れる中で、AIは効率のよい道を選び、混雑を予測できます。
* **経路の知能は惑わされることがある**: 偽の回線の報告や操作された性能のデータは、通信を乗っ取られたノードへと導くかもしれません。これはNIST AI 100-2e2025と同じ趣旨です。そのため、経路の判断は、方針と確かめられたIDで縛ります。
* **メッシュの方針の規則（提案）**: AIは承認された境界の中で経路を選び、おかしなふるまいをする回線を切り離してかまいません。しかし、どのミッションが回線を分け合ってよいかを変えること、ミッションをまたぐ新しい道を開くこと、暗号の求めをゆるめることは、有資格のネットワーク・セキュリティの担当者が承認します。

### 4. 空のネットワークのためのネットワーク技術者
メッシュを設計し、守る人々:

* **新しい技能が必要になる**: 軌道上のメッシュは、光の通信、経路の制御、サイバーセキュリティを組み合わせており、この3つすべてを理解する技術者の需要を生んでいます。
* **標準には人の協力が要る**: 国際電気通信連合の無線通信部門は、光の衛星間回線を電波のシステムと並べてどう標準化できるかの検討を始めており、この仕事は多くの国の専門家に支えられています。
* **CISSPがネットワークのセキュリティを支える**: CISSPのドメイン4は安全なネットワークの設計と分割を、ドメイン3は暗号を、ドメイン7は監視と対応を扱います。

### 5. 結論
衛星どうしのメッシュは宇宙の通信の背骨になりつつあり、軌道上で、遅れをまたいで、多くのミッションの間で働くファイアウォールを必要としています。

遅れに強いセキュリティ、量子技術についての現実的な理解、そろったネットワークの状態の把握、安全な経路、強い分離、規則の中で最適化するAI、そしてその規則を定める技能のある技術者が合わさることで、空のネットワークは、地上の最良のネットワークと同じくらい信頼できるものになります。
