# Engineering OS · 电路设计 AI 协作骨架

一套放在 Obsidian 库（或任何 Markdown 目录）里的协作规则，让 AI 做模拟电路设计时：

| 痛点 | 这套骨架怎么解决 |
| --- | --- |
| 经验沉淀不下来，换个会话就失忆 | 每个任务收尾做一次「记忆筛选」，把可复用的经验归到固定位置；下个任务开工先读相关部分。见 [[Memory]]、[[Circuit Experience]]。 |
| 约定总要重讲，换个项目就忘 | 约定和验收门槛先写进规格文件，状态与下一步写回原条目。新会话只说一句「继续」就能找回。见 [[Handoff and Verification]]、[[Start a Task]]。 |

另外约束一件事：实现和评审分开。写的人不给自己打「通过」。见 [[Roles]]。

## 目录

| 文件 | 作用 |
| --- | --- |
| [[AGENTS]] | 协作规则入口，AI 开工先读它 |
| [[Roles]] | 五个角色：谁接什么、交付什么 |
| [[Start a Task]] | 开工手册与短句口令 |
| [[Handoff and Verification]] | 任务状态、接力格式、按风险选验收证据 |
| [[Memory]] | 任务收尾、收工整理、按角色回查 |
| [[Circuit Experience]] | 长期电路经验的格式与三条示例 |
| [[Projects]] / [[Learning]] / [[Experiments]] | 三个索引，各放一个条目模板 |
| [[Task Log]] | 只追加的工作日志 |
| `examples/sky130-five-transistor-ota/` | 一个完整案例的摘要：规格、结果、图、边界 |

## 怎么用

1. 把这些文件放进你的库根目录，让 AI 在该目录里工作。
2. 在 [[Projects]] 里写第一个项目的目标和验收，再对 AI 说「Jarvis」或「继续」。
3. 每个任务结束时说「Jarvis，收工」，让它按 [[Memory]] 沉淀。
4. 把你自己的经验写进 [[Circuit Experience]]，示例条目可以删。

## 说明

- 这是骨架。示例经验只是演示格式，不含任何真实项目数据。
- 案例用开源 SKY130 PDK 和 ngspice。公开版只含摘要，不含原始波形和运行脚本；复现需要自行安装 ngspice 与 SKY130 PDK。
- 这里没有「比不用它省多少时间或 token」的对照数据，所以不做这类声称。
- 许可证：MIT，见 [LICENSE](LICENSE)。
