# Surge 图标订阅说明

## 订阅地址

```text
https://raw.githubusercontent.com/CHNragdoll/images-for-surge/main/icons.json
```

## 关键规则（已验证）

Surge 对图标图片 URL 缓存很强。  
只替换同名图片（例如一直用 `Shopify.png`）可能不会刷新。

要让 Surge 稳定更新图标，必须：

1. 每次更新图片都改文件名（例如 `Shopify_20260525_234703.png`）。
2. 同时修改 `icons.json` 里的对应 `url` 指向新文件名。
3. 提交并推送后，在 Surge 刷新订阅。

## 当前文件

- `icons.json`：订阅入口
- `images/Shopify_20260525_234703.png`：Shopify 图标
- `images/Apple.png`：Apple 图标
