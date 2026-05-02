# ⚡ Multi-Agent Power System AI

> 基于多 Agent 协同与长链推理（Long Chain Reasoning）的电力系统分析与工程文档生成平台

---

## 🚀 项目简介

本项目构建了一个面向电力工程领域的多 Agent 智能系统，用于解决：

- 复杂电力系统分析流程长、跨模块依赖强的问题
- MATLAB/Simulink 仿真与工程文档难以联动的问题
- 论文 / 报告生成效率低的问题

系统支持从 **建模 → 控制策略 → 仿真 → 分析 → 文档生成** 的完整自动化闭环。

---

## 🧠 核心能力

- ✅ 多 Agent 协同（Multi-Agent Collaboration）
- ✅ 长链推理（Long Chain Reasoning）
- ✅ 电力系统建模与控制策略生成
- ✅ MATLAB/Simulink 仿真流程辅助生成
- ✅ 自动生成论文 / 技术报告 / 答辩PPT结构

---

## 🏗️ 系统架构
User Input
↓
Controller Agent（任务调度）
↓
┌───────────────┬───────────────┬───────────────┬───────────────┬───────────────┐
│ 建模 Agent     │ 控制策略 Agent │ 仿真分析 Agent │ 分析评估 Agent │ 文档生成 Agent │
└───────────────┴───────────────┴───────────────┴───────────────┴───────────────┘
↓
Verifier Agent（结果校验）
↓
Final Output（论文 / 报告 / 仿真结果）
---

## 🔁 工作流（Workflow）

1. 用户输入研究任务（如：多变流器并网控制策略分析）
2. Controller Agent 拆解任务
3. 多 Agent 并行执行：
   - 建模 Agent：构建数学模型
   - 控制 Agent：生成控制策略（VSG / 双闭环）
   - 仿真 Agent：生成 Simulink 仿真流程
   - 分析 Agent：稳定性 & 供电质量分析
   - 文档 Agent：生成论文内容
4. Verifier Agent 进行结果校验
5. 输出完整工程结果

---

## 🧩 Agent 设计

### 1. Controller Agent
- 任务拆解
- 推理路径规划
- 多 Agent 调度

### 2. Modeling Agent
- 电力系统建模
- 参数配置
- 拓扑结构生成

### 3. Control Agent
- VSG 控制策略
- 电压电流双闭环
- 控制参数优化

### 4. Simulation Agent
- Simulink 模型构建
- 仿真流程设计
- 数据采集

### 5. Analysis Agent
- 稳定性分析
- 动态响应分析
- 供电质量评估

### 6. Document Agent
- 论文写作
- 报告生成
- PPT结构输出

### 7. Verifier Agent
- 公式校验
- 数据合理性校验
- 工程规范检查

---

## 📊 示例应用

### 📌 多变流器并网控制研究

输入：
输出：
- 控制策略设计
- MATLAB 仿真流程
- 稳定性分析报告
- 论文章节（第3/4章）

---

## 📁 项目结构
multi-agent-power-system-ai/
│
├── agents/
│   ├── controller.py
│   ├── modeling_agent.py
│   ├── control_agent.py
│   ├── simulation_agent.py
│   ├── analysis_agent.py
│   ├── document_agent.py
│   └── verifier_agent.py
│
├── workflows/
│   └── power_system_workflow.py
│
├── prompts/
│   ├── modeling_prompt.txt
│   ├── control_prompt.txt
│   ├── simulation_prompt.txt
│   └── document_prompt.txt
│
├── examples/
│   ├── vsg_case.md
│   └── substation_design.md
│
├── outputs/
│   ├── reports/
│   └── simulations/
│
├── README.md
└── requirements.txt
---

## ⚙️ 技术栈

- LLM：GPT / Claude / Xiaomi MiMo
- Agent 框架：AutoGen / CrewAI（可扩展）
- 仿真工具：MATLAB / Simulink
- 编程语言：Python

---

## 📈 使用效果

- 文档生成效率提升：**5~8倍**
- 仿真分析效率提升：**40%+**
- 支持长文本推理（>50k tokens）

---

## 📌 未来规划

- 接入企业知识库（RAG）
- 电网行业定制模型微调
- Web 可视化界面

---

## 📄 License

MIT License
