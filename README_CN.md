# wechatStep 🚶‍♂️✨

[English README](./README.md)

## 项目简介
wechatStep 是一个有趣的自动化工具，基于 GitHub Actions，每天自动提交微信步数。无需本地脚本或手动操作，设置好后让机器人帮你“走路”！🏃‍♀️🤖

## 工作原理
- ⏰ 利用 GitHub Actions 定时任务（每天北京时间 21:00）自动提交步数到微信运动。
- 🎲 步数范围可自定义，支持随机生成，让步数更自然。
- 🌐 通过调用第三方 API 实现步数提交。

## 账号及API信息
本项目使用开源的 [Steps-API](https://github.com/ymyuuu/Steps-API) 服务。关于账号注册、API 使用等详细信息，请前往该项目查看。

## 配置方法
1. 🍴 Fork 本仓库到你的 GitHub 账号。
2. 🔐 进入仓库 Settings > Secrets and variables > Actions，配置如下内容：
   - 在 Secrets 添加：
     - `STEP_ACCOUNTS`：多个账号，格式为 `邮箱1:密码1;邮箱2:密码2`（用冒号分隔账号和密码，用分号分隔多个账号）
   - 在 Variables 添加：
     - `API_URL`：步数提交 API 地址（如 `https://steps.api.030101.xyz/api`）
     - `STEP_MIN`：每日步数下限（如 8000）
     - `STEP_MAX`：每日步数上限（如 12000）
3. 🚀 workflow 会自动每天运行。如需手动触发，可在 Actions 页面选择 workflow 并点击“Run workflow”。

## 注意事项
- 📚 本项目仅供学习和交流使用，请勿用于非法用途。
- 🛡️ 请妥善保管账号信息，避免泄露。
- ⚠️ 微信可能会对异常步数或频繁提交行为进行风控，请适度使用，享受乐趣！

## License
MIT 📝
