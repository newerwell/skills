# 阅读资料

| 想解决的问题 | 原文以及适合阅读的内容 |
| --- | --- |
| 这个项目值得投入多少工程成本？ | 从代码的预期寿命、使用规模和维护成本权衡。[Titus Winters · What Is Software Engineering?](https://abseil.io/resources/swe-book/html/ch01.html) |
| 代码审查先看什么？ | 优先判断设计、行为和测试是否有效。[Google · What to Look for in a Code Review](https://google.github.io/eng-practices/review/reviewer/looking-for.html) |
| 一次变更应该多大？ | 围绕一个可独立理解的目的拆分，带上相关测试。[Google · Small CLs](https://google.github.io/eng-practices/review/developer/small-cls.html) |
| 现在需要加这层抽象吗？ | 根据已经出现的需求判断扩展点有没有价值。[Martin Fowler · YAGNI](https://martinfowler.com/bliki/Yagni.html) |
| 该写哪一层测试？ | 让快速的局部检查和少量完整流程验证各自覆盖合适的风险。[Ham Vocke · The Practical Test Pyramid](https://martinfowler.com/articles/practical-test-pyramid.html) |
| 如何及早发现集成问题？ | 频繁集成，用自动构建和测试缩短反馈时间。[Martin Fowler · Continuous Integration](https://martinfowler.com/articles/continuousIntegration.html) |
| Web 服务怎样稳定交付？ | 显式声明依赖、分离配置与代码，缩小运行环境差异。[The Twelve-Factor App（简体中文）](https://12factor.net/zh_cn/) |
| Agent 反复犯同样的错怎么办？ | 把反复纠正的错误转成代码约束，通过真实入口验证行为。参看 Lauren Tan 的[演讲与字幕](https://ai.engineer/code/2026/talks/lauren-tan)、[pstack 源码](https://github.com/cursor/plugins/tree/main/pstack)、[重复错误处理](https://github.com/cursor/plugins/blob/main/pstack/skills/correct/SKILL.md)和[应用验证流程](https://github.com/cursor/plugins/blob/main/pstack/skills/create-verification-skill/SKILL.md)。 |
