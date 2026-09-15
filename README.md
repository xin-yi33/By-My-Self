# 阮心一 · XinYi Ruan

**数据科学与大数据技术本科生 · AI Agent 开发 · 数据分析与全栈开发**

广东培正学院 · 数据科学与计算机学院 · 2024 – 2028 · 广州

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Vue 3](https://img.shields.io/badge/Vue_3-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

---

## 关于我

- 广东培正学院 · 数据科学与计算机学院，**数据科学与大数据技术**专业（2024 – 2028），GPA 3.55/4（专业前 10%）
- 主要方向：**AI Agent 与大模型应用**、**数据分析 / 大数据**、**全栈开发**
- 日常深度使用 AI Agent 工具链（Claude Code、Codex、OpenCode 等），熟练使用各种 Skill 与 MCP，并自研本地多智能体框架
- 学生科研项目：**Individualized Agent —— 一种面向个性化 LLM 智能体的受管理自进化架构**（指导教师：李俊），负责架构设计与方法实现
- 习惯以工程化方式解决真实问题：从数据采集、模型训练到 Web 应用完整落地

## 教育背景

**广东培正学院** · 数据科学与计算机学院 · 数据科学与大数据技术（本科） · 2024 – 2028

- GPA 3.55 / 4（专业前 10%）
- 主修课程：Python、数据结构与算法、数学分析、线性代数、概率论与数理统计、统计学、Linux 操作系统、数据库原理与应用
- 自学课程：Hadoop、Spark、HiveSQL、JavaWeb、BI

## 技术栈

| 方向 | 内容 |
|------|------|
| 编程语言 | Python · Java · JavaScript · SQL |
| 数据分析 | pandas · numpy · matplotlib · seaborn · scikit-learn（清洗 / 特征工程 / EDA / 可视化全流程） |
| 大数据 | Hadoop · Hive · Spark（PySpark）· HDFS · Parquet |
| AI 与深度学习 | PyTorch · YOLO · LangChain · RAG · ChromaDB · Embedding · Prompt Engineering · DeepSeek API |
| 数据库 | MySQL（复杂查询 / 窗口函数 / 多表连接） |
| Web 开发 | Flask · Vue 3 · Element Plus · SpringBoot · HTML / CSS / JavaScript |
| 工具链 | Linux · Git · Playwright · Tesseract OCR · Jupyter Notebook · AI Agent / MCP |

## 开源项目

| 项目 | 简介 | 技术栈 |
|------|------|--------|
| [RxyCode](https://github.com/xin-yi33/RxyCode) | 本地多智能体，能干的不只是写代码 —— Local multi-agent for real work, not just code | Python · TypeScript · Electron · React · MCP · TUI |
| [coding-agent-crew](https://github.com/xin-yi33/coding-agent-crew) | 把一次 AI 会话变成动手干活的工程师团队，创建与改进 Codex 形态的编码智能体 | PowerShell · Electron · MCP · JSON-RPC |
| [-novel-writer-skill](https://github.com/xin-yi33/-novel-writer-skill) | 小说写作辅助工具：从细纲到完整章节的创作引擎，支持本地写作与在线发布到番茄小说平台 | Python · Agent Skill |
| [gaokao](https://github.com/xin-yi33/gaokao) | 高考志愿智能择校推荐系统，覆盖全国 31 省 7700+ 院校，冲/稳/保三档推荐 | Flask · Vue 3 · MySQL |

## 项目经历

**高考志愿智能填报系统（全栈）** · 2025.06
- 覆盖全国 31 个省份、7700+ 所院校；基于省位次差的录取概率模型，智能生成冲 / 稳 / 保三档志愿方案
- 后端 Flask 3.x 实现 14 个 RESTful API，前端 Vue 3 + Element Plus 构建 4 个核心页面，MySQL 8.0 七张核心数据表
- 多源数据采集：Playwright 爬虫 + 三源搜索引擎交叉验证 + Tesseract OCR 管线 + pdfplumber / openpyxl 解析

**基于 LangChain 的 RAG 知识库智能问答系统** · 2025.10
- 实现索引 – 检索 – 生成三阶段标准流程；ChromaDB 向量库 + DashScope Embedding（1536 维）+ DeepSeek 生成
- 基于 LCEL 编排可组合处理链；FileChatMessageHistory 实现多会话隔离的持久化对话记忆

**基于 YOLO 的安全帽佩戴目标检测系统** · 2025.10
- 基于 PyTorch 从零实现 YOLOv1：VGG16 预训练骨干、自定义三项加权损失函数、完整的训练与推理管线

**房地产市场数据分析与可视化** · 2025.10
- 10 万+ 条二手房交易数据全流程分析：数据清洗、10+ 衍生特征工程、7 个维度深入分析、10+ 可视化图表

**某原创音乐网站歌曲数据采集** · 2025.10
- JS 逆向还原请求签名算法（execjs 调用还原的类 MD5 逻辑），requests + lxml/XPath 批量采集与音频自动化下载

**店铺销售数据分析（PySpark）**
- 针对 JSON 原始销售数据完成清洗与多维度统计（销售额排行 / 达标店铺数 / 平均单价 / 支付占比），分析结果多端落地 MySQL 与 Hive

## GitHub 概览

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=xin-yi33&show_icons=true&hide_title=true&hide_border=true)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=xin-yi33&layout=compact&hide_title=true&hide_border=true)

## 联系我

- GitHub：[@xin-yi33](https://github.com/xin-yi33)
- Email：ruanxinyi293@gmail.com ｜ 1262075942@qq.com（详细简历可邮件索取）

---

## About Me (English)

Hi, I'm **XinYi Ruan**, an undergraduate at **Guangdong Peizheng College** majoring in Data Science and Big Data Technology (2024 – 2028, GPA 3.55/4, top 10% of the major).

I build around **AI agents**: a local multi-agent system ([RxyCode](https://github.com/xin-yi33/RxyCode)), coding-agent tooling, and an AI novel-writing assistant skill. My hands-on experience covers data analysis (pandas/Spark), deep learning (PyTorch/YOLO), RAG systems (LangChain + ChromaDB), and full-stack development (Flask / Vue 3 / MySQL).

- Student research: **Individualized Agent** — a governed self-evolution architecture for personalized LLM agents
- Contact: ruanxinyi293@gmail.com ｜ 1262075942@qq.com
