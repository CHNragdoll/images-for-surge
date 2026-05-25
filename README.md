# Surge 图标订阅说明

## 订阅地址

```text
https://raw.githubusercontent.com/CHNragdoll/images-for-surge/main/icons.json
```

## JSON 结构

```json
{
  "name": "CHNragdolls icons",
  "description": "Custom icon set for Surge",
  "time": "2026-05-26 00:16:20",
  "icons": [
    {
      "name": "Shopify",
      "url": "https://raw.githubusercontent.com/CHNragdoll/images-for-surge/main/images/Shopify_20260525_234703.png"
    },
    {
      "name": "Apple",
      "url": "https://raw.githubusercontent.com/CHNragdoll/images-for-surge/main/images/Apple.png"
    }
  ]
}
```

## 关键规则（已验证）

Surge 对图标图片 URL 缓存很强。  
只替换同名图片（例如一直用 `Shopify.png`）可能不会刷新。

要让 Surge 稳定更新图标，必须：

1. 每次更新图片都改文件名（例如 `Shopify_20260525_234703.png`）。
2. 同时修改 `icons.json` 里的对应 `url` 指向新文件名。
3. 提交并推送后，在 Surge 刷新订阅。

## 更新流程（固定步骤）

1. 新增或替换图片到 `images/` 目录。
2. 图片文件名改成带时间后缀（例如 `Xianyu_20260526_001620.png`）。
3. 修改 `icons.json` 里对应图标的 `url` 指向新文件名。
4. 修改 `icons.json` 的 `time` 到当前时间（精确到秒）。
5. `git add/commit/push`。
6. 在 Surge 刷新订阅。

## 常见问题

- 改了图片但 Surge 不生效：
  - 通常是缓存命中。不要只覆盖同名图片，必须换图片文件名。
- Surge 提示无效数据：
  - 检查 `icons.json` 是否是合法 JSON；
  - 顶层必须有 `icons` 数组；
  - 每个图标项必须至少有 `name` 和 `url`。

## 当前文件

- `icons.json`：订阅入口
- `images/Shopify_20260525_234703.png`：Shopify 图标
- `images/Apple.png`：Apple 图标

## 当前在线图标清单

- `Shopify`
  - `https://raw.githubusercontent.com/CHNragdoll/images-for-surge/main/images/Shopify_20260525_234703.png`
- `Apple`
  - `https://raw.githubusercontent.com/CHNragdoll/images-for-surge/main/images/Apple.png`
- `EA`
  - `https://raw.githubusercontent.com/CHNragdoll/images-for-surge/main/images/Electronic_Arts_(@EA).png`
- `Xiaohongshu`
  - `https://raw.githubusercontent.com/CHNragdoll/images-for-surge/main/images/Xiaohongshu.png`
- `Xianyu`
  - `https://raw.githubusercontent.com/CHNragdoll/images-for-surge/main/images/Xianyu_20260526_001620.png`

## 图片预览（images）

<table>
  <tr>
    <td><img src="images/Apple.png" alt="Apple" width="96"></td>
    <td><img src="images/Electronic_Arts_(@EA).png" alt="EA" width="96"></td>
    <td><img src="images/Shopify_20260525_234703.png" alt="Shopify" width="96"></td>
    <td><img src="images/Xianyu_20260526_001620.png" alt="Xianyu" width="96"></td>
    <td><img src="images/Xiaohongshu.png" alt="Xiaohongshu" width="96"></td>
  </tr>
  <tr>
    <td>Apple</td>
    <td>EA</td>
    <td>Shopify</td>
    <td>Xianyu</td>
    <td>Xiaohongshu</td>
  </tr>
</table>
