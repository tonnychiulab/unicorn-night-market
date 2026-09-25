# Spec Delta

## Purpose

把手續繪的 13KB 競賽包和可使用免費外部素材的繪圖版分開，避免繪圖版的圖片音效被打進 zip 限制。

## ADDED Requirements

### Requirement: Contest build stays procedural
13KB 版 SHALL 繼續只用程式繪製畫面與音效。它 MUST NOT 請求或打包 Seoul Market 迷你包、Poney sprite，或其他外部圖片、字型、音檔。打包成 zip 後 MUST 仍小於或等於 13,312 bytes。

#### Scenario: Contest package has no purchased or downloaded art
- **WHEN** 只打開 13KB 版並檢查網路請求與 zip 內容
- **THEN** 沒有 Seoul Market 或 Poney 的檔案，且 zip 小於或等於 13,312 bytes

### Requirement: Illustrated edition is a separate page
繪圖版 SHALL 是另一個頁面，不取代 13KB 版。兩版的小吃判定、分數與彩虹勇氣規則 MUST 相同。

#### Scenario: Both pages exist
- **WHEN** 玩家分別打開兩版
- **THEN** 13KB 版仍是程式圖，繪圖版看得到小馬與夜市陳設，玩法規則一致
