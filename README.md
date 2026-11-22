# Listing 优化清单

> 一套给跨境卖家用的 **Listing 上架前自检流程**。不谈玄学，每一条都能逐字核对。
> 基于 Amazon + TikTok Shop 实战迭代，覆盖标题、五点、图片、搜索词、描述全流程。

**作者：The Minotaur**

## 这是什么

很多 Listing 不是写得不好，而是**写之前没核对事实**、**写完没人逐项检查**。
这份清单把优化动作拆成 8 个步骤，每步给出可勾选的检查项 + 正反案例。

适合：
- 自己做 Amazon / TikTok Shop 的卖家
- 上架前需要一套固定流程的人
- 想降低"改完反而变差"风险的运营

## 免费版包含

- [x] `SKILL.md` — 标准 Skill 入口，可被 AI 智能体直接加载
- [x] `references/checklist.md` — 8 个环节的完整自检清单（40+ 检查项）
- [x] `references/before-after-example.md` — 一条 Listing 的脱敏改写案例
- [x] `assets/fact-sheet-template.md` — 产品事实核对表
- [x] `assets/title-workspace-template.md` — 标题改写工作底稿
- [x] 平台差异速查（Amazon vs TikTok Shop）

## 作为 AI Skill 安装

本仓库已是标准 Skill 格式（含 `SKILL.md` + YAML frontmatter）。三种安装方式：

**方式 1 — 下载 zip（推荐）**
从 Releases 下载 `listing-optimization-checklist.zip`，解压到技能目录：

| 工具 | 目录 |
|---|---|
| WorkBuddy / CodeBuddy | `~/.workbuddy/skills/listing-optimization-checklist/` |
| Claude Code | `~/.claude/skills/listing-optimization-checklist/` |

解压后目录里应直接看到 `SKILL.md`。重启智能体即可在技能列表中看到「Listing 优化清单」。

**方式 2 — Git 克隆**
```bash
git clone https://github.com/jackyniu66-cmyk/listing-optimization-checklist.git ~/.workbuddy/skills/listing-optimization-checklist
```

**方式 3 — 让智能体装**
把本仓库链接发给智能体，说「帮我安装这个 Skill」。

触发方式：直接说「帮我检查这条 listing」「重写标题和五点」「上架前自检」等，智能体会自动加载。

## 完整版（付费）

| 内容 | 免费版 | 完整版 |
|---|---|---|
| 自检清单 | 基础版 | 40+ 项完整版 |
| 改写案例 | 1 个 | 10 个（多品类） |
| 标题公式库 | — | ✅ |
| 五点填空模板 | — | ✅ |
| 图片审稿批注表 | — | ✅ |
| 竞品对标表 | — | ✅ |
| 月度更新 | — | ✅ |

完整版获取方式见下方「变现版本」章节，或联系作者 The Minotaur。

## 手动使用方法（不装 Skill 也能用）

1. 复制 `assets/fact-sheet-template.md`，把产品事实填完
2. 照 `references/checklist.md` 的顺序逐项过
3. 用 `assets/title-workspace-template.md` 出 3 个标题候选
4. 发布前跑一遍第 7 节「终检」

## 变现版本

本仓库是**免费引流版**。如果你拿到的是完整版，请通过正规渠道购买，不要二次分发。

- Gumroad：（上架后填链接）
- Payhip：（上架后填链接）

## License

免费版文件采用 [CC BY-NC 4.0](./LICENSE) — 可自由分享、标注出处，**不可商用**。
完整版内容不包含在本授权内。
