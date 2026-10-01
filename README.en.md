# Awesome Wi-Fi AI Offload

[한국어](README.md) | **English**

A collection of papers and standardization resources for AI inference offloading over Wi-Fi. Journal articles come first; magazine articles, conference papers and IEEE contributions are identified separately.

**Updated:** 2026-10-01 · **Papers:** 28 core + 1 adjacent topic · **Standards documents:** listed separately

This collection makes no claim to a formal venue ranking or an exhaustive literature review. Direct WLAN papers study 802.11 itself; Transferable papers offer MEC/edge-AI concepts or models that may inform Wi-Fi research. Neither label implies adoption by IEEE 802.11bu.

Each paper’s metadata-check date is recorded as `verified_on` in [papers.json](papers.json). The standards guide retains its own verification cutoff.

## Start here

- [Reading path and FLOPS/FLOPs research guide](docs/reading-guide.md)
- [IEEE AIO standardization resources](docs/ieee-contributions.en.md)
- [Structured bibliography](papers.json)
- [Contribution and verification criteria](CONTRIBUTING.md)

## Legend

- `Journal` peer-reviewed journal · `Magazine` scholarly magazine · `Conference` conference proceedings
- `WLAN` directly about IEEE 802.11 · `Transferable` applicable MEC/edge-AI ideas
- Years prioritize the verified final issue. An arXiv link may provide an accessible manuscript; it does not itself verify the final venue
- Links point to publishers and publicly accessible author versions. PDFs are not copied into this repository

## Quick index

Ordered as 25 journal articles → 1 magazine article → 3 conference papers, newest first within each group. Short titles support navigation; exact titles appear in the detailed entries below.

| Year | Paper (short title) | Venue · type | Topic |
| --- | --- | --- | --- |
| 2026 | [MAPC DRL Scheduling](https://doi.org/10.1109/TMLCN.2026.3682239) | IEEE TMLCN · Journal | [WLAN latency and coexistence](#wlan-latency-reliability-and-coexistence) |
| 2026 | [Robust DNN Partitioning](https://doi.org/10.1109/TMC.2025.3619509) | IEEE TMC · Journal | [Resources and scheduling](#resource-aware-admission-placement-and-scheduling) |
| 2026 | [Task-Aware DNN Partitioning](https://doi.org/10.1109/TMC.2025.3650680) | IEEE TMC · Journal | [Inference partitioning](#dnn-inference-offloading-and-partitioning) |
| 2025 | [Trustworthy Edge Intelligence](https://doi.org/10.1109/COMST.2024.3446585) | IEEE COMST · Journal | [Trust and security](#trustworthy-edge-intelligence) |
| 2025 | [Wi-Fi 8 Tutorial](https://doi.org/10.1134/S003294602502005X) | Problems of Information Transmission · Journal | [Standards writing](#standards-overview-and-tutorial-writing) |
| 2025 | [Dynamic DNN Inference (FIN)](https://doi.org/10.1109/TON.2025.3543848) | IEEE TON · Journal | [Resources and scheduling](#resource-aware-admission-placement-and-scheduling) |
| 2024 | [Fine-Grained DNN Partitioning](https://doi.org/10.1109/TMC.2024.3357874) | IEEE TMC · Journal | [Inference partitioning](#dnn-inference-offloading-and-partitioning) |
| 2024 | [Job Offloading Schedule](https://doi.org/10.1109/TMC.2023.3276937) | IEEE TMC · Journal | [Resources and scheduling](#resource-aware-admission-placement-and-scheduling) |
| 2024 | [Wi-Fi MLO Latency and Throughput](https://doi.org/10.1109/TNET.2023.3283154) | IEEE/ACM TON · Journal | [WLAN latency and coexistence](#wlan-latency-reliability-and-coexistence) |
| 2023 | [Multi-Agent Collaborative Inference](https://doi.org/10.1109/TMC.2022.3183098) | IEEE TMC · Journal | [Inference partitioning](#dnn-inference-offloading-and-partitioning) |
| 2023 | [Delay-Aware Inference Throughput](https://doi.org/10.1109/TMC.2021.3125949) | IEEE TMC · Journal | [Resources and scheduling](#resource-aware-admission-placement-and-scheduling) |
| 2022 | [HiveMind](https://doi.org/10.1109/JSAC.2021.3118403) | IEEE JSAC · Journal | [Resources and scheduling](#resource-aware-admission-placement-and-scheduling) |
| 2022 | [Task-Oriented Edge Communication](https://doi.org/10.1109/JSAC.2021.3126087) | IEEE JSAC · Journal | [Adjacent: feature communication](#adjacent-task-oriented-inference-communication) |
| 2021 | [CoEdge](https://doi.org/10.1109/TNET.2020.3042320) | IEEE/ACM TON · Journal | [Inference partitioning](#dnn-inference-offloading-and-partitioning) |
| 2021 | [JointDNN](https://doi.org/10.1109/TMC.2019.2947893) | IEEE TMC · Journal | [Inference partitioning](#dnn-inference-offloading-and-partitioning) |
| 2021 | [MLO Coexistence](https://doi.org/10.3390/s21237974) | Sensors · Journal | [WLAN latency and coexistence](#wlan-latency-reliability-and-coexistence) |
| 2021 | [802.11ax Spatial Reuse](https://doi.org/10.1016/j.comcom.2021.01.028) | Computer Communications · Journal | [Wi-Fi MAC](#wi-fi-mac-foundations) |
| 2020 | [Communication-Efficient Edge AI](https://doi.org/10.1109/COMST.2020.3007787) | IEEE COMST · Journal | [Surveys and foundations](#surveys-and-edge-intelligence-foundations) |
| 2020 | [Edgent](https://doi.org/10.1109/TWC.2019.2946140) | IEEE TWC · Journal | [Inference partitioning](#dnn-inference-offloading-and-partitioning) |
| 2020 | [Edge Computing × AI](https://doi.org/10.1109/JIOT.2020.2984887) | IEEE IoTJ · Journal | [Surveys and foundations](#surveys-and-edge-intelligence-foundations) |
| 2020 | [Wi-Fi 7 Challenges and Opportunities](https://doi.org/10.1109/COMST.2020.3012715) | IEEE COMST · Journal | [Wi-Fi MAC](#wi-fi-mac-foundations) |
| 2019 | [802.11ax Tutorial](https://doi.org/10.1109/COMST.2018.2871099) | IEEE COMST · Journal | [Wi-Fi MAC](#wi-fi-mac-foundations) |
| 2019 | [Edge Intelligence: Last Mile](https://doi.org/10.1109/JPROC.2019.2918951) | Proc. IEEE · Journal | [Surveys and foundations](#surveys-and-edge-intelligence-foundations) |
| 2017 | [MEC: Communication Perspective](https://doi.org/10.1109/COMST.2017.2745201) | IEEE COMST · Journal | [Surveys and foundations](#surveys-and-edge-intelligence-foundations) |
| 2017 | [MEC: Architecture and Offloading](https://doi.org/10.1109/COMST.2017.2682318) | IEEE COMST · Journal | [Surveys and foundations](#surveys-and-edge-intelligence-foundations) |
| 2021 | [Wi-Fi 7 Strikes Back](https://doi.org/10.1109/MCOM.001.2000711) | IEEE Communications Magazine · Magazine | [Standards writing](#standards-overview-and-tutorial-writing) |
| 2017 | [Distributed DNNs](https://doi.org/10.1109/ICDCS.2017.226) | IEEE ICDCS · Conference | [Foundational systems conferences](#conference-foundations) |
| 2017 | [Neurosurgeon](https://doi.org/10.1145/3037697.3037698) | ACM ASPLOS · Conference | [Foundational systems conferences](#conference-foundations) |
| 2016 | [MCDNN](https://doi.org/10.1145/2906388.2906396) | ACM MobiSys · Conference | [Foundational systems conferences](#conference-foundations) |

## Contents

- [Surveys and edge intelligence foundations](#surveys-and-edge-intelligence-foundations)
- [DNN inference offloading and partitioning](#dnn-inference-offloading-and-partitioning)
- [Resource aware admission placement and scheduling](#resource-aware-admission-placement-and-scheduling)
- [Wi Fi MAC foundations](#wi-fi-mac-foundations)
- [WLAN latency reliability and coexistence](#wlan-latency-reliability-and-coexistence)
- [Trustworthy edge intelligence](#trustworthy-edge-intelligence)
- [Standards overview and tutorial writing](#standards-overview-and-tutorial-writing)
- [Conference foundations](#conference-foundations)
- [Adjacent task oriented inference communication](#adjacent-task-oriented-inference-communication)

## Surveys and edge intelligence foundations

- **[2020 · IEEE Communications Surveys & Tutorials · Journal] [Communication-Efficient Edge AI: Algorithms and Systems](https://doi.org/10.1109/COMST.2020.3007787)** `Transferable`
  - Reviews algorithms and systems that reduce communication costs in training and inference. Useful for comparing inference-input and intermediate-feature transfers; distinguish the training material from AIO inference.
  - [DOI](https://doi.org/10.1109/COMST.2020.3007787) · [Metadata source](https://research.polyu.edu.hk/en/publications/communication-efficient-edge-ai-algorithms-and-systems/) · [Accessible manuscript](https://arxiv.org/abs/2002.09668) · 22(4):2167–2191
  - Scope: Applicable as MEC and edge-AI background, but not an IEEE 802.11bu normative specification or adopted procedure.
- **[2020 · IEEE Internet of Things Journal · Journal] [Edge Intelligence: The Confluence of Edge Computing and Artificial Intelligence](https://doi.org/10.1109/JIOT.2020.2984887)** `Transferable`
  - Separates AI for edge from AI on edge. Helps distinguish using AI to control WLANs from using WLANs to support AI inference.
  - [DOI](https://doi.org/10.1109/JIOT.2020.2984887) · [Metadata source](https://ieeexplore.ieee.org/document/9052677/) · [Accessible manuscript](https://dsg.tuwien.ac.at/~sd/papers/Zeitschriftenartikel_2020_SD_Edge_Intelligence.pdf) · 7(8):7457–7469
  - Scope: Applicable as MEC and edge-AI background, but not an IEEE 802.11bu normative specification or adopted procedure.
- **[2019 · Proceedings of the IEEE · Journal] [Edge Intelligence: Paving the Last Mile of Artificial Intelligence With Edge Computing](https://doi.org/10.1109/JPROC.2019.2918951)** `Transferable`
  - Reviews architectures and techniques for edge training and inference. An introduction to AI offload motivation and the device–edge–cloud distinction.
  - [DOI](https://doi.org/10.1109/JPROC.2019.2918951) · [Metadata source](https://ieeexplore.ieee.org/document/8736011/) · [Accessible manuscript](https://arxiv.org/abs/1905.10083) · 107(8):1738–1762
  - Scope: Applicable as MEC and edge-AI background, but not an IEEE 802.11bu normative specification or adopted procedure.
- **[2017 · IEEE Communications Surveys & Tutorials · Journal] [A Survey on Mobile Edge Computing: The Communication Perspective](https://doi.org/10.1109/COMST.2017.2745201)** `Transferable`
  - A starting point for jointly modeling wireless transmission and computation offloading. Useful for separating communication time, compute time, energy and resource allocation.
  - [DOI](https://doi.org/10.1109/COMST.2017.2745201) · [Metadata source](https://hub.hku.hk/handle/10722/259246) · [Accessible manuscript](https://arxiv.org/abs/1701.01090) · 19(4):2322–2358
  - Scope: Applicable as MEC and edge-AI background, but not an IEEE 802.11bu normative specification or adopted procedure.
- **[2017 · IEEE Communications Surveys & Tutorials · Journal] [Mobile Edge Computing: A Survey on Architecture and Computation Offloading](https://doi.org/10.1109/COMST.2017.2682318)** `Transferable`
  - Classifies offloading decisions, compute-resource allocation and mobility management. Useful for organizing AIO provider selection and session mobility while distinguishing them from their MEC background.
  - [DOI](https://doi.org/10.1109/COMST.2017.2682318) · [Metadata source](https://6gmobile.fel.cvut.cz/wp-publications/ieee-mec-survey/) · [Accessible manuscript](https://arxiv.org/abs/1702.05309) · 19(3):1628–1656
  - Scope: Applicable as MEC and edge-AI background, but not an IEEE 802.11bu normative specification or adopted procedure.

## DNN inference offloading and partitioning

- **[2026 · IEEE Transactions on Mobile Computing · Journal] [Task-Aware Collaborative Inference and Fine-Grained DNN Partitioning in MEC Networks](https://doi.org/10.1109/TMC.2025.3650680)** `Transferable`
  - Combines operator-level DAG partitioning with task-completion-based decision windows and joint resource allocation. A small Wi-Fi-connected edge testbed complements the MEC model; useful for studying when an offload scheduler should update its decisions.
  - [DOI](https://doi.org/10.1109/TMC.2025.3650680) · [Metadata source](https://api.crossref.org/works/10.1109/TMC.2025.3650680) · [Accessible manuscript](https://dsg.tuwien.ac.at/team/sd/papers/Journal_paper_2026_S_Dustdar_Task.pdf) · 25(6):8911–8927
  - Scope: Transferable MEC scheduling research with a small Wi-Fi-connected prototype. The analytical radio model and omitted control-message latency do not validate an 802.11 MAC procedure or 802.11bu feature.
- **[2024 · IEEE Transactions on Mobile Computing · Journal] [Distributed DNN Inference With Fine-Grained Model Partitioning in Mobile Edge Computing Networks](https://doi.org/10.1109/TMC.2024.3357874)** `Transferable`
  - Uses fine-grained DNN block partitioning to reduce inference latency on heterogeneous devices. Wi-Fi extensions should also account for additional transfers and control costs caused by partitioning.
  - [DOI](https://doi.org/10.1109/TMC.2024.3357874) · [Metadata source](https://api.crossref.org/works/10.1109/TMC.2024.3357874) · [Accessible manuscript](https://threadlocal.github.io/assets/files/TMC-Model_partition.pdf) · 23(10):9060-9074
  - Scope: An algorithmic MEC study, not a Wi-Fi standard feature or MAC implementation.
- **[2023 · IEEE Transactions on Mobile Computing · Journal] [Multi-Agent Collaborative Inference via DNN Decoupling: Intermediate Feature Compression and Edge Learning](https://doi.org/10.1109/TMC.2022.3183098)** `Transferable`
  - Jointly chooses partition points, channels and transmit power for multiple devices while compressing intermediate features. Useful for studying the coupling between AI-feature volume and competition for wireless resources.
  - [DOI](https://doi.org/10.1109/TMC.2022.3183098) · [Metadata source](https://api.crossref.org/works/10.1109/TMC.2022.3183098) · [Accessible manuscript](https://www.eng.auburn.edu/~szm0001/papers/TMC2023Hao.pdf) · 22(10):6041-6055
  - Scope: Assumes a powerful edge server and omits edge-inference latency. Do not cite it as solving compute queueing. Its wireless-interference model also differs from 802.11 CSMA/CA.
- **[2021 · IEEE/ACM Transactions on Networking · Journal] [CoEdge: Cooperative DNN Inference With Adaptive Workload Partitioning Over Heterogeneous Edge Devices](https://doi.org/10.1109/TNET.2020.3042320)** `Transferable`
  - Studies cooperative inference with heterogeneous edge-device performance and communication costs. Its ideas can inform joint airtime and compute allocation when distributing work among devices near an AP.
  - [DOI](https://doi.org/10.1109/TNET.2020.3042320) · [Metadata source](https://api.crossref.org/works/10.1109/TNET.2020.3042320) · [Accessible manuscript](https://par.nsf.gov/servlets/purl/10313790) · 29(2):595-608
  - Scope: Distinguish this paper from other papers named CoEdge. Its testbed results alone do not validate bu scheduling.
- **[2021 · IEEE Transactions on Mobile Computing · Journal] [JointDNN: An Efficient Training and Inference Engine for Intelligent Mobile Cloud Computing Services](https://doi.org/10.1109/TMC.2019.2947893)** `Transferable`
  - A basic model for choosing device–server partitions using layer-level compute and transfer costs. Wi-Fi offloading can extend it with measured airtime and server queueing.
  - [DOI](https://doi.org/10.1109/TMC.2019.2947893) · [Metadata source](https://api.crossref.org/works/10.1109/TMC.2019.2947893) · [Accessible manuscript](https://www.mpedram.com/Papers/research_projects_papers/Amirerfan/Joint/jointdnn.pdf) · 20(2):565-576
  - Scope: Mobile/cloud optimization. A Wi-Fi application needs to replace generalized link costs with realistic costs sensitive to contention.
- **[2020 · IEEE Transactions on Wireless Communications · Journal] [Edge AI: On-Demand Accelerating Deep Neural Network Inference via Edge Computing](https://doi.org/10.1109/TWC.2019.2946140)** `Transferable`
  - Jointly adapts DNN partition points and early exits to trade inference accuracy against latency. A starting point for offloading policies that respond to varying Wi-Fi rates.
  - [DOI](https://doi.org/10.1109/TWC.2019.2946140) · [Metadata source](https://api.crossref.org/works/10.1109/TWC.2019.2946140) · [Accessible manuscript](https://arxiv.org/abs/1910.05316) · 19(1):447-457
  - Scope: A bandwidth-adaptive inference design. It does not establish implementation of a standardized Wi-Fi MAC scheduler or bu feature.

## Resource aware admission placement and scheduling

- **[2026 · IEEE Transactions on Mobile Computing · Journal] [Robust DNN Partitioning and Resource Allocation Under Uncertain Inference Time](https://doi.org/10.1109/TMC.2025.3619509)** `Transferable`
  - Accounts for inference-time uncertainty and deadline-violation probability, extending approaches that optimize only average latency. Relevant to further work incorporating Wi-Fi delay variability.
  - [DOI](https://doi.org/10.1109/TMC.2025.3619509) · [Metadata source](https://api.crossref.org/works/10.1109/TMC.2025.3619509) · 25(3):3680-3696
  - Access scope: Final bibliographic metadata and the publisher abstract were checked. No open full text was obtained for this curation, so no claims about detailed experiments are included.
  - Scope: MEC optimization with probabilistic deadlines. WLAN contention and retransmissions require a separate model.
- **[2025 · IEEE Transactions on Networking · Journal] [Distributing Inference Tasks Over Interconnected Systems Through Dynamic DNNs](https://doi.org/10.1109/TON.2025.3543848)** `Transferable`
  - Connects inference placement with communication-resource allocation under joint partitioning, placement, bandwidth, compute and memory constraints. A broad modeling reference for Wi-Fi edge placement.
  - [DOI](https://doi.org/10.1109/TON.2025.3543848) · [Metadata source](https://api.crossref.org/works/10.1109/TON.2025.3543848) · [Abstract/digest](https://www.comsoc.org/system/files/2025-09/publications_contents_digest_2025_aug.pdf) · 33(4):1717-1730
  - Access scope: This introduction is based on the institutional abstract and ComSoc digest, not a review of the complete paper or its detailed experiments.
  - Scope: Publisher metadata uses IEEE Transactions on Networking, unlike the IEEE/ACM name retained in some author records. It is not bu adoption evidence.
- **[2024 · IEEE Transactions on Mobile Computing · Journal] [Optimizing Job Offloading Schedule for Collaborative DNN Inference](https://doi.org/10.1109/TMC.2023.3276937)** `Transferable`
  - Addresses pipeline ordering across multiple inference jobs, which partition-point optimization alone can miss. Relevant when designing Wi-Fi upload order together with edge-execution order.
  - [DOI](https://doi.org/10.1109/TMC.2023.3276937) · [Metadata source](https://api.crossref.org/works/10.1109/TMC.2023.3276937) · [Accessible manuscript](https://cis.temple.edu/~wu/research/publications/Publication_files/TMC_2022_04_0301_Final.pdf) · 23(4):3436-3451
  - Scope: Application and compute-pipeline scheduling. Airtime, retransmissions, contention and wireless queues require separate modeling.
- **[2023 · IEEE Transactions on Mobile Computing · Journal] [Throughput Maximization of Delay-Aware DNN Inference in Edge Computing by Exploring DNN Model Partitioning and Inference Parallelism](https://doi.org/10.1109/TMC.2021.3125949)** `Transferable`
  - Optimizes the number of inference requests meeting deadlines rather than packet throughput. Relevant to objective functions and admission control in joint Wi-Fi–edge scheduling.
  - [DOI](https://doi.org/10.1109/TMC.2021.3125949) · [Metadata source](https://api.crossref.org/works/10.1109/TMC.2021.3125949) · [Accessible manuscript](https://www.cs.cityu.edu.hk/~weliang/papers/LLLXJG23.pdf) · 22(5):3017-3030
  - Scope: Studies request admission and compute parallelism, distinct from packet-level Wi-Fi contention control. The final issue year is 2023.
- **[2022 · IEEE Journal on Selected Areas in Communications · Journal] [HiveMind: Towards Cellular Native Machine Learning Model Splitting](https://doi.org/10.1109/JSAC.2021.3118403)** `Transferable`
  - Considers multiple splits and control-message costs across devices, multiple edges and the cloud. Useful background for placement across multiple APs and edge nodes.
  - [DOI](https://doi.org/10.1109/JSAC.2021.3118403) · [Metadata source](https://api.crossref.org/works/10.1109/JSAC.2021.3118403) · [Accessible manuscript](https://sowang46.github.io/files/hivemind.pdf) · 40(2):626-640
  - Scope: A 5G cellular MEC study. Wi-Fi applications require changing the cellular-topology and link assumptions.

## Wi Fi MAC foundations

- **[2021 · Computer Communications · Journal] [Spatial Reuse in IEEE 802.11ax WLANs](https://doi.org/10.1016/j.comcom.2021.01.028)** `WLAN`
  - Clearly progresses from specification explanation to small-topology analysis and simulation. Its writing and validation approach can inform evaluation of AIO signaling costs and effects on existing traffic.
  - [DOI](https://doi.org/10.1016/j.comcom.2021.01.028) · [Metadata source](https://www.sciencedirect.com/science/article/pii/S0140366421000499) · [Accessible manuscript](https://arxiv.org/abs/1907.04141) · 170:65–83
  - Scope: Studies 11ax spatial reuse rather than AI offload itself; the analysis is based on Draft 4.0.
- **[2020 · IEEE Communications Surveys & Tutorials · Journal] [IEEE 802.11be Wi-Fi 7: New Challenges and Opportunities](https://doi.org/10.1109/COMST.2020.3012715)** `WLAN`
  - Broadly classifies candidate Wi-Fi 7 MAC and PHY technologies. Read for wireless-latency background and as an example of a standardization-trends paper.
  - [DOI](https://doi.org/10.1109/COMST.2020.3012715) · [Metadata source](https://ieeexplore.ieee.org/abstract/document/9152055) · [Accessible manuscript](https://arxiv.org/abs/2007.13401) · 22(4):2136–2166
  - Scope: A historical survey of TGbe candidate features. Do not describe every discussed candidate as a finally adopted feature.
- **[2019 · IEEE Communications Surveys & Tutorials · Journal] [A Tutorial on IEEE 802.11ax High Efficiency WLANs](https://doi.org/10.1109/COMST.2018.2871099)** `WLAN`
  - A foundation for OFDMA random access, spatial reuse and existing WLAN operation. Helps distinguish reused MAC features from new service signaling in a bu paper.
  - [DOI](https://doi.org/10.1109/COMST.2018.2871099) · [Metadata source](https://art.torvergata.it/handle/2108/240055) · [Accessible manuscript](https://www.ittc.ku.edu/~frost/EECS_563/A_Tutorial_on_IEEE_802.11ax_High_Efficiency_WLANs.pdf) · 21(1):197–216
  - Scope: A historical tutorial explaining Draft D3.0; it is not the current normative specification or a bu paper.

## WLAN latency reliability and coexistence

- **[2026 · IEEE Transactions on Machine Learning in Communications and Networking · Journal] [Deep Reinforcement Learning-Based Scheduling for Wi-Fi Multi-Access Point Coordination](https://doi.org/10.1109/TMLCN.2026.3682239)** `WLAN`
  - Compares PPO-based multi-AP spatial-reuse scheduling with MNP, OP and TAT heuristics using mean and 99th-percentile delay. Useful for designing tail-latency and background-traffic evaluations of inference-offload transport.
  - [DOI](https://doi.org/10.1109/TMLCN.2026.3682239) · [Metadata source](https://ieeexplore.ieee.org/document/11478468/) · [Accessible manuscript](https://arxiv.org/abs/2507.19377) · 4:744–757
  - Scope: AI for Wi-Fi scheduling, not an AI-inference offloading protocol or evidence of 802.11bu adoption. Simulation results depend on traffic and topology; some overloaded realizations are excluded, and low-load results do not uniformly favor the learned scheduler. The accessible manuscript is distinct from the verified journal publication.
- **[2024 · IEEE/ACM Transactions on Networking · Journal] [Wi-Fi Multi-Link Operation: An Experimental Study of Latency and Throughput](https://doi.org/10.1109/TNET.2023.3283154)** `WLAN`
  - Uses measured channel-occupancy traces to analyze MLO latency and throughput, including degradation with asymmetric links. An alternative to modeling offload-transfer delay as a constant.
  - [DOI](https://doi.org/10.1109/TNET.2023.3283154) · [Metadata source](https://ieeexplore.ieee.org/document/10149044/) · [Accessible manuscript](https://arxiv.org/abs/2305.02052) · 32(1):308–322
  - Scope: An evaluation using measured traces, not direct validation on commercial Wi-Fi 7 hardware. The final author record uses Carrascosa-Zamacois.
- **[2021 · Sensors · Journal] [Multi-Link Operation with Enhanced Synchronous Channel Access in IEEE 802.11be Wireless LANs: Coexistence Issue and Solutions](https://doi.org/10.3390/s21237974)** `WLAN`
  - Evaluates MLO gains alongside harm to legacy stations. A complementary example for studying coexistence costs of AIO signaling and explaining procedures and state transitions.
  - [DOI](https://doi.org/10.3390/s21237974) · [Metadata source](https://pmc.ncbi.nlm.nih.gov/articles/PMC8659962/) · [Accessible manuscript](https://pmc.ncbi.nlm.nih.gov/articles/PMC8659962/) · 21(23):7974
  - Scope: Included as a complementary coexistence-evaluation example, not because of a venue ranking. The paper does not establish final standard adoption of its proposed mechanism.

## Trustworthy edge intelligence

- **[2025 · IEEE Communications Surveys & Tutorials · Journal] [A Survey on Trustworthy Edge Intelligence: From Security and Reliability to Transparency and Sustainability](https://doi.org/10.1109/COMST.2024.3446585)** `Transferable`
  - Provides background for treating compute-endpoint security and trust separately from wireless-link protection. Relevant to AIO service authorization and trust assumptions.
  - [DOI](https://doi.org/10.1109/COMST.2024.3446585) · [Metadata source](https://ieeexplore.ieee.org/document/10640100/similar) · [Accessible manuscript](https://arxiv.org/abs/2310.17944) · 27(3):1729–1757
  - Scope: Applicable as MEC and edge-AI background, but not an IEEE 802.11bu normative specification or adopted procedure.

## Standards overview and tutorial writing

Do not interpret historical candidates or draft status as the current normative specification.

- **[2025 · Problems of Information Transmission · Journal] [A Tutorial on Wi-Fi 8: The Journey to Ultra High Reliability](https://doi.org/10.1134/S003294602502005X)** `WLAN`
  - Distinguishes feature-to-KPI relationships from inclusion in the draft. A model for literature reviews that separate AIO contributions, information-gathering polls and normative adoption.
  - [DOI](https://doi.org/10.1134/S003294602502005X) · [Metadata source](https://link.springer.com/article/10.1134/S003294602502005X) · [Accessible manuscript](https://link.springer.com/article/10.1134/S003294602502005X) · 61:164–210
  - Scope: Describes the state of the bn draft in 2025. Do not interpret KPI targets as universally measured performance gains.
- **[2021 · IEEE Communications Magazine · Magazine] [IEEE 802.11be: Wi-Fi 7 Strikes Back](https://doi.org/10.1109/MCOM.001.2000711)** `WLAN`
  - A magazine article combining a standards overview with a coordinated-beamforming latency example. Useful for judging the depth of procedural explanation and validation in an overview paper.
  - [DOI](https://doi.org/10.1109/MCOM.001.2000711) · [Metadata source](https://ieeexplore.ieee.org/document/9433521/) · [Accessible manuscript](https://arxiv.org/abs/2008.02815) · 59(4):102–108
  - Scope: A record of historical candidates and simulation. Do not use it as a current feature inventory or adoption evidence.

## Conference foundations

These conference papers provide systems foundations and are classified separately from journal articles.

- **[2017 · IEEE ICDCS · Conference] [Distributed Deep Neural Networks Over the Cloud, the Edge and End Devices](https://doi.org/10.1109/ICDCS.2017.226)** `Transferable`
  - Studies distributing DNNs across the device–edge–cloud hierarchy and reducing communication. Useful for experiments with multiple compute providers, without assuming model partitioning itself falls within bu scope.
  - [DOI](https://doi.org/10.1109/ICDCS.2017.226) · [Metadata source](https://dash.harvard.edu/bitstreams/d5edc79d-48a2-4884-88a7-a9636e55f444/download) · [Accessible manuscript](https://arxiv.org/abs/1709.01921) · 328–339
  - Scope: Prior work on distributed-inference systems. It does not establish that model partitioning and multi-device orchestration are within the current normative scope of bu.
- **[2017 · ACM ASPLOS · Conference] [Neurosurgeon: Collaborative Intelligence Between the Cloud and Mobile Edge](https://doi.org/10.1145/3037697.3037698)** `Transferable`
  - An early representative system using device–cloud DNN partitioning and layer-level cost profiles. A starting point for comparing actual layer and communication costs instead of a simple FLOPs/FLOPS ratio.
  - [DOI](https://doi.org/10.1145/3037697.3037698) · [Metadata source](https://www.cl.cam.ac.uk/~ey204/teaching/ACS/R244_2023_2024/papers/kang_asplos_2017.pdf) · [Accessible manuscript](https://www.cl.cam.ac.uk/~ey204/teaching/ACS/R244_2023_2024/papers/kang_asplos_2017.pdf)
  - Scope: An ASPLOS proceedings paper. Do not confuse its DOI with the SIGARCH issue DOI or classify it as a journal article. It does not define bu signaling.
- **[2016 · ACM MobiSys · Conference] [MCDNN: An Approximation-Based Execution Framework for Deep Stream Processing Under Resource Constraints](https://doi.org/10.1145/2906388.2906396)** `Transferable`
  - Jointly considers accuracy, memory, energy and remote-execution costs across multiple DNN streams. System background for why compute descriptors should convey more than a single peak-performance number.
  - [DOI](https://doi.org/10.1145/2906388.2906396) · [Metadata source](https://homes.cs.washington.edu/~arvind/papers/mcdnn.pdf) · [Accessible manuscript](https://homes.cs.washington.edu/~arvind/papers/mcdnn.pdf)
  - Scope: A mobile-DNN resource-management systems study. It does not define IEEE 802.11bu procedures or frames.

## Adjacent task oriented inference communication

An optional adjacent topic. Do not equate learned feature-communication designs with standardized Wi-Fi PHY/MAC mechanisms.

- **[2022 · IEEE Journal on Selected Areas in Communications · Journal] [Learning Task-Oriented Communication for Edge Inference: An Information Bottleneck Approach](https://doi.org/10.1109/JSAC.2021.3126087)** `Transferable`
  - Reduces AI traffic by transmitting features needed to preserve accuracy. Useful for studying the trade-off between Wi-Fi airtime savings and inference accuracy.
  - [DOI](https://doi.org/10.1109/JSAC.2021.3126087) · [Metadata source](https://api.crossref.org/works/10.1109/JSAC.2021.3126087) · [Accessible manuscript](https://ira.lib.polyu.edu.hk/bitstream/10397/107084/1/Shao_Learning_Task-Oriented_Communication.pdf) · 40(1):197-211
  - Scope: An optional adjacent topic. Learned source/channel coding is not directly applicable as a standardized Wi-Fi PHY/MAC mechanism.

## Metadata notes

- Edgent: IEEE TWC **2020**; distinguish the 2019 manuscript and DOI history
- JointDNN: IEEE TMC **2021**; distinguish online-first publication in 2019
- Wi-Fi MLO: IEEE/ACM TON **2024**; distinguish the 2023 manuscript and DOI history
- Proceedings of the IEEE is a journal despite its name, not conference proceedings
- Publisher metadata for the 2025 FIN paper uses IEEE Transactions on Networking; some author records retain the IEEE/ACM name

## Related curation structures

[Edge AI Papers](https://github.com/withhaotian/awesome-edge-AI-papers) · [Edge Machine Learning](https://github.com/Bisonai/awesome-edge-machine-learning) · [Real-time AI](https://github.com/bob-zhihe/awesome-real-time-AI)

These repositories informed the classification and navigation structure. Their descriptions and metadata were not copied.


