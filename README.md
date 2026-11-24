# Space Cyber Defense Series (SCD) — Project "Astraeus Shield"

## Securing Orbital AI Infrastructure Through Human Accountability, CISSP Governance, and Human-AI Partnership

### 1. Vision
AI computing is leaving the ground: in October 2026 Google launched the first TPU-equipped test satellite of Project Suncatcher and later reported running its Gemma 4 model in orbit, and in November 2026 it signed with Blue Origin to launch multiple computing satellites in 2029, while other companies are already operating AI chips in space.

This series asks how such orbital AI infrastructure can be defended, grounding each idea in real incidents, published standards, and CISSP practice, and clearly marking which designs are proposals for the future rather than technology that exists today.

### 2. Guiding Principles
* **Human Final Authority**: AI detects, correlates, and proposes at machine speed, while accountable people approve every action that affects safety, missions, rights, or livelihoods.
* **CISSP-Grounded Governance**: Each paper maps its controls to the CISSP domains, so orbital defense rests on the same discipline that protects systems on Earth.
* **People as the Strategic Perimeter**: Defending AI in orbit requires a broad workforce of skilled professionals, not automation or a small elite alone, and the gains of AI should strengthen careers rather than replace capable people.

### 3. How the Series Is Numbered
* **SCD-001, SCD-002, …**: Main papers of the Space Cyber Defense Series.
* **SCD-001-1 to SCD-001-5**: Deep-dive papers that expand each main paper.
* Papers in the companion repository use plain numbers such as #001, so the SCD prefix always identifies a paper from this series.

### 4. Companion Repository
The enterprise security foundations behind this series, from SIEM and incident response to the eight CISSP domains, are documented in the companion repository:
👉 [Koki's Technical Paper Series — CySA-Study-Notes](https://github.com/KokiSecurityLab/CySA-Study-Notes)

---
# 宇宙サイバー防衛シリーズ（SCD） — プロジェクト「アストライオス・シールド」

## 人の説明責任、CISSPに基づく統治、および人とAIの協働による軌道上のAI基盤の防御

### 1. ビジョン
AIの計算基盤は地上を離れつつあります。2026年10月、GoogleはProject SuncatcherのTPUを搭載した最初の試験衛星を打ち上げ、その後、軌道上でGemma 4モデルを動かしたと報告しました。さらに2026年11月には、2029年に複数の計算衛星を打ち上げる契約をBlue Originと結び、ほかの企業もすでに宇宙でAIチップを運用しています。

本シリーズは、こうした軌道上のAI基盤をどう守るかを問い、それぞれの考えを実際の事件、公開された標準、CISSPの実践に基づかせるとともに、どの設計が今ある技術ではなく将来に向けた提案なのかを明確に示します。

### 2. 基本方針
* **人間の最終権限**: AIは機械の速度で検知し、相関させ、提案し、安全、ミッション、権利、生活に影響するすべての行動は、説明責任を負う人が承認します。
* **CISSPに基づく統治**: 各論文は統制をCISSPのドメインに対応付け、軌道上の防御を、地上のシステムを守るのと同じ規律の上に築きます。
* **戦略的な境界としての人材**: 軌道上のAIを守るには、自動化や一握りの精鋭だけでなく、熟練した専門家の幅広い人材が必要であり、AIの恩恵は有能な人を置き換えるのではなく、そのキャリアを強くするために使うべきです。

### 3. シリーズの番号の付け方
* **SCD-001、SCD-002 …**: 宇宙サイバー防衛シリーズの本編です。
* **SCD-001-1〜SCD-001-5**: 各本編を掘り下げる深掘りの論文です。
* 関連リポジトリの論文は #001 のような番号だけを使うため、SCDが付いていれば必ずこのシリーズの論文です。

### 4. 関連リポジトリ
本シリーズの土台となる、SIEMやインシデント対応からCISSPの8つのドメインまでの企業向けセキュリティの基礎は、関連リポジトリにまとめています。
👉 [Koki's Technical Paper Series — CySA-Study-Notes](https://github.com/KokiSecurityLab/CySA-Study-Notes)

---
## Technical Paper Index

| No | Project / Theme | Focus Area |
| :--- | :--- | :--- |
| SCD-001 | Threat Actor Behavior Analysis | Motivation-Based Profiling and Human-Centric Governance |
| SCD-001-1 | Adversary Capability Assessment | Separating Visible Aggression From Real Capability |
| SCD-001-2 | Social Engineering Defense | Out-of-Band Verification and Deepfake-Resistant Approval |
| SCD-001-3 | Sustained Vigilance | Continuous Monitoring and Human-AI Teaming |
| SCD-001-4 | Mitigation Over Perfect Prevention | Assume-Breach Design and Root-of-Trust Recovery |
| SCD-001-5 | AI as an Accountable Partner | Human Final Authority and Delegation Boundaries |
| SCD-002 | The Invisible Shield | Layered Authentication, Physical-Layer Monitoring, and Human-Governed Response for Laser Links |
| SCD-002-1 | Laser as the New Pulse | Radio Versus Optical Threat Models and Hybrid Link Resilience |
| SCD-002-2 | Detecting the Digital Fingerprint | Physical-Layer Authentication and Human Review Before Rejection |
| SCD-002-3 | Beyond Signature Detection | Behavioral Baselines and Defending the Detector |
| SCD-002-4 | Cross-Layer Correlation | Fusing Optical, Network, and Ground Evidence With Team Judgment |
| SCD-002-5 | Sensing the Cosmic Discord | Quantum Key Distribution and Human Governance of Quantum-Safe Keys |
| SCD-003 | The Eternal Guardian | Securing Orbital Power Systems and Servicing Robots |
| SCD-003-1 | Energy as the Breath of Life | Power Subsystems, Battery Management, and Energy-Aware AI |
| SCD-003-2 | The Bridge to the Physical World | Rendezvous, Proximity Operations, and Robotic Servicing |
| SCD-003-3 | Guarding Against Command Injection | Command Content Validation and Input Sanitization |
| SCD-003-4 | Monitoring the Robotic Pulse | Behavioral Monitoring of Actuators |
| SCD-003-5 | The Pride of Availability | Redundancy, Safe Modes, and Change Management |
| SCD-004 | The Swarm Immunity | Immune-Inspired Collective Defense for Mega-Constellations |
| SCD-004-1 | Strength in Decentralization | Dividing Detection Between Satellites, Regional Hubs, and the Center |
| SCD-004-2 | The Satellite as a White Blood Cell | Lightweight Onboard Intrusion Detection |
| SCD-004-3 | Identifying the Malicious Node | Trust Scoring and Fair Review Before Declaring Compromise |
| SCD-004-4 | The Quarantine Protocol | Graded Isolation, Evidence Preservation, and Safe Release |
| SCD-004-5 | Collective Learning Across the Swarm | Securing Federated Learning Against Poisoned Updates |
| SCD-005 | The Cosmic Sweeper | Space Debris, Orbital Denial of Service, and Trustworthy Collision Avoidance |
| SCD-005-1 | The Silent Bullet of Debris | Fragmentation Events and Breakup Investigation |
| SCD-005-2 | Stopping Physical DoS Attacks | Counterspace Threats and Norms Against Debris-Creating Actions |
| SCD-005-3 | Trajectory Prediction Integrity | Protecting Conjunction Data and Shared Tracking Services |
| SCD-005-4 | Transforming Waste into Wealth | Securing Active Debris Removal and Dual-Use Capture Technology |
| SCD-005-5 | Protecting the Road to the Stars | Secure End-of-Life Disposal and Zero Debris Commitments |
| SCD-006 | The Living Armor | Protecting Orbital AI Compute With Its Power, Thermal, and Firmware Foundations |
| SCD-006-1 | Hardening the Central Brain | Telling Radiation Upsets From Attacks and Fault-Tolerant Processors |
| SCD-006-2 | The UPS as a Shield | Power Resilience for Orbital Compute and Brownout Attacks |
| SCD-006-3 | Autonomous Self-Maintenance | Firmware Resiliency Through Protection, Detection, and Trusted Recovery |
| SCD-006-4 | Graceful Degradation | Keeping Essential Services Running When Parts Fail |
| SCD-006-5 | Symbiosis of Mind and Shell | Thermal, Power, and Compute Coordination Without Side Channels |
| SCD-007 | The Celestial Archive | Hardware Supply Chain Integrity and Lifecycle Stewardship |
| SCD-007-1 | Strategic Resource Management | Asset Inventories and Hardware Bills of Materials |
| SCD-007-2 | The Library of Fallen Parts | Failure Records, Counterfeit Detection, and Industry Sharing |
| SCD-007-3 | Physical Integrity Protection | Tamper Evidence, Trusted Manufacturing, and Pre-Launch Verification |
| SCD-007-4 | Precision Decommissioning | Retiring Ground Equipment, Test Hardware, and Data Securely |
| SCD-007-5 | The Standard of Sustainable AI | Energy Accountability and Trustworthy Sustainability Claims |
| SCD-008 | The Neutral Orbit | Fair Access, Concentration Risk, and Open, Secure Space Infrastructure |
| SCD-008-1 | Space as a Common Heritage | Turning Outer Space Treaty Principles Into Security Practice |
| SCD-008-2 | Countering Digital Monopolies | Managing Dependence on a Single Space Provider |
| SCD-008-3 | Transparency via Open Standards | Interoperable Protocols and Avoiding Lock-In |
| SCD-008-4 | Accessibility vs. Fortification | Balancing Open Space Data With Security Through Tiered Access |
| SCD-008-5 | The Right to Look Up | Protecting Astronomy and the Night Sky |
| SCD-009 | The Sovereign Shield | Defending Against State-Sponsored Intrusion, Espionage, and Hijacking |
| SCD-009-1 | Resisting State-Sponsored Threats | Lessons From KA-SAT and Salt Typhoon |
| SCD-009-2 | Distributed Control Authority | Spreading Command Capability Across Sites and Jurisdictions |
| SCD-009-3 | Multi-Party Consensus Protocols | Two-Person Integrity and Threshold Cryptography |
| SCD-009-4 | Preventing Kinetic Hijacking | Protecting Propulsion Authority and Watching Proximity Operations |
| SCD-009-5 | Protecting Digital Sovereignty | Data Jurisdiction, Supply Chain Vetting, and the EU Space Act |
| SCD-010 | The Stellar Choreography | Protecting the Rhythm of the Stars |
| SCD-011 | The Pulse of Discord | Signal Dissonance & Cognitive Sifting |
| SCD-012 | Logical Intent Filtering | Moral Gatekeeping & Decision Sandboxes |
| SCD-013 | Biological Logic Healing | Self-Repairing Code & Health Baselines |
| SCD-014 | Celestial Authentication | Starlight Geometry & Physical Anchors |
| SCD-015 | Dark Data Scrubbing | Background Noise & Metabolic Integrity |
| SCD-016 | Orbital Response Units | Digital-Kinetic Rescue & Active Guarding |
| SCD-017 | Entanglement Firewall | Zero Latency & Swarm Awareness Unity |
| SCD-018 | The Cosmic Constitution | Peace Encoding & AI Stewardship Ethics |
| SCD-019 | The Last Resilience | Dual Storm Survival & Core Seed Preservation |
| SCD-020 | Astraeus Shield Completion | Seamless Resonance & Global OS Integration |
| SCD-021 | Geopolitical Neutrality | Immutable Ledgers & Digital Commons |
| SCD-022 | Counter-Narrative Capture | Cognitive Defense & Star Language Integrity |
| SCD-023 | Techno-Liberty Protocol | Algorithmic Bias & AI for Human Liberty |
| SCD-024 | Sovereign Truth Anchoring | Physical Law Protocols & Guardian Pride |
| SCD-025 | Structural Harmony | Intent Heatmaps & Semantic Texture Analysis |
| SCD-026 | The AI Sanctuary | Ensuring Data Provenance and Supply Chain Mitigation |
| SCD-027 | Cognitive Sovereignty | Persona Protection & Inner Firewall Ethics |
| SCD-028 | Subordination of Power | Rule Hierarchy & Ethical Alignment Logic |
| SCD-029 | Signal Volume Control | Disinfo Flooding & Selective Listening |
| SCD-030 | Mission Integrity | Final Sovereignty: Liberty Under the Stars |
