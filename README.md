# 汽车产业链年报 AI 披露识别 · 开题答辩网页

单文件演示网页，共 15 页，固定 16:9 版式。

- 全部样式、脚本、6 张图表（base64）都已内嵌在 `index.html` 中
- 无外部依赖、无需构建、无需联网，双击即可离线播放
- 访问方式：鼠标滚轮 / 方向键 / 右下角上下按钮翻页；第 7 页（macro-F1）有「上一步 / 下一步 / 自动演示」交互

## 文件说明

| 文件 | 作用 |
| --- | --- |
| `index.html` | 网页本体，唯一必需文件（约 816 KB） |
| `.nojekyll` | 空文件，告诉 GitHub Pages 不要用 Jekyll 处理，避免静态资源被拦截 |
| `README.md` | 本说明，可保留也可删除，不影响访问 |

请保持 `index.html` 文件名不变，GitHub Pages 会自动把它作为首页。

## 用 GitHub Pages 上线（任选一种）

### 方式一：网页上传（最简单，不需要 Git）

1. 在 GitHub 新建仓库，**Visibility 选 Public**（GitHub 免费账号的 Pages 只对公开仓库开放），不要勾选任何初始化文件。
2. 进入仓库 → `Add file` → `Upload files` → 把 `index.html` 和 `.nojekyll` 一起拖进去 → `Commit changes`。
3. 进入 `Settings` → 左侧 `Pages` → `Source` 选 `Deploy from a branch`，`Branch` 选 `main`、目录选 `/ (root)` → `Save`。
4. 等待 1–2 分钟刷新页面，顶部出现站点地址，形如：
   `https://<你的用户名>.github.io/<仓库名>/`

### 方式二：命令行

```bash
git init
git add index.html .nojekyll
git commit -m "add defense deck"
git branch -M main
git remote add origin https://github.com/<用户名>/<仓库名>.git
git push -u origin main
```

推送后同样到 `Settings → Pages` 选择 `main` 分支 `/ (root)` 即可。

### 访问地址规则

- 仓库名为 `xxx.github.io` 时：`https://xxx.github.io/`
- 其他仓库名：`https://<用户名>.github.io/<仓库名>/`
- 首次部署有 1–5 分钟延迟；改完文件重新推送后也需等一两分钟再刷新。

## 注意事项

- 文件里不含任何 API 密钥、账号或本地路径，可以公开。
- 页面是 1280×720 固定画布并按窗口等比缩放，**建议用桌面浏览器全屏展示**；手机竖屏下字会偏小。
- 若需要投屏答辩，用 Chrome / Edge 按 `F11` 全屏，比例最接近 PPT。
- 若把仓库设为 Private，Pages 需要付费账号，免费账号会 404。
