# 多元专家研究引擎生成器

一个基于大语言模型的智能研究引擎构造系统，接收任意事项并自动生成定制化的多元专家研究引擎。

## 项目结构

```
├── AGENTS.md                    # 生成器提示词
├── 0-build-agents.md            # 构造元指令
├── 1-engine-design.md           # 引擎设计规范
├── 2-example-research-result.md # 参考案例
├── rules/                       # 通用规则库
│   ├── research-report-writing.md
│   ├── data-source-evaluation.md
│   ├── quality-review-workflow.md
│   ├── fact-check-workflow.md
│   ├── few-shot-research-report.md
│   └── few-shot-synthesis.md
└── tasks/                       # 生成的引擎实例目录
```

## 核心功能

- **事项分析**：接收自然语言描述的研究事项，分析其属性和复杂度
- **引擎生成**：为事项量身定制多维度专家研究引擎
- **工作流规划**：设计完整的研究工作流程和阶段门控
- **专家体系**：配置维度专家、横向专家、综合判断专家等

## 工作原理

1. 用户输入研究事项（如决策问题、科研课题、对比分析等）
2. 生成器分析事项属性，推导研究维度和专家配置
3. 生成包含 `main.md` 入口的引擎实例文件
4. 另一个 AI 加载引擎执行研究，最终产出学术报告

## 使用要求

- 支持大语言模型 API（用于 AI 执行研究）
- 文件路径引用需要与 `./1-engine-design.md` 规范保持一致

## 相关文档

- [AGENTS.md](AGENTS.md) - 生成器完整提示词
- [1-engine-design.md](1-engine-design.md) - 引擎设计规范
- [2-example-research-result.md](2-example-research-result.md) - 研究成果示例
