# Query Plan

目前matrixone的plan构建过程，没有与代码关联紧密的文档。此外，复杂的代码逻辑加重了业务团队的学习负担。

0.6, 0.7，在业务开发和维护过程，相当多的地方需要修改到plan代码。当前出现的弊端是非plan的原始开发人员，无法深入到涉及plan的功能开发和bug修复过程中，导致相关的feature和bug积压到少数人身上。单人负担重，质量和效率难上去。业务团队也没成长起来。随着代码的复杂化，在后续版本中，业务团队大概率会重蹈覆辙。

本文以tpch的sql为例，根据自己的理解，分析matrixone的plan构建过程。注重代码逻辑的理解。会讲解关键代码的思路，但不会讲每一行代码。会引用代码的片段，辅助讲解。必要时会提供图片释义。先以q1为例子，后续逐步增加更复杂的sql。

目标是让业务团队能够掌握这块内容，在业务开发过程中得心应手游刃有余。

囿于笔者水平，难免有疏漏。欢迎斧正。

## 目录

[第一章 单表](./ch1.md)

[未完待续]()
