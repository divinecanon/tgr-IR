# TGR-IR

TGR-IR（Thixotropic Generative Recursion — Intermediate Representation）是一种最小化的原语中间表示，用于描述生成机制本身。

TGR 文档体系中的哲学概念，以及数学、物理、语言等已有表达体系，均可视为 IR 在不同层级上的翻译或表达，而非 IR 的定义来源。IR 的目标不是替代已有理论，而是提供它们共同可映射的底座。

## 当前状态

当前冻结版本：**v6.4**（历史版本见 `docs/archive/`）。

v6.4 核心变化：
- 明确 Ωδ 作为"元锚定声明"的定位（系统运行前提，不可被再次对象化）。
- 明确 Mapping/Translation 为纯表达层工作，只能发生在 IR 内部生成完成之后。
- 术语体系变更：以"原语（Primitive）／导出结构（Derived Structure）／表达（Representation）"三层体系，及"生成距离"作为唯一层级判据，替代此前边界不清的"一阶／二阶／三阶"划分。

## 文档结构

- [`docs/00-scope.md`](docs/00-scope.md) —— 本规范管什么、不管什么，一页纸说明
- [`docs/01-core-spec.md`](docs/01-core-spec.md) —— 唯一规范正文（哲学主张 / 工程规范 / 机制操作手册）
- [`docs/02-workflow.md`](docs/02-workflow.md) —— 时序工作流（时序0-7，如何产出下一版规范）
- [`docs/03-glossary.md`](docs/03-glossary.md) —— 导出结构词汇表（非独立原语）
- [`docs/mapping/`](docs/mapping/) —— 表达层，IR → 已有理论的映射说明
- [`docs/proposals/`](docs/proposals/) —— 未冻结假说、待定事项（含几何映射假说 H1-H37）
- [`docs/archive/`](docs/archive/) —— 历史版本（v1.0 - v6.3）

具体理论映射的工程案例记录于 [`ir-mapping`](https://github.com/divinecanon/ir-mapping) 仓库。

## 许可

见 [LICENSE](LICENSE)。
