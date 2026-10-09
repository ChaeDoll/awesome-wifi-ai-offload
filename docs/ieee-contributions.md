# IEEE 802.11 AI Offload 공식 문헌

[한국어](ieee-contributions.md) | [English](ieee-contributions.en.md)

**문서 검토 기준일: 2026-10-06 (한국시간); 개정 공지 확인일: 2026-10-09 (한국시간)**

AIO PAR/CSD 범위와 기고문 제안을 정리한 목록이다. [공식 WG 현황](https://www.ieee802.org/11/)은 PAR/CSD의 Working Group 승인을 확인하며, IEEE 802 검토·승인은 2026년 11월로 예상한다. 확인 기준일 현재 AIO는 여전히 Study Group으로 표시되어 있다. WG 승인은 IEEE-SA 최종 승인, 규범적 필드/프레임 채택 또는 제품 준수를 의미하지 않는다.

공식 문헌을 추적하는 참고 목록이며 IEEE의 공식 해석이나 표준 채택 보증이 아닙니다. 기고자의 제안, SG/WG 범위 승인, 규범적 표준 채택은 서로 다릅니다.

- [AIO SG 현황](https://www.ieee802.org/11/Reports/aio_update.htm)
- [IEEE Mentor AIO 문서 목록](https://mentor.ieee.org/802.11/documents?is_group=0aio)

date는 IEEE Mentor catalog의 업로드일(ET). cover_date는 별도 확인된 표지 날짜이다. 등록일·표지일·업로드일은 다를 수 있다.

## 현재 범위를 읽는 방법

- MAC signaling/transport 및 MAC service interface를 통해 discovery·session lifecycle·service authorization을 지원하는 방향입니다
- Compute provider는 AP, non-AP STA, DS 경유 장치를 포함합니다
- CSD는 PHY/lower-MAC 독립과 software upgrade를 지향합니다. 특정 채널접근 변경, AI 모델 의미·분할·컴파일을 이미 11bu가 규정한다고 해석하면 안 됩니다
- 802.11bn(UHR), 802.11bp(AMP), AIML SC 및 WIN SG는 별도 활동입니다

## PAR / CSD

### IEEE 802.11-26/1477r0 — Draft P802.11bu PAR

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1477-00-0aio-draft-p802-11bu-par.pdf)
- 저자: Robert Stacey | 소속: Intel
- 업로드일(ET): 2026-07-17
- 주제: scope, PAR, timeline
- 상태: draft_PAR_not_final_IEEE_SA_approval

 P802.11bu의 명칭·MAC 범위·MAC 서비스 인터페이스를 확인하는 시작점. 문서상 PAR Status는 Draft이며, 2029년 7월 initial SA ballot 및 2030년 7월 RevCom 제출은 제안 일정이다.

### IEEE 802.11-26/0978r7 — Initial PAR discussion

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-0978-07-0aio-initial-par-discussion.docx)
- 저자: Gaurang Naik, Xiaofei Wang, Jerome Henry, Zhanjing Bao, Mahmoud Hasabelnaby, Peng Liu | 소속: Qualcomm, InterDigital, Cisco, ZTE, Huawei
- 업로드일(ET): 2026-07-15 | 표지 날짜: 2026-07-15
- 주제: scope, PAR
- 상태: SG_motion_passed_86_0_14_on_2026_07_15

 7월 SG 승인 motion의 대상 버전. AP·non-AP STA·DS 경유 장치를 통한 AI offload 및 discovery를 포함한다. SG 승인은 IEEE-SA 최종 승인이나 구체적인 필드 채택과 구별해야 한다.

### IEEE 802.11-26/0979r7 — Initial CSD discussion

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-0979-07-0aio-initial-csd-discussion.docx)
- 저자: Gaurang Naik, Jerome Henry | 소속: Qualcomm, Cisco
- 업로드일(ET): 2026-07-15 | 표지 날짜: 2026-07-15
- 주제: scope, CSD, software_upgrade
- 상태: SG_motion_passed_71_12_17_on_2026_07_15

 Discovery, session setup/authorization, 정보 교환과 teardown의 방향을 설명한다. PHY/lower-MAC 독립과 기존 장치의 software upgrade를 지향하며 모델 availability/characteristics 광고를 예시로 든다.

## 회의록과 상태 보고

### IEEE 802.11-26/1493r1 — AIO SG July 2026 Plenary Meeting Minutes

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1493-01-0aio-aio-sg-july-2026-plenary-meeting-minutes.docx)
- 저자: Zhanjing Bao, Xiaofei Wang | 소속: ZTE, InterDigital
- 업로드일(ET): 2026-08-03 | 표지 날짜: 2026-08-04
- 주제: minutes, adoption_evidence
- 상태: approved_unanimously_on_2026_09_16

 7월 13–15일 논의, PAR/CSD 표결 및 계층 경계 관련 이견을 기록한다. 9월에 승인된 회의록이며 발표 내용과 합의 사항을 분리해 읽기에 유용하다.

### IEEE 802.11-26/1944r0 — AIO September 2026 Interim Meeting Minutes

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1944-00-0aio-aio-september-2026-interim-meeting-minutes.docx)
- 저자: Zhanjing Bao, Gaurang Naik | 소속: ZTE, Qualcomm
- 업로드일(ET): 2026-09-30 | 표지 날짜: 2026-09-26
- 주제: minutes, discovery, scope
- 상태: initial_minutes_not_yet_approved_at_cutoff

 9월 16–17일 논의. SG straw poll은 정보 수집 목적임을 명시하며 session termination poll은 41/8/23으로 기록한다. 11월 LMSC 의견 대응과 최종 승인 추진을 다음 목표로 제시한다.

2026-10-05 Tao Chun Lee가 [WG reflector](https://www.ieee802.org/11/email/stds-802-11/msg09645.html)에 보안 관련 검토 의견을 공개했다. 10월 8일 Zhanjing Bao는 이에 대한 회신에서 [R1 업데이트를 알렸다](https://www.ieee802.org/11/email/stds-802-11/msg09650.html). R1 원문과 catalog 메타데이터는 아직 독립적으로 검증하지 못했으므로 이 항목의 상세 요약과 날짜는 r0 기준이다. 이 공지는 회의록 승인이나 규범적 채택을 입증하지 않는다.

### IEEE 802.11-26/1517r0 — aio-sg-september-2026-closing-report

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1517-00-0aio-aio-sg-september-2026-closing-report.pptx)
- 저자: Gaurang Naik | 소속: Qualcomm
- 업로드일(ET): 2026-09-17 | 표지 날짜: 2026-09-17
- 주제: status, timeline
- 상태: SG_closing_report

 9월 두 세션·10개 기술 기고 논의를 확인하고, 11월 PAR/CSD 검토 계획을 제시하는 간단한 현황 자료.

## 기술 기고문

### IEEE 802.11-26/1599r0 — AI offload non-colocated compute

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1599-00-0aio-ai-offload-non-colocated-compute.pptx)
- 저자: Duncan Ho | 소속: Qualcomm
- 업로드일(ET): 2026-09-15 | 표지 날짜: 2026-09
- 주제: topology, session, mobility, higher_layer
- 상태: discussed_in_SG_no_normative_adoption_verified

 AP 외부의 AP·STA·비-Wi-Fi 장치까지 compute provider를 확장한다. 세션 식별·roaming 연속성을 논의하며 setup 이후 실제 inference traffic은 상위 계층으로 둔다. 표지 제목은 AI/ML Inference Offload To Remote Devices.

### IEEE 802.11-26/1601r0 — AI Offload Framework for Topologies with Non-AP STA Compute Service Provider

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1601-00-0aio-ai-offload-framework-for-topologies-with-non-ap-sta-compute-service-provider.pptx)
- 저자: Chung-Ta Ku, Wilson Tsao, Paul Cheng | 소속: MediaTek
- 업로드일(ET): 2026-09-11 | 표지 날짜: 2026-09-11
- 주제: discovery, registration, TDLS, compute_capability
- 상태: discussed_in_SG_no_normative_adoption_verified

 등록·beacon discovery·association·세션 시작/종료와 선택적 TDLS 경로를 제시한다. 관련 9월 회의록에서는 association 전 TOPS/memory와 이후 동적 가용량을 구분하여 논의한다.

### IEEE 802.11-26/1605r1 — Thoughts on AIO - Requirements and TG Direction

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1605-01-0aio-thoughts-on-aio-requirements-and-tg-direction.pptx)
- 저자: Zhanjing Bao et al. | 소속: ZTE
- 업로드일(ET): 2026-09-16 | 표지 날짜: 2026-09-16
- 주제: taxonomy, discovery, scope, session
- 상태: discussed_in_SG_no_normative_adoption_verified

 Requester·responder·consumer·compute provider를 구분하고 coarse discovery에서 상세·보호 단계로 발전하는 구조를 제안한다. TG 업무 배분과 타 계층 역할은 기고자의 권고이며 확정 사항이 아니다.

### IEEE 802.11-26/1620r0 — Considerations on roaming issues for AI offload

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1620-00-0aio-considerations-on-roaming-issues-for-ai-offload.pptx)
- 저자: Tongxin Shu et al. | 소속: Sanechips
- 업로드일(ET): 2026-09-16 | 표지 날짜: 2026-09-16
- 주제: mobility, FT, SMD, session
- 상태: discussed_in_SG_no_normative_adoption_verified

 연결 연속성과 AI 서비스 연속성을 구분한다. target BSS로 compute 이동·기존 provider 유지·DS appliance의 세 경우와 FT/SMD 재사용을 제안하며 compute-state migration은 상위 계층에 둔다.

### IEEE 802.11-26/1425r0 — AIO Discovery and Session Setup for a Local Compute-capable Device

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1425-00-0aio-aio-discovery-and-session-setup-for-a-local-compute-capable-device.pptx)
- 저자: Ben Hwanwoong Hwang et al. | 소속: WILUS
- 업로드일(ET): 2026-09-12 | 표지 날짜: 2026-09-13
- 주제: discovery, provider_selection, session
- 상태: discussed_in_SG_no_normative_adoption_verified

 등록·beacon/probe discovery와 preferred responder list 기반 AP 중계 setup을 제안한다. 처리 수락을 뜻하는 setup Ack는 표준 MAC ACK와 다르다. 표지 제목은 AIO Discovery and Session Setup for a Compute-capable non-AP STA.

### IEEE 802.11-26/1670r0 — Design Considerations for AI Offload

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1670-00-0aio-design-considerations-for-ai-offload.pptx)
- 저자: Juhyung Lee et al. | 소속: Nokia
- 업로드일(ET): 2026-09-16 | 표지 날짜: 2026-09-17
- 주제: compute_availability, discovery, admission, teardown
- 상태: discussed_in_SG_no_normative_adoption_verified

 AI-capable과 현재 AI-available의 차이를 강조한다. compact/coarse discovery, 상세 resource profile·QoS 기반 setup, AP-solicited offload와 early teardown을 제안한다. 슬라이드의 5개 poll 문항은 검토한 회의록에서 결과가 확인되지 않는다.

### IEEE 802.11-26/1604r2 — Discussions on AIO Service Flow

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1604-02-0aio-discussions-on-aio-service-flow.pptx)
- 저자: Xu Chen et al. | 소속: Xiaomi
- 업로드일(ET): 2026-09-17 | 표지 날짜: 2026-09-17
- 주제: session, instance, teardown
- 상태: discussed_information_only_termination_SP_41_8_23

 세션과 반복/요청형 inference instance를 구분한다. 결과 전달 대상과 implicit/explicit 종료를 논의한다. 종료 지원 poll 41/8/23은 SG 정보 수집이며 규범적 절차 채택이 아니다. 표지 제목은 복수형 Flows.

### IEEE 802.11-26/1701r3 — AAA of AI Service in AI Offload

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1701-03-0aio-aaa-of-ai-service-in-ai-offload.pptx)
- 저자: Tao Chun Lee | 소속: MediaTek
- 업로드일(ET): 2026-09-17 | 표지 날짜: 2026-09-17
- 주제: security, authorization, admission
- 상태: discussed_in_SG_no_normative_adoption_verified

 여기서 AAA는 Authentication·Authorization·Admission이다(Accounting 아님). 네트워크 인증·서비스 권한·자원 기반 admission을 구별하고 MAC/상위 계층의 두 단계 구조를 제안한다.

### IEEE 802.11-26/1707r0 — Security and Privacy Considerations for AI Offload

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1707-00-0aio-security-and-privacy-considerations-for-ai-offload.pptx)
- 저자: Robin Thomas | 소속: Lenovo
- 업로드일(ET): 2026-09-15 | 표지 날짜: 2026-09-17
- 주제: security, privacy, lifecycle, trust
- 상태: discussed_in_SG_no_normative_adoption_verified

 Lifecycle·provider 위치·deployment별 위협과 책임을 검토한다. 링크 보호와 compute endpoint 신뢰를 구분하고 reuse/add/delegate 틀을 제안한다. 시간 부족으로 질의가 생략된 것이 합의를 뜻하지 않는다.

### IEEE 802.11-26/1667r2 — AIO Framework for AI Glasses

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1667-02-0aio-aio-framework-for-ai-glasses.pptx)
- 저자: Mahmoud Hasabelnaby et al. | 소속: Huawei
- 업로드일(ET): 2026-09-17 | 표지 날짜: 2026-09-16
- 주제: native_L2, model_discovery, compute_capability
- 상태: discussed_in_SG_no_normative_adoption_verified

 Pre-deployed model을 활용하는 native L2 예시. 서비스 광고 후 선택적 상세 model/compute query와 QoS/resource setup을 제안한다. 모델·서비스 식별체계와 저장 용량 문제는 열려 있다. 표지 제목은 Layer-2 AI Offload Framework for AI Glass.

### IEEE 802.11-26/1042r1 — Thoughts on AI Offload

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1042-01-0aio-thoughts-on-ai-offload.pptx)
- 저자: Shravan Kumar Kalyankar | 소속: Huawei
- 업로드일(ET): 2026-07-10 | 표지 날짜: 2026-07-12
- 주제: compute_capability, TOPS, discovery, scope
- 상태: discussed_in_SG_no_normative_adoption_verified

 Slide 4에 TOPS 기반 장치 예, slide 5에 서비스·compute capability·가용 자원 discovery/registration을 제시한다. Slides 7–9의 예약·compute-aware MAC 운영도 제안 단계다.

### IEEE 802.11-26/0857r0 — Considerations on the scope of AI Offload

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-0857-00-0aio-considerations-on-the-scope-of-ai-offload.pptx)
- 저자: Robin Thomas | 소속: Lenovo
- 업로드일(ET): 2026-05-09 | 표지 날짜: 2026-05-13
- 주제: scope, MAC_hooks, model_interoperability
- 상태: discussed_in_SG_no_normative_adoption_verified

 변화에 강한 최소 MAC hook·capability/IE/frame과 확장점을 제안하고 application semantics/orchestration을 상위 계층과 구별한다. 초기 전망 일정은 이후 회의록으로 갱신해서 읽어야 한다.

### IEEE 802.11-26/1391r0 — AI offload framework

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1391-00-0aio-ai-offload-framework.pptx)
- 저자: Duncan Ho et al. | 소속: Qualcomm
- 업로드일(ET): 2026-07-14
- 주제: framework, session, model_reference
- 상태: discussed_in_SG_no_normative_adoption_verified

 모델 URL·endpoint와 AP compute admission을 활용하는 예시. 모델 caching 및 세션별 모델 사용을 논의한다. SCS 사용/결합 여부는 당시 미정이었다.

### IEEE 802.11-26/1379r0 — Thoughts on AIO directions

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1379-00-0aio-thoughts-on-aio-directions.pptx)
- 저자: Jerome Henry | 소속: Cisco
- 업로드일(ET): 2026-07-08
- 주제: scope, existing_mechanism_reuse
- 상태: discussed_in_SG_no_normative_adoption_verified

 기존 WLAN 기능의 재사용과 DS compute의 투명성을 제안한다. 7월 회의록은 제시된 결론을 그룹 합의가 아닌 후보 방안으로 읽어야 한다고 명시한다.

### IEEE 802.11-26/1340r1 — Thoughts on AI Offload from an Automotive Perspective

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1340-01-0aio-thoughts-on-ai-offload-from-an-automotive-perspective.pptx)
- 저자: Jing Ma | 소속: Toyota
- 업로드일(ET): 2026-07-14
- 주제: mobility, automotive
- 상태: discussed_in_SG_no_normative_adoption_verified

 차량·AGV의 compute/session 연속성과 이동 provider의 가용성 문제를 제기한다. 이후 1620의 roaming 분류와 함께 읽기 좋다.

### IEEE 802.11-26/1282r0 — Thoughts on cooperative AI Offload solutions

- [공식 원문](https://mentor.ieee.org/802.11/dcn/26/11-26-1282-00-0aio-thoughts-on-cooperative-ai-offload-solutions.pptx)
- 저자: Tongxin Shu | 소속: Sanechips
- 업로드일(ET): 2026-07-10
- 주제: cooperative_compute, scope
- 상태: discussed_scenario_SP_51_25_28_not_normative

 다수 AP/STA의 협력 compute를 논의한다. 관련 시나리오 poll은 51/25/28이었고 task partitioning과 MAC 역할의 경계가 논쟁점이다.

## FLOPS / FLOPs와 AIO discovery 읽기 순서

1. **1042r1, slides 4–5**: TOPS 기반 장치 예시와 capability/가용 자원 discovery의 출발점
2. **1601r0, slides 5–6 및 1944r0의 관련 토론**: beacon capability 광고, association 전 TOPS/memory와 이후 동적 가용량의 구분
3. **1670r0, slides 3–4**: 장치의 명목 능력과 현재 가용성의 차이; coarse discovery와 상세 setup 구분
4. **1667r2, slide 5**: 선택적 request/response를 통한 모델·compute 상세 정보와 service descriptor
5. **1605r1, slide 4**: pre-association·상세·보호 단계별 정보 분배 및 계층 경계

**채택 여부 주의:** 확인한 문헌은 FLOPS/FLOPs라는 구체적 discovery 필드의 규범적 채택을 입증하지 않습니다. 처리성능·workload descriptor 교환을 연구하는 것과 해당 필드가 이미 표준화되었다고 주장하는 것은 다릅니다. 모델 FLOPs의 계산 방식이나 특정 선택 알고리즘도 이 목록에서 표준 요구사항으로 제시하지 않습니다.

**단위 주의:** FLOPs는 연산량, FLOPS는 초당 부동소수점 연산 처리율입니다. TOPS 예시는 특정 floating-point precision의 FLOPS와 수치적으로 동일시할 수 없습니다. Peak capability, runtime availability, model readiness도 구별해서 읽어야 합니다.

## 자료 검증 범위

PAR/CSD, 7·9월 회의록, 9월 closing report, 10개 9월 기술 기고문, 1042r1·857r0·1391r0 원문을 확인했습니다. 1379r0·1340r1·1282r0은 공식 catalog와 회의록을 교차 확인했으며 각 슬라이드 전체를 독립 검토했다는 의미는 아닙니다. 9월 회의록의 상세 검토는 1944r0 기준입니다. 10월 8일 공식 R1 개정 공지는 10월 9일(한국시간)에 확인했으며, R1 원문 대조와 catalog 메타데이터 검증은 아직 완료하지 못했습니다. 해당 공지만으로 회의록 승인이나 규범적 채택을 확인할 수는 없습니다.

