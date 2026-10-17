# Mohammed Abdullah | Silicon Architecture & AI Acceleration
[![Live Portfolio](https://img.shields.io/badge/Live_Portfolio-abdullaah0309.github.io-blue?style=for-the-badge&logo=googlechrome&logoColor=white)](https://abdullaah0309.github.io)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Mohammed_Abdullah-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/abdullah-ece-mvsr)
[![SystemVerilog](https://img.shields.io/badge/HDL-SystemVerilog%20%7C%20Verilog-orange?style=for-the-badge)](https://github.com/abdullaah0309)
[![Artix-7 Verified](https://img.shields.io/badge/FPGA-AMD%20Artix--7%20Timing%20Met-brightgreen?style=for-the-badge)](https://github.com/abdullaah0309)

---

## 🏛️ Silicon Portfolio Overview
Welcome to the production repository for my personal engineering portfolio. This site showcases end-to-end digital VLSI, custom ASIC design, and deep-learning hardware accelerator architectures.

- **Primary Track:** AI Hardware Accelerators, RTL Architecture, Low-Power Digital VLSI
- **Affiliation:** B.E. in Electronics & Communication Engineering, MVSR Engineering College (Class of 2028)
- **Target Roles:** Silicon Architecture, RTL Design, ASIC/FPGA Implementation

---

## ⚡ Flagship Architectures Featured

### 1. TITAN-SPARSE NPU (2:4 Structured Sparsity Engine)
- **Datapath:** Zero-overhead 2:4 metadata decompression decoder, 0-cycle combinational activation crossbar, dual-lane INT8 MAC multiplier tree, 32-bit accumulator with saturation, and single-cycle ReLU activation unit.
- **Memory Subsystem:** Double-buffered Ping-Pong SRAM scratchpad (twin 16-word banks) achieving 100% DMA latency hiding and 1-cycle pipeline-matched read latency.
- **Interconnect:** AMBA AXI4-Lite CSR slave control interface + 64-bit AXI4-Stream bulk DMA ingestion with full `TVALID`/`TREADY` backpressure handshaking.
- **Physical Silicon Verification (AMD Artix-7 `xc7a35tcsg324-1`):**
  - **Setup Timing Slack ($WNS$):** `+7.079 ns` @ 100 MHz ($f_{\max} \approx 342.3\text{ MHz}$)
  - **Total On-Chip Power:** `97 mW` (`26 mW` dynamic compute, `70 mW` static @ 25.5°C)
  - **Resource Footprint:** `202 Logic LUTs` (0.97%), `32 FFs` (0.08%), `37 CARRY4`

### 2. 32-Bit Workload-Adaptive AI ALU
- **Architecture:** Dynamic 16-bit operand isolation, 4-lane INT8 SIMD vector partitioning, and hardware ReLU.
- **Implementation:** Placed & routed on AMD Artix-7 (107 mW, 689 LUTs). Full-custom CMOS ASIC layout generated in KLayout with 108 pad-ring I/O bonds and dual VDD/VSS power rails.

### 3. 2D Systolic Array Accelerator
- **Architecture:** Weight-stationary 2D spatial mesh compute matrix with pipelined boundary skew registers for dense matrix multiplication (GEMM).

---

## 🌐 Visit the Interactive Web Platform
Launch the interactive web portal for architecture schematics, interactive timing reports, and power analysis:
👉 **[https://abdullaah0309.github.io](https://abdullaah0309.github.io)**

---
© 2026 Mohammed Abdullah. Designed for high-performance silicon engineering.
