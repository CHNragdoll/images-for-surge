# Surge 图片库（Raw 订阅）

这个仓库提供：

- `Shopify.png`：图片文件
- `icons.json`：图片清单（可用 raw 订阅）

## 1. 发布到 GitHub

在当前目录执行：

```bash
cd "/Users/apple/Documents/PyCharm/images for surge"
git init
git add Shopify.png icons.json README.md
git commit -m "init: add Shopify image library json"
git branch -M main
git remote add origin https://github.com/<YOUR_GITHUB_USERNAME>/<YOUR_REPO>.git
git push -u origin main
```

## 2. Raw 地址

发布后可用：

- 图片 raw：
  - `https://raw.githubusercontent.com/<YOUR_GITHUB_USERNAME>/<YOUR_REPO>/main/Shopify.png`
- JSON raw：
  - `https://raw.githubusercontent.com/<YOUR_GITHUB_USERNAME>/<YOUR_REPO>/main/icons.json`

## 3. 在 Surge 里使用

### 方式 A：直接用图片 raw

在需要图片 URL 的位置填：

```text
https://raw.githubusercontent.com/<YOUR_GITHUB_USERNAME>/<YOUR_REPO>/main/Shopify.png
```

### 方式 B：订阅 JSON 清单

在需要订阅/拉取图片库清单的工具中填：

```text
https://raw.githubusercontent.com/<YOUR_GITHUB_USERNAME>/<YOUR_REPO>/main/icons.json
```

如果你要，我可以下一步直接把 `<YOUR_GITHUB_USERNAME>` 和 `<YOUR_REPO>` 替换成你的真实仓库并帮你完成本地 `git` 提交。
