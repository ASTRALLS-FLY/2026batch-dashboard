# 莫桑耳饰 2026 批次 · 数据分析看板

单文件静态看板，展示 2026 批次产品表现与目标达成情况（多 Tab、ECharts 图表、明细表、诊断结论）。

## 目录

```
index.html                     看板主页面（入口）
vendor/echarts.min.js          ECharts 5.5.0，本地内置，无需 CDN
.github/workflows/pages.yml    GitHub Pages 自动部署
```

站点完全自包含，断网或 CDN 不可达时图表仍可正常渲染。

## 本地预览

```bash
python3 -m http.server 8000
# 打开 http://localhost:8000
```

## 部署到 GitHub Pages

1. 新建仓库并推送本目录（仓库需为 Public，Pages 才对所有人可访问）。
2. 仓库 Settings → Pages → Build and deployment → Source 选 **GitHub Actions**。
3. push 到 `main` 后 workflow 自动构建并发布，访问地址为
   `https://<用户名>.github.io/<仓库名>/`。

也可在 Actions 页手动运行 `Deploy static site to GitHub Pages`。

## 注意

看板内含 2026 批次产品表现、目标达成等经营数据。**设为公开仓库前请确认数据可以对外**，否则请用私有仓库仅作代码托管，线上访问继续使用 WorkBuddy 分享链接。
