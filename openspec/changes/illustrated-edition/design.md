# Design

## Context

13KB 版已在 `index.html`，規則見 `unicorn-night-market` 的規格。這次只加繪圖版。行為見 `specs/edition-split`、`specs/market-dressing`、`specs/pony-patron`。動機見 proposal.md。

## Goals / Non-Goals

**Goals:**

- 繪圖版與 13KB 版共用同一套判定、分數與勇氣數字。
- 攤位只用 Seoul Market 迷你包的 8 個圖示與 2 張地磚。
- 顧客只用 `poney_1.png` 與 `poney_2.png` 輪替。
- 缺素材時仍能看懂要去哪裡下載，不出現破圖。

**Non-Goals:**

- 不修改 13KB 版的畫法，不把外部檔打進 `unicorn-night-market.zip`。
- 不使用 Seoul Market 完整包，也不把辣炒年糕、魚板串、糖餅標成三道台灣小吃。
- 不把 Seoul Market 的 PNG 或 WAV 提交進公開 repo。

## Decisions

### 兩個頁面

`index.html` 維持 13KB 版。繪圖版用 `illustrated.html`，複製同一套狀態機與文案，只換顧客與攤位的畫法。不共用會把圖片打進競賽包的建置步驟。

不做單一頁面切換。切換容易讓 zip 打包時把素材夾進去。

### 素材目錄

- `assets/pony/poney_1.png`、`assets/pony/poney_2.png`：可提交。旁註 `assets/pony/CREDITS.txt`，寫 OpenGameArt 頁面與 CC0。
- `assets/seoul-market/`：本機放置迷你包，寫進 `.gitignore`。頁面用相對路徑載入，不用 CDN。
- 檔案不在時，`illustrated.html` 顯示迷你包下載網址，顧客位置留白或暫時用小馬（若小馬已在）。

### 小馬輪替與反應

約每 0.35 秒切換兩幀。太重口、烤焦、破裂或逾時時，把小馬往右移，並在嘴邊畫彩虹粒子（粒子仍用程式畫，因為 CC0 包沒有噴彩虹的幀）。勇氣加減與 13KB 版相同：成功 +15，太生或太清淡 −10，其餘 −25。

### 攤位拼法

濕地面鋪滿攤位下方，橘色攤棚放在櫃檯上方，餐車、凳子、紙杯與一種食物圖放在櫃上。訂單文字仍用系統字型畫在圖上。迷你包音效只在端出成功時可播確認聲，失敗不播加分音。

## Risks / Trade-offs

- [韓國陳設不像台灣夜市] → 訂單文字維持三道台灣小吃；迷你包只負責燈、棚、櫃，不改菜名。
- [公開 repo 再散佈迷你包] → 該目錄 gitignore，README 只放下載連結。
- [兩張小馬加上網頁後仍想塞進 13KB] → 明確禁止；小馬只出現在 `illustrated.html`。

## Migration Plan

先提交小馬與說明，再在本機放入迷你包。13KB 的 `index.html` 與 zip 不改。若要回到只有手續繪，不打開 `illustrated.html` 即可。

## Open Questions

無。完整 Seoul Market 包不納入，直到確認它免費。
