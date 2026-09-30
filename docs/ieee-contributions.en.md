# IEEE 802.11 AI Offload Official References

[한국어](ieee-contributions.md) | [English](ieee-contributions.en.md)

[English home](../README.en.md)

**Verification cutoff: 2026-09-30**

This list summarizes the PAR/CSD scope approved by the AIO SG and proposals in contributions. It does not indicate final IEEE-SA approval, normative adoption of fields or frames, or product compliance. As of 2026-09-30, AIO remains at the SG stage, with responses to LMSC comments and efforts toward final approval planned for November.

This is a reference list for tracking official documents, not an official IEEE interpretation or a guarantee of standards adoption. Contributor proposals, SG scope approval, and normative standards adoption are distinct.

- [AIO SG status](https://www.ieee802.org/11/Reports/aio_update.htm)
- [IEEE Mentor AIO document catalog](https://mentor.ieee.org/802.11/documents?is_group=0aio)

date is the upload date (ET) in the IEEE Mentor catalog. cover_date is the separately verified date on the document cover. Registration dates, cover dates, and upload dates may differ.

## How to interpret the current scope

- The direction is to support discovery, session lifecycle, and service authorization through MAC signaling/transport and the MAC service interface
- Compute providers include APs, non-AP STAs, and devices reached through the DS
- The CSD aims for independence from the PHY/lower MAC and support through software upgrades. It must not be read as indicating that 11bu already specifies particular channel-access changes or AI model semantics, partitioning, or compilation
- 802.11bn (UHR), 802.11bp (AMP), AIML SC, and WIN SG are separate activities

## PAR / CSD

### IEEE 802.11-26/1477r0 — Draft P802.11bu PAR

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1477-00-0aio-draft-p802-11bu-par.pdf)
- Authors: Robert Stacey | Affiliations: Intel
- Upload date (ET): 2026-07-17
- Topics: scope, PAR, timeline
- Status: draft_PAR_not_final_IEEE_SA_approval

 A starting point for checking the P802.11bu title, MAC scope, and MAC service interface. The document lists the PAR Status as Draft; the initial SA ballot in July 2029 and submission to RevCom in July 2030 are proposed milestones.

### IEEE 802.11-26/0978r7 — Initial PAR discussion

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-0978-07-0aio-initial-par-discussion.docx)
- Authors: Gaurang Naik, Xiaofei Wang, Jerome Henry, Zhanjing Bao, Mahmoud Hasabelnaby, Peng Liu | Affiliations: Qualcomm, InterDigital, Cisco, ZTE, Huawei
- Upload date (ET): 2026-07-15 | Cover date: 2026-07-15
- Topics: scope, PAR
- Status: SG_motion_passed_86_0_14_on_2026_07_15

 The version covered by the SG approval motion in July. It includes AI offload and discovery involving APs, non-AP STAs, and devices reached through the DS. SG approval must be distinguished from final IEEE-SA approval or adoption of specific fields.

### IEEE 802.11-26/0979r7 — Initial CSD discussion

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-0979-07-0aio-initial-csd-discussion.docx)
- Authors: Gaurang Naik, Jerome Henry | Affiliations: Qualcomm, Cisco
- Upload date (ET): 2026-07-15 | Cover date: 2026-07-15
- Topics: scope, CSD, software_upgrade
- Status: SG_motion_passed_71_12_17_on_2026_07_15

 Describes the direction for discovery, session setup/authorization, information exchange, and teardown. It aims for independence from the PHY/lower MAC and software upgrades for existing devices, and gives advertising model availability/characteristics as an example.

## Meeting minutes and status reports

### IEEE 802.11-26/1493r1 — AIO SG July 2026 Plenary Meeting Minutes

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1493-01-0aio-aio-sg-july-2026-plenary-meeting-minutes.docx)
- Authors: Zhanjing Bao, Xiaofei Wang | Affiliations: ZTE, InterDigital
- Upload date (ET): 2026-08-03 | Cover date: 2026-08-04
- Topics: minutes, adoption_evidence
- Status: approved_unanimously_on_2026_09_16

 Records discussions on July 13–15, PAR/CSD votes, and disagreements about layer boundaries. These minutes were approved in September and help distinguish presentation content from agreed outcomes.

### IEEE 802.11-26/1944r0 — AIO September 2026 Interim Meeting Minutes

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1944-00-0aio-aio-september-2026-interim-meeting-minutes.docx)
- Authors: Zhanjing Bao, Gaurang Naik | Affiliations: ZTE, Qualcomm
- Upload date (ET): 2026-09-30 | Cover date: 2026-09-26
- Topics: minutes, discovery, scope
- Status: initial_minutes_not_yet_approved_at_cutoff

 Covers discussions on September 16–17. It explicitly states that SG straw polls are for information gathering and records the session termination poll as 41/8/23. It identifies responding to LMSC comments and pursuing final approval in November as the next objectives.

### IEEE 802.11-26/1517r0 — aio-sg-september-2026-closing-report

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1517-00-0aio-aio-sg-september-2026-closing-report.pptx)
- Authors: Gaurang Naik | Affiliations: Qualcomm
- Upload date (ET): 2026-09-17 | Cover date: 2026-09-17
- Topics: status, timeline
- Status: SG_closing_report

 A brief status report confirming two September sessions and discussion of 10 technical contributions, and presenting plans for PAR/CSD review in November.

## Technical contributions

### IEEE 802.11-26/1599r0 — AI offload non-colocated compute

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1599-00-0aio-ai-offload-non-colocated-compute.pptx)
- Authors: Duncan Ho | Affiliations: Qualcomm
- Upload date (ET): 2026-09-15 | Cover date: 2026-09
- Topics: topology, session, mobility, higher_layer
- Status: discussed_in_SG_no_normative_adoption_verified

 Extends compute providers beyond the AP to other APs, STAs, and non-Wi-Fi devices. It discusses session identification and continuity during roaming, while leaving actual inference traffic after setup to higher layers. The cover title is AI/ML Inference Offload To Remote Devices.

### IEEE 802.11-26/1601r0 — AI Offload Framework for Topologies with Non-AP STA Compute Service Provider

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1601-00-0aio-ai-offload-framework-for-topologies-with-non-ap-sta-compute-service-provider.pptx)
- Authors: Chung-Ta Ku, Wilson Tsao, Paul Cheng | Affiliations: MediaTek
- Upload date (ET): 2026-09-11 | Cover date: 2026-09-11
- Topics: discovery, registration, TDLS, compute_capability
- Status: discussed_in_SG_no_normative_adoption_verified

 Presents registration, beacon discovery, association, session start/termination, and an optional TDLS path. The related September minutes discuss pre-association TOPS/memory separately from subsequent dynamic availability.

### IEEE 802.11-26/1605r1 — Thoughts on AIO - Requirements and TG Direction

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1605-01-0aio-thoughts-on-aio-requirements-and-tg-direction.pptx)
- Authors: Zhanjing Bao et al. | Affiliations: ZTE
- Upload date (ET): 2026-09-16 | Cover date: 2026-09-16
- Topics: taxonomy, discovery, scope, session
- Status: discussed_in_SG_no_normative_adoption_verified

 Distinguishes requester, responder, consumer, and compute provider, and proposes a structure that progresses from coarse discovery to detailed and protected stages. The allocation of TG work and the roles of other layers are contributor recommendations, not settled decisions.

### IEEE 802.11-26/1620r0 — Considerations on roaming issues for AI offload

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1620-00-0aio-considerations-on-roaming-issues-for-ai-offload.pptx)
- Authors: Tongxin Shu et al. | Affiliations: Sanechips
- Upload date (ET): 2026-09-16 | Cover date: 2026-09-16
- Topics: mobility, FT, SMD, session
- Status: discussed_in_SG_no_normative_adoption_verified

 Distinguishes connection continuity from AI service continuity. It proposes three cases—moving compute to the target BSS, retaining the existing provider, and using a DS appliance—and reuse of FT/SMD, while leaving compute-state migration to higher layers.

### IEEE 802.11-26/1425r0 — AIO Discovery and Session Setup for a Local Compute-capable Device

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1425-00-0aio-aio-discovery-and-session-setup-for-a-local-compute-capable-device.pptx)
- Authors: Ben Hwanwoong Hwang et al. | Affiliations: WILUS
- Upload date (ET): 2026-09-12 | Cover date: 2026-09-13
- Topics: discovery, provider_selection, session
- Status: discussed_in_SG_no_normative_adoption_verified

 Proposes registration, beacon/probe discovery, and AP-relayed setup based on a preferred responder list. The setup Ack, which indicates acceptance of processing, is distinct from the standard MAC ACK. The cover title is AIO Discovery and Session Setup for a Compute-capable non-AP STA.

### IEEE 802.11-26/1670r0 — Design Considerations for AI Offload

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1670-00-0aio-design-considerations-for-ai-offload.pptx)
- Authors: Juhyung Lee et al. | Affiliations: Nokia
- Upload date (ET): 2026-09-16 | Cover date: 2026-09-17
- Topics: compute_availability, discovery, admission, teardown
- Status: discussed_in_SG_no_normative_adoption_verified

 Emphasizes the difference between being AI-capable and currently AI-available. It proposes compact/coarse discovery, setup based on detailed resource profiles and QoS, AP-solicited offload, and early teardown. Results for the five poll questions in the slides were not found in the minutes reviewed.

### IEEE 802.11-26/1604r2 — Discussions on AIO Service Flow

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1604-02-0aio-discussions-on-aio-service-flow.pptx)
- Authors: Xu Chen et al. | Affiliations: Xiaomi
- Upload date (ET): 2026-09-17 | Cover date: 2026-09-17
- Topics: session, instance, teardown
- Status: discussed_information_only_termination_SP_41_8_23

 Distinguishes sessions from repeated/on-demand inference instances. It discusses result recipients and implicit/explicit termination. The 41/8/23 poll on termination support was for SG information gathering, not adoption of a normative procedure. The cover title uses the plural Flows.

### IEEE 802.11-26/1701r3 — AAA of AI Service in AI Offload

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1701-03-0aio-aaa-of-ai-service-in-ai-offload.pptx)
- Authors: Tao Chun Lee | Affiliations: MediaTek
- Upload date (ET): 2026-09-17 | Cover date: 2026-09-17
- Topics: security, authorization, admission
- Status: discussed_in_SG_no_normative_adoption_verified

 Here, AAA means Authentication, Authorization, and Admission (not Accounting). It distinguishes network authentication, service authorization, and resource-based admission, and proposes a two-stage structure spanning the MAC and higher layers.

### IEEE 802.11-26/1707r0 — Security and Privacy Considerations for AI Offload

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1707-00-0aio-security-and-privacy-considerations-for-ai-offload.pptx)
- Authors: Robin Thomas | Affiliations: Lenovo
- Upload date (ET): 2026-09-15 | Cover date: 2026-09-17
- Topics: security, privacy, lifecycle, trust
- Status: discussed_in_SG_no_normative_adoption_verified

 Examines threats and responsibilities across lifecycle stages, provider locations, and deployments. It distinguishes link protection from trust in compute endpoints and proposes a reuse/add/delegate framework. The omission of questions because of time constraints does not indicate consensus.

### IEEE 802.11-26/1667r2 — AIO Framework for AI Glasses

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1667-02-0aio-aio-framework-for-ai-glasses.pptx)
- Authors: Mahmoud Hasabelnaby et al. | Affiliations: Huawei
- Upload date (ET): 2026-09-17 | Cover date: 2026-09-16
- Topics: native_L2, model_discovery, compute_capability
- Status: discussed_in_SG_no_normative_adoption_verified

 A native L2 example using pre-deployed models. It proposes service advertisement followed by optional detailed model/compute queries and QoS/resource setup. Model and service identification schemes and storage-capacity issues remain open. The cover title is Layer-2 AI Offload Framework for AI Glass.

### IEEE 802.11-26/1042r1 — Thoughts on AI Offload

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1042-01-0aio-thoughts-on-ai-offload.pptx)
- Authors: Shravan Kumar Kalyankar | Affiliations: Huawei
- Upload date (ET): 2026-07-10 | Cover date: 2026-07-12
- Topics: compute_capability, TOPS, discovery, scope
- Status: discussed_in_SG_no_normative_adoption_verified

 Slide 4 presents TOPS-based device examples, and slide 5 presents discovery/registration of services, compute capabilities, and available resources. The reservation and compute-aware MAC operation in slides 7–9 also remain proposals.

### IEEE 802.11-26/0857r0 — Considerations on the scope of AI Offload

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-0857-00-0aio-considerations-on-the-scope-of-ai-offload.pptx)
- Authors: Robin Thomas | Affiliations: Lenovo
- Upload date (ET): 2026-05-09 | Cover date: 2026-05-13
- Topics: scope, MAC_hooks, model_interoperability
- Status: discussed_in_SG_no_normative_adoption_verified

 Proposes minimal MAC hooks, capabilities/IEs/frames, and extension points designed to accommodate change, distinguishing these from application semantics/orchestration at higher layers. The early projected schedule should be read in light of updates in subsequent minutes.

### IEEE 802.11-26/1391r0 — AI offload framework

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1391-00-0aio-ai-offload-framework.pptx)
- Authors: Duncan Ho et al. | Affiliations: Qualcomm
- Upload date (ET): 2026-07-14
- Topics: framework, session, model_reference
- Status: discussed_in_SG_no_normative_adoption_verified

 An example using model URLs/endpoints and AP compute admission. It discusses model caching and model use per session. Whether to use or combine with SCS was undecided at the time.

### IEEE 802.11-26/1379r0 — Thoughts on AIO directions

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1379-00-0aio-thoughts-on-aio-directions.pptx)
- Authors: Jerome Henry | Affiliations: Cisco
- Upload date (ET): 2026-07-08
- Topics: scope, existing_mechanism_reuse
- Status: discussed_in_SG_no_normative_adoption_verified

 Proposes reuse of existing WLAN functions and transparency of DS compute. The July minutes explicitly state that the conclusions presented should be read as candidate approaches rather than group consensus.

### IEEE 802.11-26/1340r1 — Thoughts on AI Offload from an Automotive Perspective

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1340-01-0aio-thoughts-on-ai-offload-from-an-automotive-perspective.pptx)
- Authors: Jing Ma | Affiliations: Toyota
- Upload date (ET): 2026-07-14
- Topics: mobility, automotive
- Status: discussed_in_SG_no_normative_adoption_verified

 Raises issues of compute/session continuity for vehicles and AGVs, and the availability of mobile providers. It is useful to read alongside the later roaming classification in 1620.

### IEEE 802.11-26/1282r0 — Thoughts on cooperative AI Offload solutions

- [Official source](https://mentor.ieee.org/802.11/dcn/26/11-26-1282-00-0aio-thoughts-on-cooperative-ai-offload-solutions.pptx)
- Authors: Tongxin Shu | Affiliations: Sanechips
- Upload date (ET): 2026-07-10
- Topics: cooperative_compute, scope
- Status: discussed_scenario_SP_51_25_28_not_normative

 Discusses cooperative compute across multiple APs/STAs. The related scenario poll was 51/25/28, and the boundary between task partitioning and the MAC role is a point of debate.

## Reading order for FLOPS / FLOPs and AIO discovery

1. **1042r1, slides 4–5**: A starting point for TOPS-based device examples and discovery of capabilities/available resources
2. **1601r0, slides 5–6 and the related discussion in 1944r0**: Beacon capability advertisement and the distinction between pre-association TOPS/memory and subsequent dynamic availability
3. **1670r0, slides 3–4**: The difference between nominal device capability and current availability; the distinction between coarse discovery and detailed setup
4. **1667r2, slide 5**: Detailed model/compute information and service descriptors through optional request/response exchanges
5. **1605r1, slide 4**: Distribution of information across pre-association, detailed, and protected stages, and layer boundaries

**Adoption caveat:** The documents reviewed do not establish normative adoption of specific discovery fields named FLOPS/FLOPs. Studying the exchange of processing-performance information or workload descriptors is different from claiming that these fields have already been standardized. This list also does not present a method for calculating model FLOPs or any particular selection algorithm as a standards requirement.

**Units caveat:** FLOPs is an operation count; FLOPS is a rate of floating-point operations per second. TOPS examples cannot be numerically equated with FLOPS at a particular floating-point precision. Peak capability, runtime availability, and model readiness must also be distinguished.

## Scope of source verification

The original PAR/CSD documents, July and September minutes, September closing report, 10 September technical contributions, and 1042r1, 857r0, and 1391r0 were reviewed. For 1379r0, 1340r1, and 1282r0, the official catalog and minutes were cross-checked; this does not mean that every slide was independently reviewed in full. At the cutoff date, 1944r0 was an initial set of minutes that had not yet been approved at the next meeting. Updates will be needed when new revisions or motion results become available.

