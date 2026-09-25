# Tasks

## 1. 界線

- [ ] 1.1 確認 `index.html` 與 `unicorn-night-market.zip` 沒有引用 `assets/`。重新打包 zip，確認仍 ≤ 13,312 bytes 且不含 PNG、WAV。
- [ ] 1.2 新增 `illustrated.html`，玩法與 `index.html` 相同，並在標題註明這是繪圖版。打開它時不影響 13KB 頁。

## 2. 小馬

- [ ] 2.1 放入 `assets/pony/poney_1.png` 與 `poney_2.png`，並寫 `assets/pony/CREDITS.txt`，含 https://opengameart.org/content/poney-sprite 與 CC0。檔案可被 git 追蹤。
- [ ] 2.2 繪圖版對局顯示小馬並約每 0.35 秒換幀。太重口或逾時時小馬右移並出現彩虹粒子。對照 `pony-patron` 的場景。

## 3. 夜市陳設

- [ ] 3.1 把 `assets/seoul-market/` 加入 `.gitignore`。目錄不存在時，`illustrated.html` 顯示 https://glowcompany.itch.io/seoul-market-mini ，且沒有破圖圖示。
- [ ] 3.2 本機放入迷你包後，畫出濕地面、橘色攤棚、餐車，以及至少一種食物陳設。訂單文字仍是豬血糕、臭豆腐、炸皮蛋，且不把迷你包食物標成這三道菜。
- [ ] 3.3 成功時可播迷你包確認聲；失敗不加分。確認 13KB 版完全不播這些音效。
