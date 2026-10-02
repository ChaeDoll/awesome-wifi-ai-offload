# Awesome Wi-Fi AI Offload

**한국어** | [English](README.en.md)

Wi-Fi 기반 AI 추론 오프로딩을 위한 논문과 표준화 자료 모음. 학술지 논문을 먼저 정리하고, magazine 및 conference 논문과 IEEE 기고문은 구분한다.

**갱신일:** 2026-10-02 · **논문:** 핵심 29편 + 인접 주제 1편 · **표준 문서:** 별도 목록

이 목록은 공식 venue 순위나 완전한 문헌조사를 주장하지 않는다. Direct WLAN은 802.11 자체를 연구한 논문, Transferable은 MEC/edge AI에서 Wi-Fi 연구로 옮겨 쓸 수 있는 개념·모델이다. 어느 쪽도 곧바로 IEEE 802.11bu 채택 기술을 의미하지 않는다.

각 논문의 서지 확인일은 [papers.json](papers.json)의 `verified_on`에 기록한다. 표준 문헌의 확인 기준일은 별도 안내에 유지한다.

## Start here

- [읽기 순서와 FLOPS/FLOPs 연구 가이드](docs/reading-guide.md)
- [IEEE AIO 표준화 자료](docs/ieee-contributions.md)
- [구조화된 논문 데이터](papers.json)
- [기여 및 검증 기준](CONTRIBUTING.md)

## Legend

- `Journal` 동료심사 학술지 · `Magazine` 학술 magazine · `Conference` 학회 proceedings
- `WLAN` IEEE 802.11 직접 관련 · `Transferable` MEC/edge AI 응용 가능
- 연도는 검증된 최종 권호를 우선한다. arXiv는 공개 원문 링크일 수 있으며 그 자체로 최종 venue를 보증하지 않는다
- 링크는 출판사 및 저자 공개본을 가리킨다. PDF를 이 저장소에 복제하지 않는다

## Quick index

학술지 26편 → magazine 1편 → 학회 3편 순서이며 각 묶음은 최신 연도부터 정렬한다. 제목은 탐색용 축약명이며 정확한 제목은 아래 상세 목록에 있다.

| 연도 | 논문 (축약명) | Venue · 유형 | 주제 |
| --- | --- | --- | --- |
| 2026 | [DNN Partitioning Survey](https://doi.org/10.1145/3786145) | ACM CSUR · Journal | [Survey·기반](#surveys-and-edge-intelligence-foundations) |
| 2026 | [MAPC DRL Scheduling](https://doi.org/10.1109/TMLCN.2026.3682239) | IEEE TMLCN · Journal | [WLAN 지연·공존](#wlan-latency-reliability-and-coexistence) |
| 2026 | [Robust DNN Partitioning](https://doi.org/10.1109/TMC.2025.3619509) | IEEE TMC · Journal | [자원·스케줄링](#resource-aware-admission-placement-and-scheduling) |
| 2026 | [Task-Aware DNN Partitioning](https://doi.org/10.1109/TMC.2025.3650680) | IEEE TMC · Journal | [추론 분할](#dnn-inference-offloading-and-partitioning) |
| 2025 | [Trustworthy Edge Intelligence](https://doi.org/10.1109/COMST.2024.3446585) | IEEE COMST · Journal | [신뢰성·보안](#trustworthy-edge-intelligence) |
| 2025 | [Wi-Fi 8 Tutorial](https://doi.org/10.1134/S003294602502005X) | Problems of Information Transmission · Journal | [표준화 글쓰기](#standards-overview-and-tutorial-writing) |
| 2025 | [Dynamic DNN Inference (FIN)](https://doi.org/10.1109/TON.2025.3543848) | IEEE TON · Journal | [자원·스케줄링](#resource-aware-admission-placement-and-scheduling) |
| 2024 | [Fine-Grained DNN Partitioning](https://doi.org/10.1109/TMC.2024.3357874) | IEEE TMC · Journal | [추론 분할](#dnn-inference-offloading-and-partitioning) |
| 2024 | [Job Offloading Schedule](https://doi.org/10.1109/TMC.2023.3276937) | IEEE TMC · Journal | [자원·스케줄링](#resource-aware-admission-placement-and-scheduling) |
| 2024 | [Wi-Fi MLO Latency and Throughput](https://doi.org/10.1109/TNET.2023.3283154) | IEEE/ACM TON · Journal | [WLAN 지연·공존](#wlan-latency-reliability-and-coexistence) |
| 2023 | [Multi-Agent Collaborative Inference](https://doi.org/10.1109/TMC.2022.3183098) | IEEE TMC · Journal | [추론 분할](#dnn-inference-offloading-and-partitioning) |
| 2023 | [Delay-Aware Inference Throughput](https://doi.org/10.1109/TMC.2021.3125949) | IEEE TMC · Journal | [자원·스케줄링](#resource-aware-admission-placement-and-scheduling) |
| 2022 | [HiveMind](https://doi.org/10.1109/JSAC.2021.3118403) | IEEE JSAC · Journal | [자원·스케줄링](#resource-aware-admission-placement-and-scheduling) |
| 2022 | [Task-Oriented Edge Communication](https://doi.org/10.1109/JSAC.2021.3126087) | IEEE JSAC · Journal | [인접: 특징 전송](#adjacent-task-oriented-inference-communication) |
| 2021 | [CoEdge](https://doi.org/10.1109/TNET.2020.3042320) | IEEE/ACM TON · Journal | [추론 분할](#dnn-inference-offloading-and-partitioning) |
| 2021 | [JointDNN](https://doi.org/10.1109/TMC.2019.2947893) | IEEE TMC · Journal | [추론 분할](#dnn-inference-offloading-and-partitioning) |
| 2021 | [MLO Coexistence](https://doi.org/10.3390/s21237974) | Sensors · Journal | [WLAN 지연·공존](#wlan-latency-reliability-and-coexistence) |
| 2021 | [802.11ax Spatial Reuse](https://doi.org/10.1016/j.comcom.2021.01.028) | Computer Communications · Journal | [Wi-Fi MAC](#wi-fi-mac-foundations) |
| 2020 | [Communication-Efficient Edge AI](https://doi.org/10.1109/COMST.2020.3007787) | IEEE COMST · Journal | [서베이·기초](#surveys-and-edge-intelligence-foundations) |
| 2020 | [Edgent](https://doi.org/10.1109/TWC.2019.2946140) | IEEE TWC · Journal | [추론 분할](#dnn-inference-offloading-and-partitioning) |
| 2020 | [Edge Computing × AI](https://doi.org/10.1109/JIOT.2020.2984887) | IEEE IoTJ · Journal | [서베이·기초](#surveys-and-edge-intelligence-foundations) |
| 2020 | [Wi-Fi 7 Challenges and Opportunities](https://doi.org/10.1109/COMST.2020.3012715) | IEEE COMST · Journal | [Wi-Fi MAC](#wi-fi-mac-foundations) |
| 2019 | [802.11ax Tutorial](https://doi.org/10.1109/COMST.2018.2871099) | IEEE COMST · Journal | [Wi-Fi MAC](#wi-fi-mac-foundations) |
| 2019 | [Edge Intelligence: Last Mile](https://doi.org/10.1109/JPROC.2019.2918951) | Proc. IEEE · Journal | [서베이·기초](#surveys-and-edge-intelligence-foundations) |
| 2017 | [MEC: Communication Perspective](https://doi.org/10.1109/COMST.2017.2745201) | IEEE COMST · Journal | [서베이·기초](#surveys-and-edge-intelligence-foundations) |
| 2017 | [MEC: Architecture and Offloading](https://doi.org/10.1109/COMST.2017.2682318) | IEEE COMST · Journal | [서베이·기초](#surveys-and-edge-intelligence-foundations) |
| 2021 | [Wi-Fi 7 Strikes Back](https://doi.org/10.1109/MCOM.001.2000711) | IEEE Communications Magazine · Magazine | [표준화 글쓰기](#standards-overview-and-tutorial-writing) |
| 2017 | [Distributed DNNs](https://doi.org/10.1109/ICDCS.2017.226) | IEEE ICDCS · Conference | [기초 시스템 학회](#conference-foundations) |
| 2017 | [Neurosurgeon](https://doi.org/10.1145/3037697.3037698) | ACM ASPLOS · Conference | [기초 시스템 학회](#conference-foundations) |
| 2016 | [MCDNN](https://doi.org/10.1145/2906388.2906396) | ACM MobiSys · Conference | [기초 시스템 학회](#conference-foundations) |

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

- **[2026 · ACM Computing Surveys · Journal] [DNN Partitioning for Cooperative Inference in Edge Intelligence: Modeling, Solutions, Toolchains](https://doi.org/10.1145/3786145)** `Transferable`
  - 분할 개수와 세분도에 따른 협력 추론 설계를 비교하고 모델링·실험 도구를 정리한다. Wi-Fi 오프로딩의 분할 기준선과 연산·통신 비용 평가 항목을 고르는 데 유용하다.
  - [DOI](https://doi.org/10.1145/3786145) · [서지 근거](https://crossmark.crossref.org/dialog?cm_version=v2.0&doi=10.1145%2F3786145&domain=dl.acm.org) · [공개 원문](https://doi.org/10.1145/3786145) · 58(8):Article 204, 1–34
  - 범위: 일반 협력 추론 분할 연구의 survey이며 새로운 WLAN MAC 구현이나 IEEE 802.11bu 채택 근거는 아니다. 검토한 알고리즘과 평가 조건이 서로 달라 보편적인 성능 이득으로 해석하지 않는다.
- **[2020 · IEEE Communications Surveys & Tutorials · Journal] [Communication-Efficient Edge AI: Algorithms and Systems](https://doi.org/10.1109/COMST.2020.3007787)** `Transferable`
  - 학습과 추론에서 통신 비용을 줄이는 알고리즘 및 시스템을 정리한다. inference 입력과 중간 feature 전송을 비교할 때 유용하며 학습 관련 부분은 AIO 추론과 구분한다.
  - [DOI](https://doi.org/10.1109/COMST.2020.3007787) · [서지 근거](https://research.polyu.edu.hk/en/publications/communication-efficient-edge-ai-algorithms-and-systems/) · [공개 원문](https://arxiv.org/abs/2002.09668) · 22(4):2167–2191
  - 범위: MEC 및 edge AI 배경 연구로 응용할 수 있으나 IEEE 802.11bu 규범 사양이나 채택된 절차는 아니다.
- **[2020 · IEEE Internet of Things Journal · Journal] [Edge Intelligence: The Confluence of Edge Computing and Artificial Intelligence](https://doi.org/10.1109/JIOT.2020.2984887)** `Transferable`
  - AI for edge와 AI on edge를 분리하는 개념 틀. WLAN을 AI로 제어하는 연구와 WLAN으로 AI 추론을 지원하는 연구가 섞이지 않도록 한다.
  - [DOI](https://doi.org/10.1109/JIOT.2020.2984887) · [서지 근거](https://ieeexplore.ieee.org/document/9052677/) · [공개 원문](https://dsg.tuwien.ac.at/~sd/papers/Zeitschriftenartikel_2020_SD_Edge_Intelligence.pdf) · 7(8):7457–7469
  - 범위: MEC 및 edge AI 배경 연구로 응용할 수 있으나 IEEE 802.11bu 규범 사양이나 채택된 절차는 아니다.
- **[2019 · Proceedings of the IEEE · Journal] [Edge Intelligence: Paving the Last Mile of Artificial Intelligence With Edge Computing](https://doi.org/10.1109/JPROC.2019.2918951)** `Transferable`
  - edge에서 학습과 추론을 수행하는 구조와 기술을 정리한다. AI offload의 동기와 device-edge-cloud 구분을 설명하는 입문 자료다.
  - [DOI](https://doi.org/10.1109/JPROC.2019.2918951) · [서지 근거](https://ieeexplore.ieee.org/document/8736011/) · [공개 원문](https://arxiv.org/abs/1905.10083) · 107(8):1738–1762
  - 범위: MEC 및 edge AI 배경 연구로 응용할 수 있으나 IEEE 802.11bu 규범 사양이나 채택된 절차는 아니다.
- **[2017 · IEEE Communications Surveys & Tutorials · Journal] [A Survey on Mobile Edge Computing: The Communication Perspective](https://doi.org/10.1109/COMST.2017.2745201)** `Transferable`
  - 무선 전송과 계산 오프로딩을 함께 모델링하는 출발점. 통신 시간과 compute 시간, 에너지 및 자원 배분을 분리하는 데 유용하다.
  - [DOI](https://doi.org/10.1109/COMST.2017.2745201) · [서지 근거](https://hub.hku.hk/handle/10722/259246) · [공개 원문](https://arxiv.org/abs/1701.01090) · 19(4):2322–2358
  - 범위: MEC 및 edge AI 배경 연구로 응용할 수 있으나 IEEE 802.11bu 규범 사양이나 채택된 절차는 아니다.
- **[2017 · IEEE Communications Surveys & Tutorials · Journal] [Mobile Edge Computing: A Survey on Architecture and Computation Offloading](https://doi.org/10.1109/COMST.2017.2682318)** `Transferable`
  - 오프로딩 결정, compute 자원 배분과 이동성 관리를 분류한다. AIO provider 선택과 세션 이동을 MEC 배경과 구별하여 정리하기 좋다.
  - [DOI](https://doi.org/10.1109/COMST.2017.2682318) · [서지 근거](https://6gmobile.fel.cvut.cz/wp-publications/ieee-mec-survey/) · [공개 원문](https://arxiv.org/abs/1702.05309) · 19(3):1628–1656
  - 범위: MEC 및 edge AI 배경 연구로 응용할 수 있으나 IEEE 802.11bu 규범 사양이나 채택된 절차는 아니다.

## DNN inference offloading and partitioning

- **[2026 · IEEE Transactions on Mobile Computing · Journal] [Task-Aware Collaborative Inference and Fine-Grained DNN Partitioning in MEC Networks](https://doi.org/10.1109/TMC.2025.3650680)** `Transferable`
  - DAG의 연산자 단위 분할과 작업 완료에 맞춘 의사결정 구간, 자원 공동 할당을 결합한다. 소규모 Wi-Fi 연결 엣지 실험도 포함해 오프로딩 스케줄러의 결정 갱신 시점을 연구하는 데 유용하다.
  - [DOI](https://doi.org/10.1109/TMC.2025.3650680) · [서지 근거](https://api.crossref.org/works/10.1109/TMC.2025.3650680) · [공개 원문](https://dsg.tuwien.ac.at/team/sd/papers/Journal_paper_2026_S_Dustdar_Task.pdf) · 25(6):8911–8927
  - 범위: 소규모 Wi-Fi 연결 실험을 포함한 MEC 스케줄링 연구다. 분석적 무선 모델을 사용하고 제어 메시지 지연을 생략하므로 802.11 MAC 절차나 802.11bu 기능의 검증으로 보지 않는다.
- **[2024 · IEEE Transactions on Mobile Computing · Journal] [Distributed DNN Inference With Fine-Grained Model Partitioning in Mobile Edge Computing Networks](https://doi.org/10.1109/TMC.2024.3357874)** `Transferable`
  - 세밀한 DNN 블록 분할로 이기종 장치의 추론 지연을 줄인다. Wi-Fi 환경에서는 분할이 늘릴 수 있는 전송 횟수와 제어 비용까지 포함한 확장이 필요하다.
  - [DOI](https://doi.org/10.1109/TMC.2024.3357874) · [서지 근거](https://api.crossref.org/works/10.1109/TMC.2024.3357874) · [공개 원문](https://threadlocal.github.io/assets/files/TMC-Model_partition.pdf) · 23(10):9060-9074
  - 범위: 알고리즘 중심의 MEC 연구이며 Wi-Fi 표준 기능이나 MAC 구현은 아니다.
- **[2023 · IEEE Transactions on Mobile Computing · Journal] [Multi-Agent Collaborative Inference via DNN Decoupling: Intermediate Feature Compression and Edge Learning](https://doi.org/10.1109/TMC.2022.3183098)** `Transferable`
  - 여러 단말의 분할점·채널·전력을 함께 정하고 중간 특징을 압축한다. AI 특징 전송량과 무선 자원 경쟁의 결합을 공부하기 좋다.
  - [DOI](https://doi.org/10.1109/TMC.2022.3183098) · [서지 근거](https://api.crossref.org/works/10.1109/TMC.2022.3183098) · [공개 원문](https://www.eng.auburn.edu/~szm0001/papers/TMC2023Hao.pdf) · 22(10):6041-6055
  - 범위: 강력한 edge server를 가정하여 edge 추론 지연을 생략한다. compute queue를 해결한 연구로 인용하지 않는다. 무선 간섭 모델도 802.11 CSMA/CA와 다르다.
- **[2021 · IEEE/ACM Transactions on Networking · Journal] [CoEdge: Cooperative DNN Inference With Adaptive Workload Partitioning Over Heterogeneous Edge Devices](https://doi.org/10.1109/TNET.2020.3042320)** `Transferable`
  - 여러 엣지 장치의 이기종 성능과 통신 비용을 함께 보는 협력 추론 연구다. AP 주변 장치 간 작업 분산에서 airtime·연산 자원 공동 할당 문제로 옮겨갈 수 있다.
  - [DOI](https://doi.org/10.1109/TNET.2020.3042320) · [서지 근거](https://api.crossref.org/works/10.1109/TNET.2020.3042320) · [공개 원문](https://par.nsf.gov/servlets/purl/10313790) · 29(2):595-608
  - 범위: 같은 CoEdge 이름의 다른 논문과 구분한다. 이 논문의 testbed 결과만으로 bu scheduling이 검증되는 것은 아니다.
- **[2021 · IEEE Transactions on Mobile Computing · Journal] [JointDNN: An Efficient Training and Inference Engine for Intelligent Mobile Cloud Computing Services](https://doi.org/10.1109/TMC.2019.2947893)** `Transferable`
  - 계층별 연산·전송 비용으로 단말–서버 분할을 결정하는 기본 모델이다. Wi-Fi 오프로딩에서는 실측 airtime과 서버 대기시간을 넣어 확장할 수 있다.
  - [DOI](https://doi.org/10.1109/TMC.2019.2947893) · [서지 근거](https://api.crossref.org/works/10.1109/TMC.2019.2947893) · [공개 원문](https://www.mpedram.com/Papers/research_projects_papers/Amirerfan/Joint/jointdnn.pdf) · 20(2):565-576
  - 범위: 모바일 및 클라우드 최적화다. Wi-Fi 적용 시 일반화된 링크 비용을 contention에 민감한 실제 비용으로 바꿔야 한다.
- **[2020 · IEEE Transactions on Wireless Communications · Journal] [Edge AI: On-Demand Accelerating Deep Neural Network Inference via Edge Computing](https://doi.org/10.1109/TWC.2019.2946140)** `Transferable`
  - DNN 분할점과 early exit를 함께 조정해 추론 정확도·지연을 절충한다. Wi-Fi 전송률 변동에 대응하는 오프로딩 정책의 출발점으로 적합하다.
  - [DOI](https://doi.org/10.1109/TWC.2019.2946140) · [서지 근거](https://api.crossref.org/works/10.1109/TWC.2019.2946140) · [공개 원문](https://arxiv.org/abs/1910.05316) · 19(1):447-457
  - 범위: 대역폭 적응형 추론 설계다. 표준화된 Wi-Fi MAC scheduler나 bu 기능의 구현 근거는 아니다.

## Resource aware admission placement and scheduling

- **[2026 · IEEE Transactions on Mobile Computing · Journal] [Robust DNN Partitioning and Resource Allocation Under Uncertain Inference Time](https://doi.org/10.1109/TMC.2025.3619509)** `Transferable`
  - 추론 시간 불확실성과 deadline 위반 확률을 함께 다뤄 평균 지연만 최적화하는 접근을 보완한다. Wi-Fi의 지연 변동까지 결합하는 후속 연구에 적합하다.
  - [DOI](https://doi.org/10.1109/TMC.2025.3619509) · [서지 근거](https://api.crossref.org/works/10.1109/TMC.2025.3619509) · 25(3):3680-3696
  - 열람 범위: 최종 서지정보와 출판사 초록을 확인했다. 이 목록에서는 공개 전문을 확보하지 않아 상세 실험에 대한 주장은 포함하지 않는다.
  - 범위: 확률적 deadline을 고려한 MEC 최적화다. WLAN contention과 재전송은 별도 모델로 결합해야 한다.
- **[2025 · IEEE Transactions on Networking · Journal] [Distributing Inference Tasks Over Interconnected Systems Through Dynamic DNNs](https://doi.org/10.1109/TON.2025.3543848)** `Transferable`
  - 분할·배치·대역폭·연산·메모리를 함께 제한하는 문제로, 추론을 어디서 실행할지와 통신 자원 할당을 연결한다. Wi-Fi 엣지 배치 연구의 포괄적인 모델이다.
  - [DOI](https://doi.org/10.1109/TON.2025.3543848) · [서지 근거](https://api.crossref.org/works/10.1109/TON.2025.3543848) · [초록·digest](https://www.comsoc.org/system/files/2025-09/publications_contents_digest_2025_aug.pdf) · 33(4):1717-1730
  - 열람 범위: 기관 초록과 ComSoc digest에 근거한 소개이며 전체 논문 및 상세 실험을 검토한 요약은 아니다.
  - 범위: 출판사 메타데이터는 IEEE Transactions on Networking을 사용한다. 일부 저자 자료의 IEEE/ACM 명칭과 다르다. bu 채택 증거는 아니다.
- **[2024 · IEEE Transactions on Mobile Computing · Journal] [Optimizing Job Offloading Schedule for Collaborative DNN Inference](https://doi.org/10.1109/TMC.2023.3276937)** `Transferable`
  - 분할점만 최적화하면 놓치기 쉬운 다중 추론 작업의 파이프라인 순서를 다룬다. Wi-Fi 업로드 순서와 엣지 실행 순서를 함께 설계할 때 핵심 참고다.
  - [DOI](https://doi.org/10.1109/TMC.2023.3276937) · [서지 근거](https://api.crossref.org/works/10.1109/TMC.2023.3276937) · [공개 원문](https://cis.temple.edu/~wu/research/publications/Publication_files/TMC_2022_04_0301_Final.pdf) · 23(4):3436-3451
  - 범위: 애플리케이션 및 compute pipeline scheduling이다. airtime, 재전송, contention과 무선 queue는 별도 모델이 필요하다.
- **[2023 · IEEE Transactions on Mobile Computing · Journal] [Throughput Maximization of Delay-Aware DNN Inference in Edge Computing by Exploring DNN Model Partitioning and Inference Parallelism](https://doi.org/10.1109/TMC.2021.3125949)** `Transferable`
  - 패킷 처리량 대신 deadline을 만족한 추론 요청 수를 최적화한다. Wi-Fi–엣지 공동 스케줄러의 목적함수와 admission control 설계에 직접 참고할 만하다.
  - [DOI](https://doi.org/10.1109/TMC.2021.3125949) · [서지 근거](https://api.crossref.org/works/10.1109/TMC.2021.3125949) · [공개 원문](https://www.cs.cityu.edu.hk/~weliang/papers/LLLXJG23.pdf) · 22(5):3017-3030
  - 범위: 요청 admission과 compute 병렬성 연구다. 패킷 수준의 Wi-Fi contention 제어와 구별한다. 최종 권호는 2023년이다.
- **[2022 · IEEE Journal on Selected Areas in Communications · Journal] [HiveMind: Towards Cellular Native Machine Learning Model Splitting](https://doi.org/10.1109/JSAC.2021.3118403)** `Transferable`
  - 단말–다중 엣지–클라우드 사이의 다중 분할과 제어 메시지 비용을 함께 고려한다. 다중 AP/엣지 배치의 설계 참고로 유용하다.
  - [DOI](https://doi.org/10.1109/JSAC.2021.3118403) · [서지 근거](https://api.crossref.org/works/10.1109/JSAC.2021.3118403) · [공개 원문](https://sowang46.github.io/files/hivemind.pdf) · 40(2):626-640
  - 범위: 5G cellular MEC 연구다. Wi-Fi 적용에는 cellular 토폴로지와 링크 가정의 변경이 필요하다.

## Wi Fi MAC foundations

- **[2021 · Computer Communications · Journal] [Spatial Reuse in IEEE 802.11ax WLANs](https://doi.org/10.1016/j.comcom.2021.01.028)** `WLAN`
  - 규격 설명→작은 토폴로지 분석→시뮬레이션의 전개가 명확하다. AIO의 신호 비용과 기존 트래픽 영향을 평가하는 작성·검증 방식에 응용한다.
  - [DOI](https://doi.org/10.1016/j.comcom.2021.01.028) · [서지 근거](https://www.sciencedirect.com/science/article/pii/S0140366421000499) · [공개 원문](https://arxiv.org/abs/1907.04141) · 170:65–83
  - 범위: 11ax 공간 재사용 연구다. AI offload 자체를 다루지 않으며 분석 기준은 Draft 4.0이다.
- **[2020 · IEEE Communications Surveys & Tutorials · Journal] [IEEE 802.11be Wi-Fi 7: New Challenges and Opportunities](https://doi.org/10.1109/COMST.2020.3012715)** `WLAN`
  - Wi-Fi 7의 MAC 및 PHY 후보 기술을 폭넓게 분류한다. 무선 지연 제약의 배경과 표준화 동향 논문 구성 사례로 읽는다.
  - [DOI](https://doi.org/10.1109/COMST.2020.3012715) · [서지 근거](https://ieeexplore.ieee.org/abstract/document/9152055) · [공개 원문](https://arxiv.org/abs/2007.13401) · 22(4):2136–2166
  - 범위: TGbe의 역사적 후보 기능 조사다. 논의된 후보를 최종 채택 기능으로 바꾸어 쓰지 않는다.
- **[2019 · IEEE Communications Surveys & Tutorials · Journal] [A Tutorial on IEEE 802.11ax High Efficiency WLANs](https://doi.org/10.1109/COMST.2018.2871099)** `WLAN`
  - OFDMA random access, 공간 재사용과 기존 WLAN 동작을 이해하는 기반. bu 논문에서 재사용할 기존 MAC 기능과 새 서비스 신호 교환을 구분하는 데 유용하다.
  - [DOI](https://doi.org/10.1109/COMST.2018.2871099) · [서지 근거](https://art.torvergata.it/handle/2108/240055) · [공개 원문](https://www.ittc.ku.edu/~frost/EECS_563/A_Tutorial_on_IEEE_802.11ax_High_Efficiency_WLANs.pdf) · 21(1):197–216
  - 범위: Draft D3.0을 설명하는 당시의 tutorial이며 현재 규범 사양이나 bu 논문은 아니다.

## WLAN latency reliability and coexistence

- **[2026 · IEEE Transactions on Machine Learning in Communications and Networking · Journal] [Deep Reinforcement Learning-Based Scheduling for Wi-Fi Multi-Access Point Coordination](https://doi.org/10.1109/TMLCN.2026.3682239)** `WLAN`
  - PPO 기반 multi-AP spatial-reuse scheduling을 MNP·OP·TAT 휴리스틱과 비교하고 평균 및 99th-percentile 지연을 평가한다. 추론 오프로딩 전송 경로의 tail latency와 배경 트래픽 평가를 설계할 때 참고할 수 있다.
  - [DOI](https://doi.org/10.1109/TMLCN.2026.3682239) · [서지 근거](https://ieeexplore.ieee.org/document/11478468/) · [공개 원문](https://arxiv.org/abs/2507.19377) · 4:744–757
  - 범위: Wi-Fi를 제어하는 AI 연구이며 AI 추론 오프로딩 프로토콜이나 802.11bu 채택 근거는 아니다. 시뮬레이션 결과는 트래픽·토폴로지 조건에 의존하고 일부 과부하 사례를 제외하며 저부하에서 학습 기반 기법이 항상 우세하지는 않다. 공개 원고와 검증된 학술지 게재정보를 구분한다.
- **[2024 · IEEE/ACM Transactions on Networking · Journal] [Wi-Fi Multi-Link Operation: An Experimental Study of Latency and Throughput](https://doi.org/10.1109/TNET.2023.3283154)** `WLAN`
  - 실측 channel-occupancy trace로 MLO의 지연과 처리량을 분석하고 비대칭 링크에서의 악화도 설명한다. offload 전송 지연을 상수로 가정하는 모델의 대안이다.
  - [DOI](https://doi.org/10.1109/TNET.2023.3283154) · [서지 근거](https://ieeexplore.ieee.org/document/10149044/) · [공개 원문](https://arxiv.org/abs/2305.02052) · 32(1):308–322
  - 범위: 실측 trace를 활용한 평가이며 상용 Wi-Fi 7 하드웨어 직접 검증이라는 뜻은 아니다. 최종 저자 표기는 Carrascosa-Zamacois다.
- **[2021 · Sensors · Journal] [Multi-Link Operation with Enhanced Synchronous Channel Access in IEEE 802.11be Wireless LANs: Coexistence Issue and Solutions](https://doi.org/10.3390/s21237974)** `WLAN`
  - MLO 이득과 legacy 단말 피해를 함께 평가한다. AIO signal overhead의 공존성 평가와 절차·상태 전이 설명을 배우는 보완 자료다.
  - [DOI](https://doi.org/10.3390/s21237974) · [서지 근거](https://pmc.ncbi.nlm.nih.gov/articles/PMC8659962/) · [공개 원문](https://pmc.ncbi.nlm.nih.gov/articles/PMC8659962/) · 21(23):7974
  - 범위: venue 순위로 고른 논문이 아니라 공존성 평가의 보완 사례다. 저자 제안의 최종 표준 채택을 뜻하지 않는다.

## Trustworthy edge intelligence

- **[2025 · IEEE Communications Surveys & Tutorials · Journal] [A Survey on Trustworthy Edge Intelligence: From Security and Reliability to Transparency and Sustainability](https://doi.org/10.1109/COMST.2024.3446585)** `Transferable`
  - compute endpoint의 보안·신뢰성과 무선 링크 보호를 별도 문제로 보는 배경. AIO 서비스 인가 및 신뢰 가정을 설계할 때 참고한다.
  - [DOI](https://doi.org/10.1109/COMST.2024.3446585) · [서지 근거](https://ieeexplore.ieee.org/document/10640100/similar) · [공개 원문](https://arxiv.org/abs/2310.17944) · 27(3):1729–1757
  - 범위: MEC 및 edge AI 배경 연구로 응용할 수 있으나 IEEE 802.11bu 규범 사양이나 채택된 절차는 아니다.

## Standards overview and tutorial writing

역사적 후보·초안 상태를 현재 규범 사양으로 해석하지 않는다.

- **[2025 · Problems of Information Transmission · Journal] [A Tutorial on Wi-Fi 8: The Journey to Ultra High Reliability](https://doi.org/10.1134/S003294602502005X)** `WLAN`
  - 기능별 KPI 대응과 draft 포함 여부를 구분한다. AIO 기고문·정보 수집용 poll·규범적 채택을 구분하는 문헌 정리의 사례다.
  - [DOI](https://doi.org/10.1134/S003294602502005X) · [서지 근거](https://link.springer.com/article/10.1134/S003294602502005X) · [공개 원문](https://link.springer.com/article/10.1134/S003294602502005X) · 61:164–210
  - 범위: 2025년 bn 초안의 상태를 설명한다. KPI 목표를 보편적으로 측정된 성능 이득으로 해석하지 않는다.
- **[2021 · IEEE Communications Magazine · Magazine] [IEEE 802.11be: Wi-Fi 7 Strikes Back](https://doi.org/10.1109/MCOM.001.2000711)** `WLAN`
  - 표준화 개요와 CBF 지연 사례를 결합한 magazine 논문. 개요 논문에 어느 깊이의 절차와 검증 사례를 넣는지 참고하기 좋다.
  - [DOI](https://doi.org/10.1109/MCOM.001.2000711) · [서지 근거](https://ieeexplore.ieee.org/document/9433521/) · [공개 원문](https://arxiv.org/abs/2008.02815) · 59(4):102–108
  - 범위: 과거 후보와 simulation의 기록이다. 현재 기능 목록 또는 채택 근거로 사용하지 않는다.

## Conference foundations

아래는 기초 시스템을 이해하기 위한 학회 논문이며 학술지 논문과 별도 분류한다.

- **[2017 · IEEE ICDCS · Conference] [Distributed Deep Neural Networks Over the Cloud, the Edge and End Devices](https://doi.org/10.1109/ICDCS.2017.226)** `Transferable`
  - device-edge-cloud 계층에 DNN을 분산하는 구조와 통신 절감을 다룬다. 여러 compute provider를 쓰는 실험을 생각할 때 참고하되 모델 분할 자체를 bu 범위로 가정하지 않는다.
  - [DOI](https://doi.org/10.1109/ICDCS.2017.226) · [서지 근거](https://dash.harvard.edu/bitstreams/d5edc79d-48a2-4884-88a7-a9636e55f444/download) · [공개 원문](https://arxiv.org/abs/1709.01921) · 328–339
  - 범위: 분산 추론 시스템의 선행 연구다. 모델 분할과 다중 장치 orchestration이 현재 bu 규범 범위에 포함된다는 근거는 아니다.
- **[2017 · ACM ASPLOS · Conference] [Neurosurgeon: Collaborative Intelligence Between the Cloud and Mobile Edge](https://doi.org/10.1145/3037697.3037698)** `Transferable`
  - DNN의 device-cloud 분할과 layer별 비용 profile을 이용하는 초기 대표 시스템. 단순 FLOPs/FLOPS 비율 대신 실제 layer·통신 비용을 비교하는 출발점이다.
  - [DOI](https://doi.org/10.1145/3037697.3037698) · [서지 근거](https://www.cl.cam.ac.uk/~ey204/teaching/ACS/R244_2023_2024/papers/kang_asplos_2017.pdf) · [공개 원문](https://www.cl.cam.ac.uk/~ey204/teaching/ACS/R244_2023_2024/papers/kang_asplos_2017.pdf)
  - 범위: ASPLOS proceedings 논문이다. SIGARCH issue DOI와 혼동하거나 학술지 논문으로 분류하지 않는다. bu 신호 교환을 정의하지 않는다.
- **[2016 · ACM MobiSys · Conference] [MCDNN: An Approximation-Based Execution Framework for Deep Stream Processing Under Resource Constraints](https://doi.org/10.1145/2906388.2906396)** `Transferable`
  - 여러 DNN stream의 정확도·메모리·에너지·remote 실행 비용을 함께 다룬다. compute descriptor가 peak 성능 한 숫자보다 풍부해야 하는 이유를 보여 주는 시스템 배경이다.
  - [DOI](https://doi.org/10.1145/2906388.2906396) · [서지 근거](https://homes.cs.washington.edu/~arvind/papers/mcdnn.pdf) · [공개 원문](https://homes.cs.washington.edu/~arvind/papers/mcdnn.pdf)
  - 범위: 모바일 DNN 자원 관리 시스템 연구다. IEEE 802.11bu 절차 또는 프레임을 정의하지 않는다.

## Adjacent task oriented inference communication

선택적 인접 주제. 학습 기반 특징 전송 설계를 곧바로 표준 Wi-Fi PHY/MAC로 간주하지 않는다.

- **[2022 · IEEE Journal on Selected Areas in Communications · Journal] [Learning Task-Oriented Communication for Edge Inference: An Information Bottleneck Approach](https://doi.org/10.1109/JSAC.2021.3126087)** `Transferable`
  - 정확도 유지에 필요한 특징만 전송하는 관점에서 AI 트래픽의 크기를 줄인다. Wi-Fi airtime 절감과 추론 정확도 사이의 절충을 연구하는 데 유용하다.
  - [DOI](https://doi.org/10.1109/JSAC.2021.3126087) · [서지 근거](https://api.crossref.org/works/10.1109/JSAC.2021.3126087) · [공개 원문](https://ira.lib.polyu.edu.hk/bitstream/10397/107084/1/Shao_Learning_Task-Oriented_Communication.pdf) · 40(1):197-211
  - 범위: 선택적 인접 연구다. 학습된 source/channel coding을 표준 Wi-Fi PHY/MAC에 그대로 적용할 수 있다는 뜻은 아니다.

## Metadata notes

- Edgent: IEEE TWC **2020**; 2019 원고 및 DOI와 구별
- JointDNN: IEEE TMC **2021**; online-first 2019와 구별
- Wi-Fi MLO: IEEE/ACM TON **2024**; 2023 원고 및 DOI와 구별
- Proceedings of the IEEE는 이름과 달리 conference proceedings가 아닌 학술지
- 2025 FIN 논문의 publisher metadata는 IEEE Transactions on Networking으로 표기하며 일부 저자 기록의 IEEE/ACM 명칭과 구별

## Related curation structures

[Edge AI Papers](https://github.com/withhaotian/awesome-edge-AI-papers) · [Edge Machine Learning](https://github.com/Bisonai/awesome-edge-machine-learning) · [Real-time AI](https://github.com/bob-zhihe/awesome-real-time-AI)

위 저장소는 분류와 탐색 구조를 참고했으며 설명문과 메타데이터를 복사하지 않았다.



