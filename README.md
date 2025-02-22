# OpenAI-Accelerator / 开源AI加速器

## 项目简介 / Project Overview
**OpenAI-Accelerator** 是一款 **开源 AI 加速卡**，支持 **M.2 NVMe 2280 和 PCIe x4/x8** 接口。
目标是让 AI 计算像 NVMe 读写一样简单，并兼容 **TensorFlow, PyTorch, ONNX**。

**OpenAI-Accelerator** is an **open-source AI accelerator card** that supports **M.2 NVMe 2280 and PCIe x4/x8** interfaces.
The goal is to make AI computing as easy as NVMe storage access while being compatible with **TensorFlow, PyTorch, ONNX**.

## 主要特点 / Key Features
- **低成本 AI 加速**：使用 **Hailo-8 / Edge TPU / Kneron KL720** 提供高效 AI 推理。
- **M.2 + PCIe 双模式**：笔记本、台式机通用。
- **NVMe-over-PCIe AI 加速**：像 SSD 一样使用 AI 计算。
- **支持 PyTorch / TensorFlow / ONNX**，简化 AI 推理。

- **Low-cost AI acceleration**: Utilizes **Hailo-8 / Edge TPU / Kneron KL720** for efficient AI inference.
- **Dual-mode M.2 + PCIe**: Compatible with laptops and desktops.
- **NVMe-over-PCIe AI acceleration**: Operates like an SSD for AI computations.
- **Supports PyTorch / TensorFlow / ONNX**, simplifying AI inference.

## 目标应用 / Target Applications
- **本地 AI 加速**（Llama, ChatGLM, Whisper） / **Local AI acceleration** (Llama, ChatGLM, Whisper)
- **AI 绘图**（Stable Diffusion） / **AI Image Generation** (Stable Diffusion)
- **语音识别 / 翻译**（Whisper, DeepSpeech） / **Speech Recognition / Translation** (Whisper, DeepSpeech)
- **视频超分辨率**（Real-ESRGAN, Topaz Video AI） / **Video Super-Resolution** (Real-ESRGAN, Topaz Video AI)

## 硬件架构 / Hardware Architecture
| 组件 / Component | 选项 / Options | 说明 / Description |
|------|------|------|
| **AI 计算芯片 / AI Computing Chip** | Hailo-8 / Edge TPU / Kneron KL720 | 低功耗 AI 推理 / Low-power AI inference |
| **接口 / Interface** | M.2 NVMe 2280 + PCIe x4/x8 | 兼容台式机和笔记本 / Compatible with desktops and laptops |
| **存储 / Memory** | LPDDR4 2GB-8GB | AI 数据缓存 / AI data cache |
| **电源 / Power Supply** | 3.3V (M.2) / 12V (PCIe) | 适配不同供电 / Supports different power sources |
| **散热 / Cooling** | 铝制散热片 / 低功耗风扇 | 保持计算稳定 / Ensures stable computation |
| **桥接芯片 / Bridge Chip** | ASM2824（PCIe-NVMe 适配） | 统一接口 / Unified interface |

## 软件架构 / Software Architecture
| 层级 / Layer | 组件 / Component | 作用 / Function |
|------|------|------|
| **应用层 / Application Layer** | PyTorch / TensorFlow / ONNX | 运行 AI 模型 / Runs AI models |
| **中间件 / Middleware** | AI 计算 API（OpenVINO / TensorRT） | 统一 API / Unified API |
| **驱动层 / Driver Layer** | NVMe AI 调度系统 / NVMe AI Scheduler | 让 NVMe 设备处理 AI 计算 / Allows NVMe devices to process AI tasks |
| **硬件层 / Hardware Layer** | AI 计算卡（M.2 / PCIe） | 执行 AI 任务 / Executes AI tasks |

## 代码目录结构 / Code Directory Structure
```
OpenAI-Accelerator/
├── README.md  # 项目介绍 / Project Introduction
├── hardware/  # 硬件设计（PCB / BOM） / Hardware Design (PCB / BOM)
├── software/  # 驱动与 API 代码 / Drivers and API Code
├── docs/      # 开发文档 / Documentation
└── examples/  # AI 加速示例 / AI Acceleration Examples
```

## 开发指南 / Development Guide
### 1. 硬件测试 / Hardware Testing
- **使用 M.2 转 PCIe 适配器**，测试 NVMe AI 计算能力。
- **测试 AI 推理任务**，确保 Hailo-8 / TPU 正确执行任务。

- **Use an M.2 to PCIe adapter** to test NVMe AI computation capabilities.
- **Test AI inference tasks** to ensure correct execution of Hailo-8 / TPU.

### 2. 软件适配 / Software Adaptation
- **驱动开发**：NVMe-over-PCIe AI 计算引擎。
- **AI 框架适配**：确保 PyTorch / TensorFlow 能调用硬件。

- **Driver development**: NVMe-over-PCIe AI computing engine.
- **AI framework adaptation**: Ensure PyTorch / TensorFlow can utilize the hardware.

### 3. 社区与贡献 / Community & Contributions
欢迎贡献代码和硬件设计！ / Contributions to code and hardware design are welcome!
