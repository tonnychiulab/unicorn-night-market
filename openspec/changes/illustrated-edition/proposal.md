# Proposal

## Why

13KB 手續繪版已經能玩，但夜市和獨角獸都是幾何圖形。繪圖版要用兩份確認免費、授權清楚的素材，讓攤位和客人看得出形狀，同時不把這些檔塞進 13KB 包，也不把韓國小吃冒充成豬血糕、臭豆腐或炸皮蛋。

## What Changes

- 保留 `index.html` 的 13KB 手續繪版：不載入外部圖片或音檔，zip 仍須 ≤ 13,312 bytes。
- 另做繪圖版頁面。攤位場景只用 [Seoul Market 迷你包](https://glowcompany.itch.io/seoul-market-mini)。客人只用 [Poney sprite](https://opengameart.org/content/poney-sprite) 的兩張 CC0 彩虹小馬。
- 三種小吃的品名、判定和文案維持不變。迷你包裡的辣炒年糕、魚板串、糖餅只當攤位陳設，不得當作這三道菜。
- Seoul Market 檔案不得提交進公開 repo。CC0 小馬可以放進 repo。

## Capabilities

### New Capabilities

- `edition-split`: 13KB 版與繪圖版的界線。哪個建置可以載入外部素材，哪個必須維持程式繪圖。
- `market-dressing`: 繪圖版如何使用 Seoul Market 迷你包的圖示、地面、攤棚與音效。
- `pony-patron`: 繪圖版用 CC0 彩虹小馬代替程式畫的獨角獸，並保留兩幀。

### Modified Capabilities

- 無。主規格尚未歸檔；13KB 版的既有行為不改。

## Impact

- 新增繪圖版頁面與一份本機素材目錄。公開的 `index.html` 與 `unicorn-night-market.zip` 維持現狀。
- 授權：Seoul Market 迷你包可商用、不限專案、不必署名，不可把素材包本身再散佈。Poney sprite 為 CC0（作者 jrlapatate），不必署名。
- 假設：完整 Seoul Market 包不在這次範圍，因為頁面未確認免費。
