# Koki's Technical Paper — Space Cyber Defense Series SCD-025

## The Authentic Image — Detecting Manipulated and Synthetic Satellite Imagery

### Summary Digest
Satellite imagery has long been one of the most trusted forms of visual evidence, used by journalists, researchers, and governments to check whether events really happened. Generative AI is challenging that trust. During a 2026 armed conflict, an AI-altered satellite image depicting a destroyed military base gained millions of views across platforms, and in late July 2026 a major online mapping platform withdrew, about a day after launch, a feature that let users create AI-generated scenes on top of real satellite imagery, after researchers showed it could produce convincing fake disasters and military sites. Detection research is growing, but studies show that detectors often lose much of their laboratory accuracy on real-world media.

This main paper of SCD-025 introduces the defense of authentic imagery. It applies CISSP Domains 3, 7, and 2, explains how decision risks, detection limits, metadata checks, frequency analysis, and human review fit together, and shows why people must make final judgments.

---
### 1. Why Authentic Imagery Matters
The Reference Layer of Truth:

* **Imagery Is Used to Verify Other Claims**: Researchers compare videos and reports with satellite images, so faked imagery attacks the tool people use to check the truth.
* **Fakes Can Inherit Trust**: An image that appears to come from a familiar satellite or map service may be believed simply because of where it seems to come from.
* **Real Events Can Be Denied**: The existence of easy fakes also lets people falsely dismiss genuine imagery as fake, a problem sometimes called the liar's dividend.

### 2. Five Lines of Defense for Imagery
A Structure for the SCD-025 Series:

* **Understand the Threat and the Limits**: SCD-025-1 explains how synthetic imagery can mislead decisions, and SCD-025-2 describes why detection is an ongoing contest.
* **Check the Source**: SCD-025-3 explains metadata, provenance, and orbital checks that verify where an image came from.
* **Examine the Image and Decide Carefully**: SCD-025-4 describes frequency-domain analysis, and SCD-025-5 describes generator artifacts and the role of human review.

### 3. AI Detection Under Human Judgment
Machines Flag, People Decide:

* **AI Detectors Help at Scale**: Detection models can screen large numbers of images and flag those with signs of manipulation for closer review.
* **Detectors Are Fragile**: Simple edits such as compression can reduce detector accuracy, and new generators can defeat older detectors, consistent with NIST AI 100-2e2025.
* **Proposed Authentic Image Rule**: AI may screen imagery and estimate the likelihood of manipulation, but publicly declaring an image fake or genuine, or using imagery as evidence for consequential decisions, requires review by qualified analysts using multiple independent checks.

### 4. Image Analysts as Guardians of Evidence
Skill and Care Protect Truth:

* **Open-Source Investigators Are Essential**: Analysts who compare imagery with orbital data, ground photos, and other sources provide judgment no single tool can.
* **Collaboration Across Organizations**: Imagery providers, newsrooms, researchers, and security teams sharing methods and examples strengthen everyone's ability to spot fakes.
* **CISSP Supports Image Integrity**: CISSP Domain 3 covers cryptographic signatures and integrity, Domain 7 covers investigations and evidence, and Domain 2 covers data provenance and handling.

### 5. Conclusion
When satellite imagery can be faked in minutes, protecting authentic imagery becomes part of protecting the truth itself.

Understanding how fakes mislead, recognizing the limits of detectors, checking metadata and provenance, analyzing image structure, combining AI screening with expert human review, and sharing knowledge across organizations together keep satellite imagery a trustworthy window on the world.

---
# テクニカルペーパー 宇宙サイバー防衛シリーズ SCD-025

## 本物の画像 — 改ざんされた衛星画像と合成された衛星画像を見分ける

### サマリー・ダイジェスト
衛星画像は長いあいだ、もっとも信頼される見た目の証拠のひとつで、記者、研究者、政府が、出来事が本当に起きたかを確かめるのに使ってきました。生成AIは、その信頼を揺るがしています。2026年のある武力紛争の間には、壊された軍の基地を描いた、AIで手を加えた衛星画像が、さまざまなプラットフォームで何百万回も見られました。また2026年7月の終わりには、ある大手のオンライン地図のサービスが、本物の衛星画像の上にAIで作った場面を重ねられる機能を、公開から約1日で取り下げました。研究者が、それで本物らしい偽の災害や軍の施設を作れることを示したためです。見分ける研究は増えていますが、検出の仕組みは実際の世界のメディアでは、実験室での正確さの多くを失うことが多いと、研究は示しています。

SCD-025の本編である本論文は、本物の画像を守ることを紹介します。CISSPのドメイン3、7、2を適用し、判断のリスク、検出の限界、メタデータの確認、周波数の分析、人の確認がどう組み合わさるかを説明し、最終の判断を人が下さなければならない理由を示します。

---
### 1. 本物の画像が大切な理由
真実を確かめるための基準の層:

* **画像はほかの主張を確かめるのに使われる**: 研究者は動画や報告を衛星画像と比べるため、偽の画像は、人が真実を確かめるための道具そのものを攻撃します。
* **偽物は信頼を受け継ぐことがある**: なじみのある衛星や地図のサービスから来たように見える画像は、どこから来たように見えるかというだけで信じられてしまうことがあります。
* **本当の出来事が否定されうる**: 簡単に偽物を作れるようになると、本物の画像を偽物だとうそをついて退けることもできてしまいます。これは「うそつきの配当」と呼ばれることがある問題です。

### 2. 画像を守る5つの守りの線
SCD-025シリーズの構成:

* **脅威と限界を理解する**: SCD-025-1は合成画像がどう判断を誤らせるかを、SCD-025-2は検出がなぜ続いていく競い合いなのかを説明します。
* **出どころを確かめる**: SCD-025-3は、画像がどこから来たかを確かめる、メタデータ、来歴、軌道の確認を説明します。
* **画像を調べ、慎重に決める**: SCD-025-4は周波数の領域の分析を、SCD-025-5は生成の痕跡と人の確認の役割を説明します。

### 3. 人の判断の下での、AIの検出
機械が印を付け、人が決める:

* **AIの検出は大きな規模で役立つ**: 検出のモデルは大量の画像をふるいにかけ、改ざんのしるしがあるものに印を付けて、くわしい確認に回せます。
* **検出の仕組みはもろい**: 圧縮のような簡単な編集で検出の正確さが下がることがあり、新しい生成の道具は古い検出の仕組みを打ち負かせます。これはNIST AI 100-2e2025と同じ趣旨です。
* **本物の画像の規則（提案）**: AIは画像をふるいにかけ、改ざんの可能性を見積もってかまいません。しかし、画像を公に偽物または本物と宣言すること、重大な判断の証拠として画像を使うことには、複数の独立した確認を使う有資格の分析担当者の確認が必要です。

### 4. 証拠の守り手としての画像の分析担当者
技能と注意が真実を守る:

* **公開情報の調査担当者が欠かせない**: 画像を軌道のデータ、地上の写真、ほかの源と比べる分析担当者は、どの道具だけでも与えられない判断をもたらします。
* **組織を越えた協力**: 画像の提供者、報道機関、研究者、セキュリティのチームがやり方と例を分け合うことで、みんなの偽物を見抜く力が強まります。
* **CISSPが画像の完全性を支える**: CISSPのドメイン3は暗号の署名と完全性を、ドメイン7は調査と証拠を、ドメイン2はデータの来歴と取り扱いを扱います。

### 5. 結論
衛星画像が数分で偽造できるとき、本物の画像を守ることは、真実そのものを守ることの一部になります。

偽物がどう惑わせるかを理解し、検出の仕組みの限界を知り、メタデータと来歴を確かめ、画像のつくりを分析し、AIのふるい分けと専門家の人の確認を組み合わせ、組織を越えて知識を分け合うことで、衛星画像は、世界を見る信頼できる窓であり続けます。
