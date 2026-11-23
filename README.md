# 科研工作台 / Research Tracker

> 单文件、纯前端、离线可用的学术投稿追踪工具。数据只存在你自己的浏览器里，无需服务器、无需联网。
> A single-file, frontend-only, offline-capable academic submission tracker. Your data lives only in your own browser — no server, no internet required.

---

## 简介 / Introduction

科研工作台帮助你管理「论文文件夹 + 多篇投稿」两层结构的研究产出：追踪每篇论文的投稿轮次、审稿状态、期刊等级，并以图表呈现进展。

Research Tracker helps you manage research output as a two-level model of *paper folders + multiple submissions*: track each paper's submission rounds, review status, and journal tiers, and visualise progress with charts.

本项目提供两个相互独立、但功能对等的版本：

This project ships two independent yet functionally equivalent versions:

| 版本 / Version | 入口 / Entry | 界面语言 / UI language |
|---|---|---|
| 中文版 / Chinese | [`zh/index.html`](zh/index.html) | 简体中文 + 繁體中文（香港） |
| 英文版 / English | [`en/index.html`](en/index.html) | English only |

---

## 功能 / Features

- 论文文件夹 + 多篇投稿两层数据模型 / *Paper folder + multiple submissions, two-level data model*
- 中英双语论文标题、作者位次 / 共一 / 通讯标记 / *Bilingual titles; author order / co-first / corresponding-author markers*
- 期刊等级多选与优先级（中文版：JCR / CSSCI / CSCD / CCF / 北大核心 / EI / Scopus 等）/ *Multi-select journal tiers with priority (English: JCR / EI / Scopus …)*
- 投稿轮次与状态追踪、进展时间线 / *Submission rounds & status tracking, progress timeline*
- 论文级「修改中」状态（major / minor 返修），含筛选与分组 / *Paper-level "Revising" status (major/minor), with filter & grouping*
- 卡片阶段时长贴图（当前阶段、已停留天数、当前投稿期刊及等级）/ *Card stage-duration tag: current stage, elapsed days, current journal & tier*
- 多种排序：更新时间 / 首次投稿 / 项目名 / 最近阶段 / 阶段时长 / *Multiple sorts: updated / first submit / title / latest stage / stage duration*
- 统计图表：状态分布 / 期刊等级分布 / 已接收成果分布 / 投稿期刊 TOP 5 / *Charts: status distribution / tier distribution / accepted tiers / top-5 submitted journals*
- CSV / JSON 导入导出 / *CSV / JSON import & export*
- 本地存储，数据仅存本机浏览器 / *Local storage — data stays on your device*

---

## 两个版本的差异 / Differences between the two versions

| 维度 / Dimension | 中文版 / Chinese (`zh/`) | 英文版 / English (`en/`) |
|---|---|---|
| 界面语言 / UI language | 简体中文 + 繁體中文（香港），可切换 *Simplified + Traditional Chinese (HK), switchable* | English only (no switcher) |
| 期刊自动匹配 / Auto-match | 保留 easyScholar 开放 API（需自填密钥）*Keeps easyScholar open API (bring your own key)* | 不适用 / *N/A* |
| 期刊等级体系 / Tiers | 含中文体系（CSSCI / CSCD / CCF / 北大核心 等）*Includes Chinese tiers (CSSCI / CSCD / CCF / Peking Core …)* | International tiers only (JCR Q1–Q4 / Scopus / EI / English General) |

---

## 使用方法 / How to use

1. 直接用浏览器打开对应版本的 `index.html` 即可，无需安装、无需服务器。
   *Just open the corresponding `index.html` in your browser. No install, no server.*
2. 所有数据保存在本机浏览器的 `localStorage`，不会上传任何服务器。
   *All data is saved in your browser's `localStorage`; nothing is uploaded.*
3. 建议通过「导出」功能定期备份为 JSON 文件。
   *We recommend exporting to JSON periodically as a backup.*

---

## 隐私 / Privacy

本工具不收集、不上传任何数据。easyScholar 密钥（仅中文版）由你自行填写，只保存在你本机浏览器，不会发送给本工具作者。
*This tool collects and uploads nothing. The easyScholar key (Chinese version only) is entered by you and stored solely in your browser's `localStorage`; it is never sent to the author.*

---

## 目录结构 / Repository structure

```
research-tracker/
├── README.md          # 本文件 / this file (bilingual)
├── LICENSE            # MIT
├── .gitignore
├── zh/
│   ├── index.html     # 中文版（简中 / 港繁）/ Chinese version
│   └── README.md      # 中文版说明 / Chinese README
└── en/
    ├── index.html     # 英文版 / English version
    └── README.md      # 英文版说明 / English README
```

---

## 许可证 / License

[MIT](LICENSE) © 2026 starry
