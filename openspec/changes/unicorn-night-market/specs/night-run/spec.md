# Spec Delta

## Purpose

把一客一客的夜市服務串成一局：連續來客、累計分數、勇氣見底就收攤，並能立刻再來一局。

## ADDED Requirements

### Requirement: A run is a sequence of patrons
一局 SHALL 連續派出顧客。每一客結束後，若彩虹勇氣仍大於零，系統 MUST 派出下一客。

#### Scenario: Courage remains
- **WHEN** 這一客結束且彩虹勇氣大於零
- **THEN** 下一客出現，並帶著新的小吃訂單

### Requirement: Score increases only on success
系統 SHALL 顯示分數。只有成功端出的那一客 MUST 增加分數。失敗 MUST NOT 增加分數。

#### Scenario: Successful serve scores
- **WHEN** 這一客成功
- **THEN** 畫面上的分數變高

#### Scenario: Failed serve does not score
- **WHEN** 這一客失敗
- **THEN** 分數維持不變

### Requirement: Empty courage ends the run
彩虹勇氣降到零或以下時，系統 SHALL 結束這一局，並顯示分數與再來一局。再來一局 MUST 把分數與勇氣回復到開局狀態。

#### Scenario: Courage hits zero
- **WHEN** 彩虹勇氣降到零或以下
- **THEN** 對局停止，顯示最終分數與再來一局

#### Scenario: Restart
- **WHEN** 玩家在結束畫面選擇再來一局
- **THEN** 分數歸零、勇氣回到開局值，並開始新的一客

### Requirement: Keyboard and touch both work
系統 SHALL 接受鍵盤與指標或觸控。沒有滑鼠的裝置 MUST 仍能完成端出；沒有鍵盤的裝置 MUST 仍能完成端出。

#### Scenario: Keyboard serve
- **WHEN** 玩家只用鍵盤操作
- **THEN** 可以完成一客的端出或失敗

#### Scenario: Pointer serve
- **WHEN** 玩家只用點擊或觸控
- **THEN** 可以完成一客的端出或失敗

### Requirement: Packaged game stays within the contest size
可遊玩的成品 SHALL 是不依賴外部網路資源的網頁遊戲。打包成 zip 後的大小 MUST 小於或等於 13,312 bytes。

#### Scenario: Offline package
- **WHEN** 玩家打開打包後的遊戲且沒有外加圖片、字型或音檔請求
- **THEN** 遊戲仍可從標題進入對局

#### Scenario: Zip limit
- **WHEN** 成品被壓成 zip
- **THEN** zip 檔大小小於或等於 13,312 bytes
