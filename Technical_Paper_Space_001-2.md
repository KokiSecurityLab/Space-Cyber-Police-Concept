# Koki's Technical Paper — Space Cyber Defense Series SCD-001-2

## Social Engineering Defense — Out-of-Band Verification, Deepfake-Resistant Approval, and Protecting the People Who Hold the Keys

### Summary Digest
Strong encryption does not stop an attacker who persuades an authorized person to act, as Arup learned in early 2024 when an employee in Hong Kong joined a video call in which every apparent colleague, including the chief financial officer, was an AI-generated deepfake and then sent HK$200 million, about US$25.6 million, in 15 transfers.

For the operators who approve commands, keys, and payments in space programs, this paper applies CISSP Domains 1 and 5 to build verification that does not depend on recognizing a face or voice, uses AI to flag manipulation, and treats trained, respected staff as the defense that deepfakes are designed to defeat.

---
### 1. Why Trusted People Are the Preferred Target
How Social Engineering Bypasses Technical Controls:

* **Persuasion Costs Less Than Cryptanalysis**: Breaking modern encryption is impractical, while convincing one administrator to approve a request is cheap, so attackers invest in researching the people who can reset credentials, release funds, or authorize uplink commands.
* **Deepfakes Defeat Recognition**: In the Arup case, the employee initially doubted the request but put the doubts aside because the people on the call looked and sounded like familiar colleagues, showing that seeing and hearing are no longer proof of identity.
* **Authority and Urgency as Weapons**: Messages framed as confidential, urgent instructions from senior leaders pressure staff to skip procedure, and AI now lets attackers write such messages fluently in any language and tone.

### 2. Verification That Does Not Rely on Recognition
Process Controls Built Into the Workflow:

* **Out-of-Band Confirmation for High-Impact Requests**: Any request to move money, change credentials, or send critical commands is confirmed through a separate, pre-registered channel, such as a call back to a number from the directory, never through contact details supplied in the request itself.
* **Multi-Person Approval for Irreversible Actions**: Large transfers, key releases, and commands that could endanger a spacecraft require two independent, authorized approvers, so deceiving one person is not enough.
* **Phishing-Resistant Authentication**: FIDO2 security keys and passkeys bind sign-in to the legitimate site and device, so credentials harvested through a convincing fake page cannot be replayed by the attacker.

### 3. AI as an Early Warning, People as the Decision
Detection Support Under Human Authority:

* **AI Screens Messages and Media for Manipulation**: Defensive AI flags impersonation patterns, mismatched sending infrastructure, unusual payment instructions, and possible synthetic audio or video, and attaches its reasons so staff can judge the warning.
* **The Final Decision Stays With a Trained Person**: Detection tools miss new deepfake methods and can raise false alarms, so the authority to approve or refuse remains with a qualified employee who follows the verification procedure regardless of what any screen shows.
* **Reporting Without Blame**: Staff who pause a suspicious request or report a mistake are thanked, not punished, because a culture that blames victims teaches people to hide the very signals that stop fraud.

### 4. Protecting the People Who Hold the Keys
Training, Authority, and Respect for Professional Judgment:

* **Realistic, Recurring Training**: Exercises include deepfake voice and video scenarios relevant to each role, so finance staff, ground-station operators, and administrators practice saying no to convincing requests before a real one arrives.
* **Authority to Refuse Without Fear**: Policy states clearly that following verification steps is never insubordination, even when the request appears to come from the most senior leader, and CISSP-qualified security leaders defend staff who apply it.
* **Skilled Staff Are the Control, Not the Cost**: Organizations that cut experienced employees and hand approvals to automated workflows remove the human judgment deepfakes cannot easily fool, so investing in capable people is a direct security measure and part of a future in which AI strengthens workers rather than replaces them.

### 5. Conclusion
Social engineering succeeds by exploiting trust in familiar faces and voices, and as the Arup deepfake loss demonstrated, AI has made that trust unreliable unless identity is confirmed through independent channels and shared approval.

Out-of-band confirmation, multi-person approval for irreversible actions, phishing-resistant keys, AI that warns but does not decide, and trained staff empowered to refuse together keep the people who hold the keys to orbital systems from becoming the attacker's easiest path.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-001-2

## ソーシャルエンジニアリング対策 — 別経路での確認、ディープフェイクに強い承認、および鍵を預かる人々の保護

### サマリー・ダイジェスト
強力な暗号も、権限のある人を説得して行動させる攻撃者は止められません。Arupは2024年初めにこのことを思い知りました。香港の従業員がビデオ会議に参加したところ、最高財務責任者を含む同僚に見えた全員がAIで作られたディープフェイクで、その従業員は15回の送金で2億香港ドル、約2,560万米ドルを送ってしまいました。

本論文は、宇宙計画で指令、鍵、支払いを承認する担当者のために、CISSPのドメイン1と5を適用します。顔や声の識別に頼らない確認の仕組みを築き、AIで操作の兆候を知らせ、訓練を受けて尊重される職員を、ディープフェイクが打ち破ろうとする防御そのものとして扱います。

---
### 1. 信頼される人が好んで狙われる理由
ソーシャルエンジニアリングが技術的な統制を回避する経緯:

* **暗号解読より安い説得**: 現代の暗号を破ることは現実的ではない一方、管理者一人に依頼を承認させるのは安上がりです。そのため攻撃者は、資格情報の再設定、資金の払い出し、上り回線の指令の承認ができる人々の調査に力を注ぎます。
* **識別を打ち破るディープフェイク**: Arupの事例では、従業員は当初は依頼を疑ったものの、会議の参加者が見慣れた同僚のように見え、聞こえたため、疑いを脇に置きました。見ることと聞くことは、もはや身元の証明にならないことを示しています。
* **武器としての権威と緊急性**: 上級幹部からの機密で緊急の指示という形をとった連絡は、職員に手順を飛ばすよう圧力をかけます。そしてAIにより、攻撃者はそうした文面をどの言語や口調でも流暢に書けるようになりました。

### 2. 識別に頼らない確認
業務の流れに組み込んだ手順上の統制:

* **影響の大きい依頼の別経路での確認**: 送金、資格情報の変更、重要な指令の送信の依頼は、名簿にある番号へ折り返し電話をかけるなど、事前に登録した別の経路で確認します。依頼そのものに書かれた連絡先は決して使いません。
* **取り消せない操作の複数人承認**: 高額の送金、鍵の払い出し、宇宙機を危険にさらし得る指令には、権限を持つ独立した二人の承認を必要とし、一人をだますだけでは足りないようにします。
* **フィッシング耐性のある認証**: FIDO2のセキュリティキーとパスキーはサインインを正規のサイトと機器に結びつけるため、巧妙な偽のページで集めた資格情報を攻撃者が再利用することはできません。

### 3. 早期警告としてのAI、判断するのは人
人の権限のもとでの検知の支援:

* **操作の兆候を調べるAI**: 防御のAIは、なりすましのパターン、送信基盤の不一致、普段と違う支払いの指示、合成された可能性のある音声や映像を示し、その理由を添えて、職員が警告を判断できるようにします。
* **最終判断は訓練を受けた人に**: 検知ツールは新しいディープフェイクの手法を見逃すことも誤った警報を出すこともあるため、承認または拒否の権限は、どの画面に何が表示されても確認の手順に従う有資格の職員に残します。
* **責めない報告**: 疑わしい依頼を止めた職員や、誤りを報告した職員は、罰せられるのではなく感謝されます。被害者を責める文化は、まさに詐欺を止める兆候を隠すことを人々に教えてしまうためです。

### 4. 鍵を預かる人々を守る
教育、権限、および専門的な判断の尊重:

* **現実的で繰り返される訓練**: 演習には、役割ごとに合わせたディープフェイクの音声や映像の場面を含め、財務担当者、地上局の運用担当者、管理者が、本物の依頼が来る前に、説得力のある依頼に「いいえ」と言う練習をします。
* **恐れずに断る権限**: 確認の手順に従うことは、依頼が最上位の幹部から来たように見えても決して不服従ではないと方針で明記し、CISSP資格を持つセキュリティの責任者が、それを適用した職員を守ります。
* **熟練した職員は費用ではなく統制**: 経験豊富な従業員を削減し、承認を自動化された流れに委ねる組織は、ディープフェイクが簡単にはだませない人間の判断を取り除いてしまいます。有能な人々への投資は直接的なセキュリティ対策であり、AIが働く人を置き換えるのではなく強くする未来の一部です。

### 5. 結論
ソーシャルエンジニアリングは見慣れた顔や声への信頼につけ込んで成功し、Arupのディープフェイクによる損失が示したように、AIは、独立した経路と共同の承認で身元を確かめない限り、その信頼を当てにならないものにしました。

別経路での確認、取り消せない操作の複数人承認、フィッシング耐性のある鍵、警告はしても判断はしないAI、そして断る権限を与えられた訓練済みの職員がそろうことで、軌道上のシステムの鍵を預かる人々が、攻撃者にとって最も簡単な経路になることを防ぎます。
