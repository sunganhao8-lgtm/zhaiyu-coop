# AI × BP Studio · Landing Page

独立展示页，用于小红书引流 + 招募合伙人。

## 文件结构

```
landing-for-coop/
├── landing.html          # 唯一入口页面
├── assets/
│   ├── bp-1-zhaiyu.jpeg  # 真实 BP 截图 1（品牌叙事）
│   ├── bp-2-funding.jpeg # 真实 BP 截图 2（融资方案）
│   ├── bp-3-slide.jpeg   # 真实 BP 截图 3（演示幻灯片）
│   └── qrcode-placeholder.png  # 微信二维码占位图
└── README.md
```

## 部署

### 部署到 GitHub Pages（推荐）

1. 新建 GitHub 仓 `sunganhao8-lgtm/zhaiyu-coop`（public）
2. 推送本目录所有文件
3. Settings → Pages → Source: main / root
4. 访问 `https://sunganhao8-lgtm.github.io/zhaiyu-coop/landing.html`

### 部署到 Vercel / Netlify（可选）

```bash
# 拖拽 landing-for-coop 目录到 vercel.com 即可
# 或 netlify.com drop
```

### 本地预览

```bash
cd landing-for-coop
python -m http.server 8091
# 访问 http://localhost:8091/landing.html
```

## 小红书笔记配套

发布前请准备：
1. **微信二维码** —— 替换 `assets/qrcode-placeholder.png`（建议 300×300 PNG）
2. **小红书封面图** —— 1280×800（AI 出图工具生成）
3. **笔记正文** —— 详见 README 顶层 markdown

### 推荐标题候选
1. 「我用 AI 4 小时做完了投资人愿意读完的商业计划书」
2. 「从 0 到投资人愿意读 · 一份 BP 的 AI 全流程复盘」
3. 「招合伙人 | AI + 商业计划书项目，寻找 3 位共建人」

## 设计原则

- **独立隔离**：landing 与实际 BP 项目（zhaiyu-bp）完全分离，互不关联
- **不暴露敏感数据**：截图经脱敏，文中未透露任何内部项目代号
- **品牌调性**：深色科技感 + 暖橙强调色，与"AI/创业"主题契合
- **响应式**：PC (1920px) / Mobile (375px) 均已验证

## 技术栈

- 纯 HTML + CSS + JS，单文件（landing.html）
- 字体：Inter + Noto Sans SC（Google Fonts）
- 图标：Emoji（无外部依赖）
- 动画：CSS keyframes + IntersectionObserver