# ITCCC 工具箱 · Tool Hub

ITCCC 工作相关 AI 编码（`#vibecoding`）产出索引站：**tool.itccc.app**

每个条目包含：描述、怎么用、界面截图、flomo 原始笔记链接。

## 数据来源

2026-03 以来 flomo `#vibecoding` / `#vibecoding/project` 标签笔记汇总（62 条：23 已上线 / 20 含截图 / 15 想法池）。

## 如何新增条目

1. 编辑 `index.html` 中的 `TOOLS` 数组，末尾加一行：

```js
{c:"web", n:"工具名", d:"2026-10", s:"live",
 desc:"一句话描述（是什么）",
 how:"怎么用（操作路径）",
 url:"https://xxx.itccc.app",
 shot:"截图文件名.jpg",
 notes:[{t:"标签", id:"flomo memo id"}]},
```

- `s` 状态：`live` 已上线 / `internal` 内部本地 / `idea` 想法 / `paused` 挂起
- `c` 分类 id 见 `CATS` 数组

2. 界面截图（1280×800，JPG q80）放 `screenshots/`，文件名与 `shot` 一致。

3. commit + push，Vercel 自动重新部署。

## 部署

GitHub → Vercel → 自定义域名 `tool.itccc.app`
