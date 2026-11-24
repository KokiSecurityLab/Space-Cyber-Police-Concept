# Koki's Technical Paper — Space Cyber Defense Series SCD-002-4

## Cross-Layer Correlation — Fusing Optical, Network, and Ground Evidence, AI-Assisted Analysis, and Team-Based Judgment

### Summary Digest
An attack on a space network rarely appears in only one place: a spoofed command may show up as a timing change on the optical link, a failed authentication counter, an unusual login at a ground station, and a small shift in spacecraft telemetry, each of which looks harmless when viewed alone.

This paper applies CISSP Domain 7 to fuse evidence across these layers, uses AI to align and summarize millions of events, and keeps interpretation with diverse teams of qualified people, because connecting physical, digital, and mission context is where human judgment adds the most value.

---
### 1. Why Single-Layer Monitoring Misses Attacks
Fragmented Evidence and Organizational Silos:

* **Each Team Sees One Layer**: Link engineers watch optical power and pointing, network teams watch traffic, ground IT teams watch servers, and flight operators watch telemetry, so an attack that touches each layer lightly can pass through all of them unnoticed.
* **Attackers Exploit the Gaps Between Teams**: In the 2022 KA-SAT incident, the decisive damage came from commands sent through the ground management network to user modems, a path that crossed the boundary between IT and satellite operations.
* **Space Adds Unique Evidence Sources**: Sequence numbers and anti-replay counters in CCSDS Space Data Link Security, orbital tracking data, and space weather reports are rarely in the same tool as ground logs, although together they can confirm or rule out an attack.

### 2. Building a Cross-Layer Picture
Common Time, Common Identity, and Common Models:

* **Align Every Source to One Clock and One Asset List**: Precise timestamps and a shared inventory of satellites, terminals, keys, and stations let analysts place a pointing anomaly, a rejected frame, and a ground login on the same timeline.
* **Use Shared Frameworks to Connect Events**: MITRE ATT&CK for ground systems, the SPARTA matrix for spacecraft techniques, and the Diamond Model's links between adversary, capability, infrastructure, and victim give each layer's evidence a common structure.
* **Test Hypotheses Across Layers**: If a link degrades, analysts check whether space weather explains it, whether authentication failures rose at the same moment, and whether any ground account touched the related station, turning scattered signals into a testable explanation.

### 3. AI Assembles the Picture, People Interpret It
Fusion at Scale and Accountable Conclusions:

* **AI Handles Volume and Alignment**: Models can merge millions of events, suggest which ones belong to the same episode, and draft a summary timeline, work that would take a person days across a large constellation.
* **AI Can Be Misled by Plausible Patterns**: A correlation model may link unrelated events or miss a deliberate slow attack designed to stay below thresholds, and the attack categories in NIST AI 100-2e2025 show that its inputs can be manipulated, so its conclusions are treated as hypotheses.
* **Proposed Attribution Rule**: AI may propose that events form one incident and suggest a likely technique, but declaring an incident, attributing it to an actor, or reporting it to partners such as the Space ISAC requires review and sign-off by a qualified lead analyst.

### 4. Diverse Teams as the Real Correlation Engine
Shared Rotations, Fair Opportunity, and Professional Standards:

* **Different Backgrounds See Different Clues**: An optical engineer recognizes an unusual reacquisition pattern, a network analyst recognizes beaconing, and a flight operator recognizes a command that makes no mission sense, so mixed teams catch what any single specialist would miss.
* **Rotation Builds Broad Expertise in Many People**: Rotating staff between link, network, ground, and flight operations builds a wide pool of capable defenders and avoids dependence on a small group of experts or on a single AI system.
* **CISSP Provides the Shared Frame**: The eight CISSP domains connect architecture, identity, operations, and governance, giving professionals from every layer a common basis for discussing risk and for growing into leadership roles.

### 5. Conclusion
Attacks on space systems spread their traces across optical, network, ground, and mission layers, and only a cross-layer view can join those traces into a clear picture.

AI makes that view possible at scale, while diverse teams of qualified people supply the context and accountability that turn correlations into sound decisions, and organizations that invest in those teams gain a defense that no automated tool can provide alone.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-002-4

## 層をまたぐ相関分析 — 光、ネットワーク、地上の証拠の統合、AIによる分析支援、およびチームによる判断

### サマリー・ダイジェスト
宇宙ネットワークへの攻撃が1か所だけに現れることはまれです。偽装された指令は、光リンクのタイミングの変化、認証の失敗回数、地上局での普段と違うログイン、宇宙機のテレメトリのわずかな変化として現れることがありますが、そのどれもが単独で見れば無害に見えます。

本論文はCISSPのドメイン7を適用して、これらの層をまたいで証拠を統合し、AIを使って何百万件もの事象をそろえて要約します。そして、その解釈は多様な有資格者のチームに委ねます。物理、デジタル、ミッションの文脈を結びつけることこそ、人の判断が最も価値を生む部分だからです。

---
### 1. 単一の層の監視が攻撃を見逃す理由
ばらばらの証拠と組織の縦割り:

* **各チームが見ているのは1つの層だけ**: リンクの技術者は光の出力と指向を、ネットワークのチームは通信を、地上のITチームはサーバーを、運用者はテレメトリを見ています。そのため、各層に少しずつ触れる攻撃は、どのチームにも気づかれずに通り抜けることがあります。
* **攻撃者はチームの間の隙間を突く**: 2022年のKA-SATの事案では、決定的な被害は、地上の管理ネットワークを通じて利用者のモデムに送られた指令から生じました。この経路は、ITと衛星運用の境界をまたいでいました。
* **宇宙ならではの証拠源**: CCSDSのSpace Data Link Securityの通し番号と再送防止のカウンター、軌道追跡データ、宇宙天気の報告が、地上のログと同じツールに入っていることはまれです。しかし、これらを合わせれば攻撃を確かめることも、否定することもできます。

### 2. 層をまたぐ全体像を作る
共通の時刻、共通の識別、および共通のモデル:

* **すべての情報源を1つの時計と1つの資産一覧にそろえる**: 正確なタイムスタンプと、衛星、端末、鍵、地上局の共通の一覧があれば、分析担当者は指向の異常、拒否されたフレーム、地上でのログインを同じ時系列の上に並べられます。
* **共通のフレームワークで事象を結ぶ**: 地上システムにはMITRE ATT&CK、宇宙機の手法にはSPARTAマトリクス、そして攻撃者、能力、インフラ、被害者を結ぶダイヤモンドモデルを使うことで、各層の証拠に共通の構造を与えます。
* **層をまたいで仮説を検証する**: リンクが劣化したら、宇宙天気で説明できるか、同じ瞬間に認証の失敗が増えたか、関係する地上局にどの地上アカウントが触れたかを確かめます。散らばった信号を、検証できる説明へと変えるのです。

### 3. 全体像を組み立てるのはAI、解釈するのは人
規模に応じた統合と、説明責任のある結論:

* **量とそろえ作業はAIが担う**: モデルは何百万件もの事象を統合し、どれが同じ出来事に属するかを示し、要約の時系列を起案できます。大きな衛星群では、人が行えば何日もかかる作業です。
* **AIはもっともらしいパターンに惑わされることがある**: 相関のモデルは、無関係な事象を結びつけたり、しきい値の下にとどまるよう設計されたゆっくりした攻撃を見逃したりすることがあります。またNIST AI 100-2e2025の攻撃分類は、その入力が操作され得ることを示しています。そのため、AIの結論は仮説として扱います。
* **帰属判断の規則（提案）**: AIは、複数の事象が1つのインシデントを成すことを提案し、考えられる手法を示してかまいません。しかし、インシデントの宣言、攻撃者の特定、Space ISACなどの協力先への報告には、有資格の主任分析担当者の確認と承認を必須とします。

### 4. 本当の相関エンジンとしての多様なチーム
共同のローテーション、公正な機会、および専門職の基準:

* **経歴が違えば気づく手がかりも違う**: 光の技術者は普段と違う再捕捉のパターンに、ネットワークの分析担当者は定期的な外部への通信に、運用者はミッション上意味をなさない指令に気づきます。混成チームは、どの専門家も一人では見逃すものを捉えます。
* **ローテーションが多くの人に幅広い専門性を育てる**: リンク、ネットワーク、地上、運用の間で人員を交代させることで、有能な防御者の大きな層が育ち、少数の専門家や1つのAIシステムへの依存を避けられます。
* **CISSPが共通の枠組みを与える**: CISSPの8つのドメインは、アーキテクチャ、ID、運用、ガバナンスを結びつけます。それにより、あらゆる層の専門家が、リスクを話し合い、指導的な役割へと成長するための共通の基盤を持てます。

### 5. 結論
宇宙システムへの攻撃は、光、ネットワーク、地上、ミッションの各層にその痕跡を散らします。それらの痕跡を1つの明確な全体像にまとめられるのは、層をまたぐ視点だけです。

AIはその視点を大規模に実現し、多様な有資格者のチームは、相関を健全な判断へと変える文脈と説明責任を担います。そうしたチームに投資する組織は、どの自動化ツールも単独では提供できない防御を手にします。
