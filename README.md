# David Perell Skill 工具箱

用于写作、思考与持续发表。包含独立主入口、学习地图、行动路线、专属流程、IMA检索和更新入口。

## 安装

```text
npx -y skills add FocusLiz-Lab/dpskill -g --all
```

首次使用 `$dps` 描述目标；也可直接调用子Skill。Python 3.10+ 用于本地证据检索和更新；IMA检索另外需要安装并配置官方ima-skill。普通工作流无需联网。

## 路由

| 路由 | 用途 | 产物 |
|---|---|---|
| `$dps` | 主入口 | 诊断并执行对应流程 |
| `$dps-learning-map` | 学习地图 | 能力地图与当前起点；分阶段阅读路径及真实来源；练习成果与检验标准 |
| `$dps-roadmap` | 行动路线 | 目标与瓶颈诊断；阶段行动及交付物；检查指标、风险与调整条件 |
| `$dps-ideas` | 观察素材与选题 | 素材整理；选题候选；展开角度 |
| `$dps-thinking` | 通过写作澄清观点 | 核心问题；推理链；待验证清单 |
| `$dps-writing` | 文章结构与初稿 | 文章大纲；段落安排；初稿 |
| `$dps-editing` | 论证与表达修改 | 问题诊断；修改建议；修改稿 |
| `$dps-publishing` | 持续发表与读者反馈 | 发表安排；反馈问题；改进与复用计划 |
| `$dps-ima` | 明确要求IMA检索 | 来源与证据 |
| `$dps-update` | 更新全部Skill及原子库 | 更新结果与提交号 |

## 来源与边界

首版包含 1718 条有限来源片段，实际来自 639 个去重来源（候选来源 659 个）。中英文按视频ID或文章URL合并，只取一份，优先完整中文；缺失或明显残缺时回退英文。

首版原子 type=source、confidence=medium，未经逐条人工验证，不是作者已验证结论。source_expert仅表示资料所属知识库；访谈观点需核实实际发言者。方法说明是工作流综合，使用时必须检索实际证据。来源日期和范围见 source-audit.json 与主Skill原子目录 source_catalog.json。

本项目不是作者或机构官方产品，不模仿人设，不承诺收入、健康或投资结果。原始材料权利归其权利人；这里只提供有限来源片段、索引与原创工作流，不打包整篇文稿。

## 更新

调用 `$dps-update`，或在任意子Skill中明确要求“更新skill和原子库”。检查更新运行当前Skill的 tools/update_skill.py --check。下载固定main提交，写入前备份，失败回滚。

## 未入库来源

- no_unique_qualifying_excerpt: 20

无法确认身份的历史稿件暂不原子化，避免中英文重复；详情见 source_catalog.json。缺口不能理解为已经处理完成。
