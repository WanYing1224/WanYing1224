<p align="center">
  <h1 align="center">Hi there, I'm Wan-Ying (Kevelyn) Lin 👋</h1>
  <p align="center">
    <strong>Computer Engineering Master's Student at USC</strong><br>
    Specializing in Digital VLSI Design | RTL & FPGA Acceleration | Hardware-Software Co-Design
  </p>
  <p align="center">
    <a href="https://linkedin.com/in/wan-ying-lin-27b6aa275"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
    <a href="mailto:kevelynlin1224@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
  </p>
</p>

---

## 🛠️ Technical Toolkit

### 📐 RTL Design & Verification
<img src="https://img.shields.io/badge/Verilog-F15A24?style=flat-square&logo=verilog&logoColor=white" alt="Verilog" /> <img src="https://img.shields.io/badge/RTL_Design-2C3E50?style=flat-square" alt="RTL Design" /> <img src="https://img.shields.io/badge/ModelSim-003366?style=flat-square&logo=mentor&logoColor=white" alt="ModelSim" /> <img src="https://img.shields.io/badge/Assembly_(AVR)-00599C?style=flat-square&logo=microchip&logoColor=white" alt="Assembly" />

### 🎛️ EDA Tools & Frameworks
<img src="https://img.shields.io/badge/Cadence_Virtuoso-003366?style=flat-square&logo=cadence&logoColor=white" alt="Cadence Virtuoso" /> <img src="https://img.shields.io/badge/Cadence_OrCAD-003366?style=flat-square&logo=cadence&logoColor=white" alt="Cadence OrCAD" /> <img src="https://img.shields.io/badge/Xilinx_ISE-741423?style=flat-square&logo=xilinx&logoColor=white" alt="Xilinx ISE" /> <img src="https://img.shields.io/badge/Altera_Quartus_II-002C6C?style=flat-square&logo=intel&logoColor=white" alt="Quartus II" />

### 🚀 Software, Systems & Parallel Computing
<img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white" alt="C++" /> <img src="https://img.shields.io/badge/Embedded_C-00599C?style=flat-square&logo=c&logoColor=white" alt="Embedded C" /> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" /> <img src="https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white" alt="CUDA" /> <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux" /> <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git" />

### 📡 Protocols & Interfaces
`TCP/IP` | `UDP` | `UART` | `Avalon Memory-Mapped Bus` | `AT Commands`

---

## 🚀 Featured Engineering Projects

### 🧠 BFloat16 Tensor Core SoC on NetFPGA (Earthquake Detection)
* **Architecture Design:** Developed a 4-thread inline ARM CPU pipeline and a custom BFloat16 Tensor Core accelerator directly inside a NetFPGA network datapath to bypass host-PC latency bounds.
* **Hardware Optimization & Timing Closure:** Resolved critical LUT resource overflows on a constrained Virtex-II Pro FPGA by replacing duplicated MAC units with hand-optimized Xilinx primitives (`MUXCY`, `XORCY`, `LUT2`), effectively closing timing.
* **Memory Subsystem:** Architected a Tri-BRAM Harvard memory layout (segregating features, weights, and biases) featuring a 3-zone address decoder to completely eliminate bus contention between the CPU and Tensor Core.
* **Verification:** Simulated the entire RTL pipeline using **ModelSim**, debugging a control FSM state-retention defect and demonstrating a ~98% classification accuracy against a reference GPU baseline.

### ⚡ Full-Custom CMOS 512-Bit SRAM Layout & Analysis
* **Transistor-Level Design:** Designed a complete 512-bit (32-word $\times$ 16-bit) SRAM architecture in **Cadence Virtuoso XL**, including the 6T bitcell matrix, 3-to-8 row decoders, sense amplifiers, write drivers, and pre-decoders.
* **Physical Layout:** Executed full-custom physical cell layouts for all 10 distinct sub-blocks, achieving 100% clean **Pegasus DRC/LVS verification** with zero final layout iterations.
* **Timing & SI Verification:** Conducted **Spectre** simulations to derive minimum pulse-width constraints for 5 critical control signals to prevent bitline contention, alongside **HSPICE** signal integrity analysis of FinFET technology across 0.8V–1.2V voltage scaling.

### 🧮 CUDA Accelerated Matrix Multiplication & Image Convolution
* **Parallel Performance:** Implemented and benchmarked parallel matrix multiplication approaches utilizing shared-memory tiling and **cuBLAS** on an NVIDIA RTX 3070 Ti, realizing a $3900\times$ compute speedup over the sequential CPU baseline.
* **Hardware Diagnosis:** Profiled shared-memory architectures to isolate L2 cache dependencies under specific compute constraints, and engineered a cross-boundary architecture using pinned memory (`cudaHostRegister`) for optimized Python data streaming via **ctypes**.
* **Filter Pipeline:** Scaled parallel kernels into an imaging pipeline (Gaussian, Sobel, Laplacian) utilizing constant memory for filter broadcasting, hitting a $1138\times$ performance increase.

### 📡 FMCW Radar Vital Signs Monitor (NSTC Funded Research Lead)
* **System Engineering:** Acted as Principal Investigator for an NSTC-funded project, developing a low-power, non-contact monitoring system utilizing an FMCW radar sensor paired with an **ESP32-C3** microcontroller.
* **Firmware & Signal Processing:** Authored bare-metal embedded C++ firmware to ingest high-frequency data streams, transmitting payloads over Wi-Fi to a custom Python processing pipeline optimized for real-time DSP data extraction.

---

## 📈 GitHub Insights

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=WanYing1224&show_icons=true&theme=radical" alt="Wan-Ying's GitHub Stats" width="48%" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=WanYing1224&layout=compact&theme=radical" alt="Wan-Ying's Top Languages" width="45%" />
</p>
