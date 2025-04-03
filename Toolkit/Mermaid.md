# Diagramming With Mermaid

- [文档、工具](#文档工具)
- [Flowchart（流程图）](#flowchart流程图)
  - [常用符号](#常用符号)
  - [语法](#语法)
- [Pie chart（饼状图）](#pie-chart饼状图)
- [Mindmap（思维导图）](#mindmap思维导图)
- [XY Chart（柱状曲线图）](#xy-chart柱状曲线图)
- [Class diagrams（类图）](#class-diagrams类图)
- [Gantt (甘特图)](#gantt-甘特图)


## 文档、工具
- [About Mermaid](https://mermaid.js.org/intro/)
- [关于 Mermaid](https://mermaid.nodejs.cn/intro/)
- [Live Editor（文生图）](https://mermaid.live/)
- [Mermaid Chart（图生文）](https://www.mermaidchart.com/)
- [Kroki（文本绘图服务，分享链接更简短）](https://kroki.io/)

## Flowchart（流程图）
### 常用符号

| 形状                  | 描述                                                         | 代码                                                                                      |
| --------------------- | ------------------------------------------------------------ | ----------------------------------------------------------------------------------------- |
| ![][Flow_Terminal]    | 起止（Terminal）                                             | `A([Start or End])`                                                                       |
| ![][Flow_Process]     | 程序、动作、操作（Process）                                  | `A[Process]`                                                                              |
| ![][Flow_Decision]    | 决策判断（Decision）                                         | `A{Yes or No}`                                                                            |
| ![][Flow_InOut]       | 输入/输出（Input/Output）                                    | `A[/Input or Output/]`                                                                    |
| ![][Flow_ManualInput] | 手动输入（Manual Input）                                     | `A@{ shape: manual-input, label: "Enter Your ID"}`                                        |
| ![][Flow_Subroutine]  | 已在其他地方定义的子程序（Subroutine or Predefined Process） | `A[[Subroutine]]`                                                                         |
| ![][Flow_Doc]         | 文档（Document）                                             | `A@{ shape: doc, label: "Document" }`<br>`B@{ shape: docs, label: "Multiple documents" }` |
| ![][Flow_Database]    | 数据库（Database）                                           | `A[(Database)]`                                                                           |
| ![][Flow_Comment]     | 注释（Comment）                                              | `A[Function]`<br>`C@{ shape: comment, label: "Brief: \nParams:" }`<br>`A --> C`           |


*参考文档：*
- [What do the different flowchart shapes mean?](https://www.rff.com/flowchart_shapes.php)
- [Flowchart with New Shapes](https://mermaid.js.org/syntax/flowchart.html#example-flowchart-with-new-shapes)

[Flow_Terminal]: https://kroki.io/mermaid/svg/eNpLy8kvT85ILCpR8AniUgACR43o4BIQP79IwTUvJVYTAMANCqM
[Flow_Process]: https://kroki.io/mermaid/svg/eNpLy8kvT85ILCpR8AniUgACx-iAovzk1OLiWAB-eAjr
[Flow_Decision]: https://kroki.io/mermaid/svg/eNpLy8kvT85ILCpR8AniUgACx-rI1GKF_CIFv_xaAI_3CVs
[Flow_InOut]: https://kroki.io/mermaid/svg/eNpLy8kvT85ILCpR8AniUgACx2h9z7yC0hKF_CIF_9ISIEs_FgDlLwws
[Flow_ManualInput]: https://kroki.io/mermaid/svg/eNpLy8kvT85ILCpR8AniUgACR4dqheKMxIJUK4XcxLzSxBzdzLyC0hIdhZzEpNQcKwUl17yS1CKFyPzSIgVPF6VaAMA8FVY
[Flow_Subroutine]: https://kroki.io/mermaid/svg/eNpLy8kvT85ILCpR8AniUgACx-jo4NKkovzSksy81NhYALFaCvQ
[Flow_Doc]: https://kroki.io/mermaid/svg/eNpLy8kvT85ILCpR8AniUgACR4dqheKMxIJUK4WU_GQdhZzEpNQcKwUll_zk0tzUvBIlhVqwOicUdcUIhb6lOSWZBTmpIGGwjmKgFgCMtyEW
[Flow_Database]: https://kroki.io/mermaid/svg/eNpLy8kvT85ILCpR8AniUgACx2gNl8SSxKTE4lTNWACXGQly
[Flow_Comment]: https://kroki.io/mermaid/svg/eNpLy8kvT85ILCpR8AniUgACx2i30rzkksz8vFgw39mhWqE4I7Eg1UohOT83NzWvREchJzEpNcdKQcmpKDM1zUohJi8gsSgxt9hKSaEWYoaCrq6dgjMAQN4bbw

### 语法


## Pie chart（饼状图）

## Mindmap（思维导图）

## XY Chart（柱状曲线图）

## Class diagrams（类图）

## Gantt (甘特图)