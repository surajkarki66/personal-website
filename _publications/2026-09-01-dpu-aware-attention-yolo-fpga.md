---
title: "No Attention, No Problem: DPU-Aware Attention Approximation in Modern YOLO on FPGA"
collection: publications
category: conferences
permalink: /publication/2026-09-01-dpu-aware-attention-yolo-fpga
excerpt: 'A DPU-aware architecture for attention-based YOLO variants (YOLOv26, YOLOv11) on AMD FPGAs, benchmarked across six datasets and all eight DPU configurations on the Xilinx ZCU104.'
date: 2026-09-01
venue: '29th Euromicro Conference on Digital System Design (DSD 2026), IEEE'
paperurl: 'https://doi.org/10.23919/dsdcps00089.2026.00025'
citation: '<b>Karki, S.</b>, Ahmed, Q. A., & Jungeblut, T. (2026). &quot;No Attention, No Problem: DPU-Aware Attention Approximation in Modern YOLO on FPGA.&quot; In <i>2026 29th Euromicro Conference on Digital System Design (DSD)</i>, pp. 106-113. IEEE.'
---

**Abstract.** Edge-based Artificial Intelligence (AI) acceleration has recently improved progress in real-time object detection. Object detection on edge devices requires a balance between accuracy, speed, and power efficiency. This paper proposes a customized Deep Learning Processor Unit (DPU)-aware architecture for attention-based YOLO variants deployed on AMD FPGAs. Specifically, we evaluate and benchmark YOLOv26 and YOLOv11, two modern attention-based YOLO variants, on the Xilinx ZCU104 across both standard and oriented object detection tasks. We replace unsupported activation functions, substitute split operations with 1x1 convolutions, and approximate the spatial attention mechanism in a DPU-compatible way. All models are then trained and evaluated across six benchmark datasets such as COCO, Pascal VOC, KITTI, DOTA, DIOR-R, and an in-house human presence dataset, and benchmarked across all eight DPU configurations (B512 to B4096) in terms of mAP, FPS, latency, power, and resource utilization. Notably, YOLOv26n and YOLOv26n-OBB deliver the highest end-to-end throughput at 34.05 and 29.55 FPS for standard and oriented detection, respectively, with an average of 5% absolute reduction in accuracy due to quantization while achieving up to approximately 3x lower power consumption compared with the state of the art.
