# 贡献指南 / Contributing Guidelines

感谢你对 **CC AI Accelerator** 开源项目的兴趣！🎉  
请阅读以下贡献指南，以确保贡献符合项目标准。

Thank you for your interest in the **CC AI Accelerator** open-source project! 🎉  
Please read the following contribution guidelines to ensure your contributions meet project standards.

---

## **📌 关于 / About**
**CC-AI-Accelerator** 是一款开源 AI 加速卡，支持 **M.2 NVMe 和 PCIe x4/x8**。

**CC-AI-Accelerator** is an open-source AI accelerator card that supports **M.2 NVMe and PCIe x4/x8**.

---

## **📌 如何贡献 / How to Contribute**
### ✅ 提交 Issue / Submitting Issues
如果你发现了 **Bug** 或者有新的 **功能建议**：
If you discover a **bug** or have a **feature suggestion**:
1. 进入 [GitHub Issues](https://github.com/MiT-NZ/CC-AI-Accelerator/issues)
   Go to [GitHub Issues](https://github.com/MiT-NZ/CC-AI-Accelerator/issues)
2. 点击 **New Issue**
   Click **New Issue**
3. **填写 Bug 详细信息**，包括：
   **Provide bug details**, including:
   - 复现步骤 / Steps to reproduce
   - 预期结果 / Expected result
   - 实际结果 / Actual result
   - 截图或日志（如果有）/ Screenshots or logs (if available)

### ✅ 提交 Pull Request (PR) / Submitting a Pull Request (PR)
如果你想贡献代码：
If you would like to contribute code:
1. Fork 仓库 并 Clone 到本地：
   Fork the repository and clone it locally:
   ```bash
   git clone https://github.com/MiT-NZ/CC-AI-Accelerator.git
   ```

2. 创建新分支：
   Create a new branch:
   ```bash
   git checkout -b feature-new-function
   ```

3. 提交代码：
   Commit your code:
   ```bash
   git add .
   git commit -m "Added new function XYZ"
   git push origin feature-new-function
   ```

4. 在 GitHub 提交 PR：
   Submit a PR on GitHub:
   - 进入 **Pull Requests**
     Go to **Pull Requests**
   - 选择 **Create Pull Request**
     Select **Create Pull Request**
   - **描述你的更改**
     **Describe your changes**
   - **等待 Maintainer 审核**
     **Wait for maintainer review**

---

## **🛠️ 开发环境 / Development Environment**
- **操作系统** / **Operating System**: Windows / Linux / macOS
- **依赖项** / **Dependencies**:
  ```bash
  sudo apt install build-essential git
  ```
- **编译驱动** / **Compile Driver**:
  ```bash
  cd software/driver
  make
  sudo insmod ai_driver.ko
  ```

---

## **📜 代码风格 / Code Style**
- 使用 **PEP8**（Python） / **Linux Kernel Style**（C 语言）
  Follow **PEP8** (Python) / **Linux Kernel Style** (C)
- 变量命名采用 **snake_case**（Python） / **camelCase**（C）
  Use **snake_case** (Python) / **camelCase** (C) for variable naming
- 提交信息格式 / Commit Message Format:
  ```bash
  git commit -m "模块: 详细描述"
  ```
  示例 / Example:
  ```
  driver: 修复 AI 计算超时问题
  driver: Fix AI computation timeout issue
  ```

---

## **💡 贡献者名单 / Contributors List**
感谢所有贡献者！
Thank you to all contributors! 
你可以在 [GitHub Contributors](https://github.com/MiT-NZ/CC-AI-Accelerator/graphs/contributors) 查看完整列表。
You can view the full list at [GitHub Contributors](https://github.com/MiT-NZ/CC-AI-Accelerator/graphs/contributors).

---

🚀 **欢迎你的贡献！如果有问题，请在 Issues 里提交反馈！**  
🚀 **We welcome your contributions! If you have any questions, please submit them via Issues!**

