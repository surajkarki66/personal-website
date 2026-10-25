---
title: "FPGA-Accelerated Network Intrusion Detection"
excerpt: "A small MLP trained on UNSW-NB15, quantized to INT8 and run on a custom FPGA neural-network accelerator for network intrusion detection."
collection: portfolio
permalink: /portfolio/fpga-accelerated-network-intrusion-detection/
header:
  teaser: portfolio/fpga-nids.png
---

![FPGA-Accelerated Network Intrusion Detection](/images/portfolio/fpga-nids.png)

This project trains a compact multilayer perceptron on the **UNSW-NB15** network-traffic dataset, quantizes it to **INT8 (Q1.7 fixed point)**, and runs the same network on a custom FPGA accelerator for binary attack detection.

**Pipeline**

* **Feature selection:** recursive feature elimination reduces the input to 10 features.
* **Training and evaluation:** float model trained in PyTorch (default topology 10 → 6 → 1; deeper networks configurable).
* **Deployment:** weights quantized to INT8 Q1.7 and exported as `.mem` ROM files and Verilog parameters.
* **Hardware:** a fully connected network accelerator in Verilog with shared MAC processing elements and an AXI4-Lite host interface, executing one layer at a time.
* **Verification:** golden vectors from the full UNSW-NB15 test set, Icarus Verilog testbenches, Verilator lint, and pytest unit tests, all run in GitHub Actions CI.

**Tech stack:** Python · PyTorch · Quantization (INT8) · Verilog · FPGA · AXI4-Lite · Icarus Verilog · Verilator

[Source code](https://github.com/surajkarki66/FPGA-Accelerated-Network-Intrusion-Detection)
