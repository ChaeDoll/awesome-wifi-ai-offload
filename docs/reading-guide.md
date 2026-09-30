# Reading guide for Wi-Fi AI Offload

## What this collection does

This is a journal-first starting set for studying AI inference offloading over WLANs. It combines two intentionally distinct literatures:

- **Direct WLAN**: IEEE 802.11 MAC, link access, MLO, coexistence and transport latency
- **Transferable edge AI/MEC**: inference placement, partitioning, compute-resource management, profiling and service trust

A paper can be useful to an AIO design without proposing an IEEE 802.11bu mechanism. AIO SG contributions are listed separately from peer-reviewed papers. The selection does not claim an exhaustive review or a formal journal ranking.

## A practical initial reading path

1. **Mao et al., COMST 2017 — A Survey on Mobile Edge Computing: The Communication Perspective**
   Start with the communication/compute trade-off and avoid treating wireless transfer as a fixed negligible delay
2. **Zhou et al., Proceedings of the IEEE 2019 — Edge Intelligence: Paving the Last Mile...**
   Establish device-edge-cloud architecture and separate training from inference
3. **Neurosurgeon, ASPLOS 2017**
   See why layer-level execution and intermediate data size matter in a split-inference model
4. **MCDNN, MobiSys 2016**
   See resource/accuracy trade-offs and model-specific profiles instead of a single device capability number
5. **Carrascosa-Zamacois et al., IEEE/ACM TON 2024 — Wi-Fi Multi-Link Operation...**
   Add realistic channel occupancy and tail-latency behavior to the transfer model
6. **Karamyshev et al., Problems of Information Transmission 2025 — A Tutorial on Wi-Fi 8...**
   Learn to distinguish candidate features, draft contents and KPI goals in standards-facing writing

Use the focused inference journals in the bibliography after this path to choose a closer baseline for the actual problem: single-request partitioning, multi-request scheduling, server selection or end-edge collaboration.

## For the user's FLOPS/FLOPs discovery idea

The questions should be separated:

1. **Is the metadata exchange a plausible AIO research proposal?**
   Read the official PAR/CSD and capability/discovery contributions. Device processing capability has TOPS-based precedents; an explicit model-FLOPs descriptor should be labelled as the author's assumption/proposal unless adoption is evidenced
2. **Where does the model's operation count come from?**
   A provider-hosted model catalog and a requester-supplied new model have different information ownership. The requester can profile its workload offline, while discovery supplies provider capability/availability
3. **Is FLOPs / FLOPS a defensible latency model?**
   Use a workload-conditioned effective rate or an explicit simplified model. Peak capability is not current service availability. State precision, input shape, batch, sparse/dense convention, operation counting and whether model loading is included
4. **What is the WLAN contribution?**
   Make the discovery/query/setup semantics, management airtime, freshness and failure/admission behavior explicit. The upper-layer selection algorithm need not be mandated by the standard

[MCDNN's original paper](https://homes.cs.washington.edu/~arvind/papers/mcdnn.pdf) provides a useful historical example of model resource profiles. [NVIDIA GPU performance guidance](https://docs.nvidia.com/deeplearning/performance/dl-performance-gpu-background/index.html) explains why compute throughput alone misses memory-limited and underutilized execution. [TensorRT benchmarking](https://docs.nvidia.com/deeplearning/tensorrt/latest/performance/benchmarking.html) distinguishes execution, transfers, enqueue and warm-up costs. These vendor documents belong under measurement resources, not the peer-reviewed paper count.

## Minimal baseline/evaluation checklist

- Local-only, whole-offload and appropriate partitioned/selected-provider baselines
- Same model accuracy, input shapes, precision, compute capacity and radio resources
- Request-to-result completion, deadline-success rate and tails, including failures/timeouts
- Discovery/setup airtime, stale-resource rejections, model warm-up and provider queueing
- Legacy/background WLAN traffic impact
- Trace/testbed versus simulation labels; no generic percentage gain without the original conditions

## Bibliographic pitfalls already resolved

- Edgent's journal paper is **IEEE TWC 2020**, with a 2019 accepted manuscript and DOI registration; not JSAC 2019
- JointDNN's final issue is **IEEE TMC 2021**, with a 2019 DOI/online history
- Wi-Fi MLO's final issue is **IEEE/ACM TON 2024**, with a 2023 author manuscript and DOI registration
- Proceedings of the IEEE is a **journal**, despite its name
- Neurosurgeon's ASPLOS proceedings DOI is distinct from its SIGARCH issue DOI
- Older Wi-Fi standards papers may discuss candidates that were later altered or excluded
