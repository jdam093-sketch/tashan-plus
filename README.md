版本：v2（2026-11-24）

# 他山增强版 · Tashan Plus

**想学一个不熟的方向，让智能体去看别人怎么做——最怕出处是编的，或者一上来就铺很大一摊。**

他山增强版用来“取经”：从外部公开的做法里，看别人怎么分工、怎么把关，提炼出你能搬走的原则，写成一页笔记，或者提示词、SOP、技能草案。

默认走**快速档**：看 3–5 个样本，交一页写明出处的笔记，样本按核实程度分级。要做**完整档**时，它先报时间、费用和检验安排，你说“开始”它才动手。涉及敏感材料，先按隐私规则处理。

> **非官方改编版，改编自 [zhenxishuai/tashan-skill](https://github.com/zhenxishuai/tashan-skill)（MIT）。** 原作者 Tashan contributors，改动者 beyond zhang。这不是原作者的官方版本。许可全文和版权行见 [LICENSE](LICENSE)，中英声明见 [NOTICE](NOTICE.md)，来源核对见 [来源说明](来源说明.md)。

### 三步上手

1. 下载本仓库，把整个 `tashan-plus` 文件夹放进智能体的个人技能目录（Claude Code 用 `~/.claude/skills/`，Codex 用 `~/.agents/skills/`）。工具不支持装技能的，把 `SKILL.md` 发给它，说“请按这份说明工作”。
2. **新开一个对话**，直接说：“取经一下：开源项目怎么写贡献指南，给我一页笔记。”
3. 要认真做时加上“完整档”。它会先给出预估，等你说“开始”。

## 文件入口

| 文件 | 用途 |
|---|---|
| [SKILL.md](SKILL.md) | 主规则、触发边界、两档分流 |
| [快速档](references/快速档.md)、[完整档](references/完整档.md) | 按档位读详细步骤 |
| [隐私规则](references/隐私规则.md) | 涉及敏感材料或外发时读取 |
| [纠正写回规则](references/纠正写回规则.md)、[待吸收意见](待吸收意见.md) | 当次草稿、中央登记、统一改版 |
| [一页笔记](templates/一页笔记.md)、[完整笔记](templates/完整笔记.md)、[提示词骨架](templates/提示词骨架.md) | 通用产出模板 |
| [法律合规](templates/领域-法律合规.md) | 适用：中国大陆；按需读取 |
| [两个合成示例](references/examples.md) | 快速档笔记与完整档预估单，非实测 |
| [CHANGELOG.md](CHANGELOG.md) | 当前变化、历史摘要和统一后续清单 |
| [来源说明](来源说明.md)、[NOTICE.md](NOTICE.md)、[LICENSE](LICENSE) | 来源、非官方改编声明及 MIT 全文 |

## 怎么用

- “取经一下：开源项目怎么写贡献指南，给我一页笔记。”
- “完整档：横向对标公开的贡献流程，沉淀成长期使用的 SOP 草案。”

出练习用 learning-practice，媒体笔记用 media-to-knowledge，还原事件用 evidence-reconstruction，制作已定点子的小样用 idea-to-prototype，需求判断用 product-demand-validation。只分析一份合同等具体材料直接处理；人物思维和已有技能草案的打包测试交相应功能工具（如已安装）。这些路由不表示已安装或已调用对应工具。

## 许可、验证与后续

改编自 Tashan，原作者 Tashan contributors，来源 https://github.com/zhenxishuai/tashan-skill，MIT 许可；改动者 beyond zhang。此为改编版，非原作者官方版本。许可全文和版权行见 LICENSE，中英声明见 NOTICE。

正文使用中文，description 与 NOTICE 中英双语。各客户端对 frontmatter 字段、自动发现和调用方式的支持【未核实】；仅使用 name、description，不宣称某个平台已经兼容。合成示例不证明真实任务效果；未做联网核验、安装或新会话路由测试。

后续阶段统一见 CHANGELOG.md：其它领域模板、可选抓取加速工具、经授权的多客户端同步、检查小工具脚本。


可以和「眼见 · 个人 AI 基础设施技能包」（仓库 yanjian-skills）搭配使用；两者是独立仓库，许可分开。本仓库依据 v2 公开版发布。
