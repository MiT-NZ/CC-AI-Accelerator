# 贡献指南 / Contributing Guidelines

感谢你对 **CC AI Accelerator** 开源项目的兴趣！🎉  
请阅读以下贡献指南，以确保贡献符合项目标准。

---

## **📌 如何贡献**
### ✅ 提交 Issue
如果你发现了 **Bug** 或者有新的 **功能建议**：
1. 进入 [GitHub Issues](https://github.com/MiT-NZ/CC-AI-Accelerator/issues)
2. 点击 **New Issue**
3. **填写 Bug 详细信息**，包括：
   - 复现步骤
   - 预期结果
   - 实际结果
   - 截图或日志（如果有）

### ✅ 提交 Pull Request (PR)
如果你想贡献代码：
1. Fork 仓库 并 Clone 到本地：
   ```bash
   git clone https://github.com/MiT-NZ/CC-AI-Accelerator.git
   ```

2. 创建新分支：
   ```bash
   git checkout -b feature-new-function
   ```

3. 提交代码：
   ```bash
   git add .
   git commit -m "Added new function XYZ"
   git push origin feature-new-function
   ```

4. 在 GitHub 提交 PR：
   - 进入 **Pull Requests**
   - 选择 **Create Pull Request**
   - **描述你的更改**
   - **等待 Maintainer 审核**

---

## **🛠️ 开发环境**
- **操作系统**：Windows / Linux / macOS
- **依赖项**：
  ```bash
  sudo apt install build-essential git
  ```
- **编译驱动**
  ```bash
  cd software/driver
  make
  sudo insmod ai_driver.ko
  ```

---

## **📜 代码风格**
- 使用 **PEP8**（Python） / **Linux Kernel Style**（C 语言）
- 变量命名采用 **snake_case**（Python） / **camelCase**（C）
- 提交信息格式：
  ```bash
  git commit -m "模块: 详细描述"
  ```
  示例：
  ```
  driver: 修复 AI 计算超时问题
  ```

---

## **💡 贡献者名单**
感谢所有贡献者！你可以在 [GitHub Contributors](https://github.com/MiT-NZ/CC-AI-Accelerator/graphs/contributors) 查看完整列表。

---

🚀 **欢迎你的贡献！如果有问题，请在 Issues 里提交反馈！**

