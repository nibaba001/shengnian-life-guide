# 高性价比人生指南 · AI 技能（离线版）

把开源项目[《高性价比人生指南》](https://github.com/eternity4719/HowToLiveBetter)做成一个装进 AI 就能用的技能。遇到「该不该、值不值、怎么选、犯不犯法、出事了先做什么」这类问题，直接问 AI：它先去书里把相关条目查出来，再按书的算账方式（花多少钱、时间、精力，换回什么，证据靠不靠谱）排好序回答，每条都标明出自第几节第几条；书里没写的，直说没查到，不会自己编。

和原项目自带技能的区别：全书 34 节正文已经打包在本仓库的 `data/` 里，不联网也能查；补了 WorkBuddy 的装法。回答规则沿用原作者写的那一套。

## 安装

### 方法一：发一句话，让 AI 自己装（WorkBuddy、Codex 都行）

把下面这段话原样发给你的 AI：

```
帮我安装这个 AI 技能：https://github.com/nibaba001/shengnian-life-guide 。把仓库下载下来，整个文件夹命名为 howtolivebetter-guide，放进你的技能目录（WorkBuddy 是 ~/.workbuddy/skills/，Codex 是 ~/.agents/skills/，Claude Code 是 ~/.claude/skills/），装好后告诉我怎么用。
```

AI 执行下载和复制命令前会请你确认，同意即可。装完没生效的话，重启一下 WorkBuddy / Codex。

### 方法二：一条命令（Codex、Claude Code、Cursor 等）

```bash
npx skills add nibaba001/shengnian-life-guide
```

按提示选择要装到哪个工具。这个命令目前不支持 WorkBuddy，WorkBuddy 请用方法一或方法三。

### 方法三：手动

点本页的 Code → Download ZIP，解压后把文件夹改名为 `howtolivebetter-guide`，复制到对应的技能目录（见方法一），重启工具。

## 怎么用

直接把问题和你的实际情况告诉它，越具体越好，比如：

- 朋友让我替他担保，签不签？
- 每天通勤两小时，值不值？
- 被公司裁员了，第一步该做什么？
- 想把钱存起来，放哪里不被费率和骗局吃掉？

它会按这个结构回答：一句话结论 → 先做这几条（每条标出处，比如「第 8 节第 18 条」）→ 别做的 → 书里没写的。

只想看书、不装 AI：原项目提供[在线检索页](https://eternity4719.github.io/HowToLiveBetter/)，以及 PDF、EPUB 和离线单文件网页版，入口在[原项目 README](https://github.com/eternity4719/HowToLiveBetter)。

## 注意

- 书给的是通用口径，不替代医生、律师、会计；涉及具体病情、案件、税务，以专业人士为准。
- 政策类的金额、时限会变，答复里会带上书里写的截止日期，请再到官方渠道核对。
- `data/` 是 2026-10-07 的正文版本，作者一直在更新；`SKILL.md` 里写了联网取最新正文的方法。

## 来源与协议

- 原书：《高性价比人生指南》，作者 [eternity4719](https://github.com/eternity4719)，原项目 https://github.com/eternity4719/HowToLiveBetter
- 正文（`data/book`、`data/docs`、`data/README.md`）按 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.zh-hans) 使用，见 [LICENSE](LICENSE)。
- 技能规则 `SKILL.md` 改编自原项目的 `skills/life-decision-guide`，和 `data/index.html` 一起按 MIT 使用，见 [LICENSE-CODE](LICENSE-CODE)。
- 本仓库做了哪些改动见 [来源与署名.md](来源与署名.md)；书的内容未做修改。
- 整理：盛年
