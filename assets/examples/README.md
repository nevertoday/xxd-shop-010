# XXD Shop 010 样张

每张都是本编号按 `references/sample-workflow.md` 一次生成、目视通过的原图，像素未改，只清理了元数据。商品是虚构的演示品牌，画面上的价格、规格等数字都是演示设定。

| 文件 | 用途 | 实际像素 | 输入 | 文字方式 | visual_review |
|---|---|---|---|---|---|
| `c01-category-3x4-1086x1448.png` | 详情页模块 | 1086x1448 | 商品图 `product-mc-milk.jpg`、Logo `logo-muchuan.png` | plan zh-CN | passed |
| `c02-category-1x1-1254x1254.png` | 白底主图 | 1254x1254 | 商品图 `product-keke-chips.jpg`、Logo `logo-keke.png` | plan zh-CN | passed |
| `c03-category-1x1-1254x1254.png` | 白底主图 | 1254x1254 | 商品图 `product-mc-yogurt.jpg`、Logo `logo-muchuan.png` | plan zh-CN | passed |
| `c04-category-4x5-1122x1402.png` | 详情页模块 | 1122x1402 | 商品图 `product-xd-steak.jpg`、Logo `logo-xiandao.png` | plan zh-CN | passed |
| `c05-category-3x4-1086x1448.png` | 详情页模块 | 1086x1448 | Logo `logo-chengli.png` | plan zh-CN | passed |
| `c06-category-1x1-1254x1254.png` | 白底主图 | 1254x1254 | 商品图 `product-lc-water.jpg`、Logo `logo-lengchuan.png` | plan zh-CN | passed |
| `s01-size-1x1-1254x1254.png` | 白底主图 | 1254x1254 | 原图 `orange.jpg`、Logo `logo-chengli.png` | prompt zh-CN | passed |
| `s02-size-3x4-1086x1448.png` | 详情页模块 | 1086x1448 | 原图 `orange.jpg`、Logo `logo-chengli.png` | prompt zh-CN | passed |
| `s03-size-9x16-941x1672.png` | 竖屏 | 941x1672 | 原图 `orange.jpg`、Logo `logo-chengli.png` | prompt zh-CN | passed |
| `s04-size-16x9-1672x941.png` | 横版模块 | 1672x941 | 原图 `orange.jpg`、Logo `logo-chengli.png` | prompt zh-CN | passed |
| `s05-category-3x4-1086x1448.png` | 详情页模块 | 1086x1448 | 原图 `strawberry.jpg`、Logo `logo-chengli.png` | prompt zh-CN | passed |
| `s06-category-1x1-1254x1254.png` | 白底主图 | 1254x1254 | 商品图 `product-yfp-honey.jpg`、Logo `logo-yefengpo.png` | plan zh-CN | passed |
| `s07-category-3x4-1086x1448.png` | 详情页模块 | 1086x1448 | 商品图 `product-shanyu-coldbrew.jpg`、Logo `logo-shanyu.png` | plan zh-CN | passed |
| `s08-special-1x1-1254x1254.png` | 白底主图 | 1254x1254 | 原图 `orange.jpg`、Logo `logo-chengli.png` | prompt en-US | passed |

## 输入素材

`sources/` 里是生成时交给本编号的输入缩样，模拟商家手里的素材：带包装与 Logo 的商品图、品牌 Logo，个别为原图。
演示品牌、Logo 和商品图由本项目生成；其中以 Unsplash 照片为底的，署名如下，适用 [Unsplash License](https://unsplash.com/license)，**不属于**本仓库的 PolyForm Noncommercial 授权范围。

| 输入 | 说明 · 来源 |
|---|---|
| `sources/logo-chengli.png` | 演示品牌 Logo，本项目生成 |
| `sources/logo-keke.png` | 演示品牌 Logo，本项目生成 |
| `sources/logo-lengchuan.png` | 演示品牌 Logo，本项目生成 |
| `sources/logo-muchuan.png` | 演示品牌 Logo，本项目生成 |
| `sources/logo-shanyu.png` | 演示品牌 Logo，本项目生成 |
| `sources/logo-xiandao.png` | 演示品牌 Logo，本项目生成 |
| `sources/logo-yefengpo.png` | 演示品牌 Logo，本项目生成 |
| `sources/orange.jpg` | 原图 [vRF8YpnkSHc](https://unsplash.com/photos/vRF8YpnkSHc) · @fukayamamo |
| `sources/product-keke-chips.jpg` | 演示商品图，本项目生成 |
| `sources/product-lc-water.jpg` | 演示商品图，本项目生成 |
| `sources/product-mc-milk.jpg` | 演示商品图，本项目生成 |
| `sources/product-mc-yogurt.jpg` | 演示商品图，本项目生成 |
| `sources/product-shanyu-coldbrew.jpg` | 演示商品图，本项目生成；底图 [7moPg-okWAI](https://unsplash.com/photos/7moPg-okWAI) · @elozanov |
| `sources/product-xd-steak.jpg` | 演示商品图，本项目生成 |
| `sources/product-yfp-honey.jpg` | 演示商品图，本项目生成；底图 [0em3k8ebFCs](https://unsplash.com/photos/0em3k8ebFCs) · @jonathanpielmayer |
| `sources/strawberry.jpg` | 原图 [xnRg3xDcNnE](https://unsplash.com/photos/xnRg3xDcNnE) · @allecgomes |
