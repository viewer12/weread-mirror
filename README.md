# weread-mirror

A private reading portrait, generated from 8 years of WeRead (微信读书) data by an AI third-party evaluator.

一份基于微信读书 8 年数据生成的私人读书画像。由 AI 作为第三者评估者撰写——不吹捧、不奉承、不和外部基准对比，所有解读都从可指认的数据点出发。

→ [在线浏览（GitHub Pages，需仓库主开启）](https://viewer12.github.io/weread-mirror/)

---

## 项目特点

- **数据驱动**：488 本书架 / 55 本读完 / 681 条笔记 / 1041 个阅读日 / 8 年逐年统计
- **AI 第三者视角**：Claude 作为 AI 评估者撰写，不替主人公美化也不贬低
- **可复用**：第 09 节包含完整的评估原则与给他人复制使用的 prompt
- **单文件 HTML**：所有数据与样式都内嵌，无外部依赖
- **移动端兼容**：响应式布局，支持手机、平板、桌面

## 画像章节

| 章节 | 内容 |
|---|---|
| 01 · Overview | 核心数据：488 / 55 / 402h / 681 / 1041 |
| 02 · Timeline | 八年起伏：年度柱状图 + 月度热力图 + 心路五段 |
| 03 · Drift | 口味的漂移：9 张年度卡片 |
| 04 · Rhythm | 偏好节律：分类、作者、24h 阅读时段 |
| 05 · Fragments | 思想切片：从 681 条笔记中精选 12 段 |
| 06 · Shelf | 书架上的灯塔：6 本置顶 + 笔记最深的 12 本 |
| 07 · Reading between the lines | 关于他的 6 个观察 |
| 08 · Coda | 过去 · 现在 · 之后 |
| 09 · Method | 评估方法与可复用 prompt |

## 为自己生成一份

1. 安装 [weread-skills](https://weread.qq.com/r/weread-skills)（微信读书官方 AI Skill）
2. 配置环境变量：`export WEREAD_API_KEY=wrk-xxxxxxxx`
3. 打开 [index.html](./index.html) 的第 09 节，复制完整 prompt
4. 粘贴到 Claude Code 或其他能调用 weread-skills 的 AI 助手

完整原则与 prompt 见画像第 09 节。

## 评估原则（节选）

1. **数据先于解读** — 每一句判断都要能指向具体数据点
2. **不和外部基准比** — 读书是私人的事，不是竞技
3. **区分三层** — 加书架 / 读完 / 留下笔记，三者落差本身就是画像
4. **看节奏的变化** — 哪一年最密、哪一年沉默、何时开始私密化
5. **不无病呻吟** — 允许诗意，但煽情必须从数据长出来
6. **第三人称** — 用「他」/「她」，不用「你」
7. **承认盲区** — 诚实标注数据看不到的部分

完整 10 条原则见画像第 09 节。

## 文件结构

```
weread-mirror/
├── index.html       # 画像本体（单文件，含所有数据/CSS/JS）
├── README.md        # 本文件
└── .gitignore       # 排除原始私有数据
```

注：原始的微信读书 JSON 数据（书架、笔记原文等）属于私人内容，**未推送到本仓库**。本仓库只包含已聚合到 HTML 中的画像内容。

## License

代码部分 MIT。画像内容是个人作品，仅供阅读参考。

---

*Portrait by Claude · a third-party AI evaluator*
