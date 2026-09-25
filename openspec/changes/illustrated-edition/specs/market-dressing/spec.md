# Spec Delta

## Purpose

繪圖版的攤位只用 Seoul Market 免費迷你包的圖示、地磚與音效，並且不把韓國小吃說成台灣的三道暗黑菜。

## ADDED Requirements

### Requirement: Stall uses only the free mini pack
繪圖版的攤位陳設 SHALL 只使用 Seoul Market 迷你包（https://glowcompany.itch.io/seoul-market-mini）裡的這 8 個圖示與 2 張地磚：辣炒年糕、魚板串、糖餅、塑膠凳、紙杯、餐車、愛心、硬幣、濕地面、橘色攤棚。MUST NOT 為了這個畫面另買或混用其他素材包。

#### Scenario: Stall shows the mini pack
- **WHEN** 玩家打開繪圖版
- **THEN** 看得到餐車或橘色攤棚，以及迷你包裡的至少一種食物陳設

### Requirement: Korean snacks are props
迷你包裡的食物 MUST 只作為攤位陳設。訂單品名 MUST 仍是豬血糕、臭豆腐、炸皮蛋。畫面 MUST NOT 把辣炒年糕、魚板串或糖餅標成這三道菜。

#### Scenario: Order name stays Taiwanese
- **WHEN** 繪圖版開始一客
- **THEN** 訂單文字是豬血糕、臭豆腐、炸皮蛋之一，而迷你包食物沒有被標成該訂單

### Requirement: Mini-pack files stay out of the public repo
Seoul Market 檔案 MUST 放在被版本庫忽略的本機目錄。公開 repo MUST NOT 包含這些 PNG 或 WAV。缺少檔案時，繪圖版 SHALL 顯示下載頁連結，而不是破圖。

#### Scenario: Assets missing
- **WHEN** 本機沒有迷你包檔案
- **THEN** 繪圖版說明要到 Seoul Market 迷你包頁面下載，且 repo 裡沒有那些檔

### Requirement: Mini-pack audio is optional flavor
繪圖版 MAY 播放迷你包的鐵板聲、投幣聲、確認聲或獲得道具聲。這些音效 MUST NOT 取代成功與失敗的判定，也 MUST NOT 進入 13KB 版。

#### Scenario: Sound does not change the score
- **WHEN** 繪圖版播放迷你包音效且這一客失敗
- **THEN** 分數規則與 13KB 版相同，不會因為音效而加分
