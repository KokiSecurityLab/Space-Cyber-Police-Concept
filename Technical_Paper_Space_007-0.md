# Koki's Technical Paper — Space Cyber Defense Series SCD-007

## The Celestial Archive — Hardware Supply Chain Integrity and Lifecycle Stewardship for Orbital Platforms

### Summary Digest
Every satellite is built from thousands of parts made by many suppliers, and governments are raising expectations for how those parts are tracked: CISA published a Hardware Bill of Materials framework in September 2023, and under the EU Cyber Resilience Act, reporting obligations for products with digital elements have applied since September 11, 2026, with full obligations from December 11, 2027.

This paper applies CISSP Domains 1 and 3 to the full lifecycle of orbital hardware, from sourcing and manufacturing through operation and retirement, and argues that a trustworthy record of every component, maintained by people and supported by AI, is the archive on which space security depends.

---
### 1. Why the Supply Chain Is a Space Security Problem
Many Hands, Long Lifetimes, No Second Chances:

* **Components Come From Everywhere**: Processors, memory, radios, and sensors may be designed in one country, made in another, and assembled in a third, so a weakness introduced anywhere can travel into orbit.
* **Flaws Cannot Be Recalled From Orbit**: On Earth, a faulty part can be replaced, but a compromised or counterfeit component launched into space stays there for the life of the mission.
* **Lifetimes Outlast Suppliers**: Satellites may operate for many years, during which suppliers change, parts become obsolete, and new vulnerabilities are discovered in components already in orbit.

### 2. Building the Celestial Archive
Records That Follow Hardware From Birth to Retirement:

* **Know What Is Inside**: A hardware bill of materials lists components, manufacturers, and origins, and CISA's framework provides a consistent format so that buyers and suppliers can share this information reliably.
* **Manage Supplier Risk Systematically**: NIST SP 800-161 Revision 1, published in May 2022 and updated in November 2024, guides organizations in identifying, assessing, and responding to cybersecurity risks at every level of the supply chain.
* **Keep the Record Alive**: The archive is updated as vulnerabilities are disclosed, parts fail, and spacecraft are retired, so operators can quickly find which satellites contain an affected component.

### 3. AI-Assisted Analysis Under Human Stewardship
Using AI to Search the Archive Without Trusting It Blindly:

* **AI Finds Patterns Across Thousands of Parts**: Models can match new vulnerability reports to components in the archive, flag suppliers with unusual histories, and spot inconsistencies between documents and test results.
* **The Archive Itself Can Be Poisoned**: Falsified supplier records or manipulated test data could lead AI tools to approve unsafe parts, the data poisoning risk described in NIST AI 100-2e2025, so sources are authenticated and changes are logged.
* **Proposed Supply Chain Approval Rule**: AI may screen suppliers and parts and recommend decisions, but approving a new supplier for flight hardware, accepting a part with an unresolved anomaly, or waiving a supply chain requirement requires approval by qualified engineering and security reviewers.

### 4. The People Who Keep the Archive Honest
Quality Engineers, Supply Chain Analysts, and Shared Standards:

* **Supply Chain Security Is Human Work**: Inspecting parts, auditing suppliers, and judging whether documentation is trustworthy require experience that AI tools support but cannot replace.
* **Many Organizations Must Participate**: Large primes, small suppliers, and testing laboratories all hold parts of the record, and training people across this ecosystem spreads both responsibility and opportunity.
* **CISSP Connects Supply Chain and Governance**: CISSP Domain 1 covers supply chain risk management and governance, and Domain 3 covers secure design, giving professionals a common framework for lifecycle stewardship.

### 5. Conclusion
Orbital platforms inherit every strength and weakness of the parts they are built from, and those parts cannot be replaced once they are launched.

A living archive of hardware components, systematic supplier risk management, AI that searches the record under human oversight, and qualified people who make the final approvals give space systems a foundation of trust from the factory floor to retirement.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-007

## 天空の記録庫 — 軌道上の基盤のためのハードウェアのサプライチェーンの完全性とライフサイクルの管理

### サマリー・ダイジェスト
どの衛星も、多くの供給元が作った何千もの部品からできています。そして各国の政府は、それらの部品の追跡についての期待を高めています。米国のCISAは2023年9月に「ハードウェア部品表（HBOM）」の枠組みを公表しました。EUのサイバーレジリエンス法のもとでは、デジタルの要素を持つ製品について、2026年9月11日から報告の義務が適用され、2027年12月11日からは義務の全体が適用されます。

本論文はCISSPのドメイン1と3を、調達と製造から運用と引退までの、軌道上のハードウェアのライフサイクル全体に適用します。そして、人が維持し、AIが支える、すべての部品についての信頼できる記録こそが、宇宙のセキュリティが拠って立つ「記録庫」であると論じます。

---
### 1. サプライチェーンが宇宙のセキュリティの問題である理由
多くの手、長い寿命、やり直しのきかない世界:

* **部品はあらゆる場所から来る**: プロセッサー、メモリー、無線機、センサーは、ある国で設計され、別の国で作られ、さらに別の国で組み立てられることがあります。どこかで入り込んだ弱点が、そのまま軌道まで運ばれます。
* **欠陥を軌道から回収することはできない**: 地上なら欠陥のある部品は交換できますが、侵害された部品や偽造品が宇宙に打ち上げられると、ミッションが終わるまでそこに残ります。
* **寿命が供給元より長い**: 衛星は何年も動き続けることがあり、その間に供給元が変わり、部品は生産終了となり、すでに軌道上にある部品で新しい脆弱性が見つかります。

### 2. 天空の記録庫を築く
誕生から引退までハードウェアに付いていく記録:

* **中に何が入っているかを知る**: ハードウェア部品表は、部品、製造元、出どころを一覧にします。CISAの枠組みは一貫した形式を示し、買い手と供給元がこの情報を確実に共有できるようにします。
* **供給元のリスクを体系的に管理する**: 2022年5月に公表され、2024年11月に更新されたNIST SP 800-161 第1版は、サプライチェーンのあらゆる段階で、サイバーセキュリティのリスクを見つけ、評価し、対応する方法を組織に示しています。
* **記録を生きたものに保つ**: 記録庫は、脆弱性が公表されたとき、部品が故障したとき、宇宙機が引退したときに更新します。そうすれば、影響を受ける部品を積んだ衛星を、運用者がすぐに見つけられます。

### 3. 人の管理のもとでのAIによる分析
記録庫をやみくもに信じずに、AIで探す:

* **AIは何千もの部品にまたがるパターンを見つける**: モデルは、新しい脆弱性の報告を記録庫の部品と照らし合わせ、普段と違う経歴を持つ供給元を示し、書類と試験結果の食い違いを見つけられます。
* **記録庫そのものが汚染され得る**: 偽造された供給元の記録や操作された試験データは、AIツールに安全でない部品を承認させかねません。これはNIST AI 100-2e2025が示すデータ汚染のリスクです。そのため、情報源を認証し、変更を記録します。
* **サプライチェーン承認の規則（提案）**: AIは供給元と部品を選別し、判断を推奨してかまいません。しかし、飛行用ハードウェアの新しい供給元の承認、未解決の異常を抱えた部品の受け入れ、サプライチェーンの要件の免除には、有資格の技術とセキュリティの確認者の承認を必須とします。

### 4. 記録庫を正直に保つ人々
品質の技術者、サプライチェーンの分析担当者、および共通の基準:

* **サプライチェーンのセキュリティは人の仕事**: 部品を検査し、供給元を監査し、書類が信頼できるかを判断するには、AIツールが支えることはできても置き換えることはできない経験が必要です。
* **多くの組織が参加しなければならない**: 大手の元請け、小さな供給元、試験機関は、それぞれ記録の一部を持っています。このつながり全体で人を育てることで、責任と機会の両方が広がります。
* **CISSPがサプライチェーンとガバナンスを結ぶ**: CISSPのドメイン1はサプライチェーンのリスク管理とガバナンスを、ドメイン3は安全な設計を扱い、ライフサイクルの管理のための共通の枠組みを専門家に与えます。

### 5. 結論
軌道上の基盤は、それを作る部品のあらゆる強さと弱さを受け継ぎ、それらの部品は打ち上げた後には交換できません。

ハードウェア部品の生きた記録庫、体系的な供給元のリスク管理、人の監督のもとで記録を探すAI、そして最終的な承認を行う有資格の人々が、工場の床から引退まで、宇宙システムに信頼の土台を与えます。
