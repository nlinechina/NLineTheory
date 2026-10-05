# NLineTheory（联线理论）

> **A pattern-triggered hierarchical reduction method for financial sequential data**
> 面向序列数据的模式触发层次归约方法

[官网 nlinechina.com](https://www.nlinechina.com) ｜ [NLINE 联线智库](https://github.com/nlinechina)

---

## 一、这是什么

联线理论（NLineTheory）是一套针对 K 线序列的结构分析理论：
将原始行情经**八层单向归约**，逐层抽出可确定、可复现的结构标注，对
线段、转折、形态与计数给出严格定义。

| 层 | 名称 | 层 | 名称 |
|----|------|----|------|
| L1 | 同组 | L5 | 转折 |
| L2 | 异组 | L6 | 形态 |
| L3 | 恒组 | L7 | 折叠 |
| L4 | 线段 | L8 | 计数 |

三个特征：

- **确定性** —— 同一输入必得同一输出（同一段行情两次编译结果唯一）
- **单向分层** —— 层间只传数值，不互相改写逻辑；每层职责由规范严格定义
- **原文可溯** —— 每条规则可在理论文档中找到出处，禁止无依据的桥接概念

## 二、为什么存在

主流技术分析语言中，「回调还是反转」这类判断边界含混、不可复现——
同一段行情，不同的人（甚至同一个人在不同时候）给出不同答案。联线理论
把这类判断改写为**可执行的判定规则**，使市场结构分析第一次具备
「同题同答」的可检验性。它研究的是序列数据的波动规律；金融只是当前
的数据源，不是边界。

## 三、从哪读起

```
docs/
├── outline/          原始大纲（理论源头）
├── whitepaper/       白皮书四章：K线组合 → 线段转折 → 形态归集 → 计量系统
├── specification/    L1–L8 各层规范
├── canonical-cases/  标准案例
└── research/         研究参与与复现协议
src/                  参考实现（Reference Implementation，教学导向）
tests/                测试向量（机器可读）
```

> 本仓库处于 v0.1 准备阶段，部分目录随发布逐步就位。
> 规范 + 参考实现 + 测试向量三者互验：跑通测试即理解验收标准。

## 四、如何引用

见 [CITATION.cff](CITATION.cff)：

```bibtex
@misc{nlinetheory2026,
  title  = {NLineTheory: A Pattern-Triggered Hierarchical Reduction Method
            for Financial Sequential Data},
  author = {Song, Shugang},
  year   = {2026},
  url    = {https://github.com/nlinechina/NLineTheory}
}
```

## 五、如何参与 / 商业授权

- **勘误与贡献**：[CONTRIBUTING.md](CONTRIBUTING.md)（首次 PR 视为签署 CLA）
- **研究合作**：复现协议与数据接口见 `docs/research/`，或来信
- **商业实施**：生产级实现、API、企业集成、认证兼容为商业授权范围；
  官方身份相关表述规范见 [TRADEMARKS.md](TRADEMARKS.md)
- 联系：**songshugang@nlinechina.com**

## 许可

| 范围 | 许可 |
|---|---|
| 代码（`src/`、`tests/`、`tools/`） | [Apache-2.0](LICENSE) |
| 文档与规范（`docs/`、各 `.md`） | [CC BY 4.0](LICENSE-DOCS) |
| 商标与官方身份 | [TRADEMARKS.md](TRADEMARKS.md)（不随开源许可授予） |

权属与存证：[PROVENANCE.md](PROVENANCE.md) ｜ 历史时间线：[HISTORY.md](HISTORY.md) ｜
更正制度：[ERRATA.md](ERRATA.md) ｜ 治理：[GOVERNANCE.md](GOVERNANCE.md)

---

*联线理论 © 2026 湖南联线智库信息科技有限公司。理论 © 与规范由权利方
持续维护；「官方身份」永远不在开源范围之内。*
