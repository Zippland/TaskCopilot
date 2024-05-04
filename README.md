# LifeSync-AI

- [English README](README_EN.md)
- [中文 README](README.md)

## 概览
**LifeSync-AI** 超越了传统的任务管理功能，提供了一个动态的、由AI驱动的个人助理，旨在提高生活管理和决策能力。通过集成包括跨平台任务协同、AI智能建议、账单流水跟踪及实时环境数据反馈等一系列工具，LifeSync-AI帮助用户以前所未有的效率和洞察力来应对日常任务。

## 主要功能
- [X] **GHA自动化支持**：部署在github action中，以全自动运行程序。
- [X] **任务集成**：自动获取并管理Notion数据库中的task。
- [X] **智能建议生成**：利用OpenAI GPT生成优先级任务列表和战略性建议。
- [X] **天气信息**：获取实时天气更新和根据您的日程定制的建议。
- [X] **每日定时邮件通知**：每天清晨发送日常总结和任务提醒到您的邮箱，确保您始终准备就绪。
- [X] **灵活的任务调度**：根据实时数据和个性化建议智能调整您的任务管理。
- [ ] **环境变量管理**：自动获取并管理Notion数据库中的环境变量。
- [ ] **路线建议**：根据用户的出行目的和环境因素，提供每日出行的路线建议。
- [ ] **账单监控与总结**：监控用户的账单流水，并动态地总结和绘制表单。
- [ ] **日历和任务自动化管理**：通过主流的日历和task管理工具自动增删改查日历日程和日常任务。

## 入门指南

### 先决条件
- Python 3.8+
- 具有API访问权限的Notion账户
- Mailgun API密钥
- OpenAI API密钥
- OpenWeather API密钥

### 安装
克隆仓库并安装所需的依赖项：
```bash
git clone https://github.com/Zippland/LifeSync-AI.git
cd LifeSync-AI
pip install -r requirements.txt
```

### 配置
先打开下列两个页面并复制于notion。
1. 任务数据库：
```
https://ubiquitous-myth-d1f.notion.site/1bd1c2c586144ee18b07a6a698edf16f?v=fd6a11be5a5b45b28be53d307940a6ba
```
2. 用户信息配置界面：
```
https://ubiquitous-myth-d1f.notion.site/74dc39a6d0fc41ae9c353d8f2ae734b9?v=b1487a20df1647f2b1cb33e3b61d80f2&pvs=4
```
然后在 `config.py` 文件以设置您用户信息配置界面的token、OpenAI密钥以及openweather API。

### 使用
运行以下命令激活您的个人助理：
```bash
python main.py
```
启动应用程序前，请确保 `config.py` 中的所有配置都是正确的。

## 贡献
我们欢迎各种形式的贡献。要贡献，请：
1. Fork仓库。
2. 创建您的功能分支。
3. 如果您添加了功能，请添加测试。
4. 确保您的更改符合项目的编码风格。
5. 提交合并请求。

## 许可证
根据 [Apache 许可证](LICENSE) 许可。

## 联系方式
如需支持或查询，请通过[zihan.jian@outlook.com](mailto:zihan.jian@outlook.com)与我联系。
