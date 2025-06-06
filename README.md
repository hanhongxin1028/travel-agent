# 🌏 旅游攻略智能 Agent 项目

---

## 🚀 项目简介

本项目旨在打造一个智能旅游助手Agent，集成旅游攻略制定、车票和酒店推荐、团购优惠推送等核心功能，帮助用户高效规划旅行，享受便捷愉快的出行体验。

---

## 📋 功能模块

| 模块名称           | 主要功能描述                                             |
|--------------------|----------------------------------------------------------|
| 🧠 意图识别模块     | 通过大语言模型（LLM）解析用户自然语言输入，提取关键出行信息，输出结构化 JSON 格式供后续调用。 |
| 🗺️ 行程规划模块    | 根据用户需求与偏好，智能生成合理的旅游行程方案。               |
| 🚆 车票推荐模块     | 实时查询并推荐符合用户行程的交通票务选项。                     |
| 🏨 酒店推荐模块     | 结合用户偏好与行程，推荐优质酒店资源。                         |
| 🛍️ 团购推荐模块    | 汇聚当地优惠团购及活动，提升旅行性价比。                       |
| 📊 结果展示模块     | 以简洁友好的界面形式展示最终旅游攻略和推荐结果。                 |

---

## 📁 仓库结构
```
travel-agent/
├── configs/
│   ├── llm_config.yaml           # 存储 LLM API Key、模型设置等
│   └── planner_config.yaml       # 可选：行程规划等模块的参数
│
├── modules/
│   ├── intent_recognition/       # 意图识别模块
│   ├── itinerary_planner/        # 行程规划模块
│   ├── ticket_recommendation/    # 车票推荐模块
│   ├── hotel_recommendation/     # 酒店推荐模块
│   ├── groupbuy_recommendation/  # 团购推荐模块
│   └── result_display/           # 结果展示模块（如统一输出格式、UI）
│
├── common/                       # 公共工具函数（如 LLM 接口封装、日志）
│   ├── llm_interface.py
│   ├── logger.py
│   └── utils.py
│
│
├── tests/                        # 单元测试，每个模块一个文件
│   ├── test_intent_recognition.py
│   └── ...
│
├── run.py                        # 主程序入口（负责加载配置，调用模块）
├── requirements.txt              # 项目依赖
├── README.md                     # 项目介绍
├── CONTRIBUTING.md               # 协作指南
└── .gitignore                    # 忽略缓存、venv、日志等

```
---

## 💻 环境搭建
* Python 版本建议 3.9 及以上

* 安装依赖：
```bash
pip install -r requirements.txt
```
---

## 🛠️ 开发流程简要
1. 克隆仓库，切换到 `dev` 分支。

2. 创建功能分支，命名规范为 `feature/模块名称`。

3. 本地开发，频繁提交，推送功能分支。

4. 创建 Pull Request，关联 Issue，等待代码 Review。

5. Review 通过后合并到 dev 分支。

6. 持续同步 dev 分支最新代码。

详细流程请参考 https://github.com/hanhongxin1028/travel-agent/blob/main/CONTRIBUTING.md
