# Spec Delta

## Purpose

用獨角獸遊客與霓虹彩虹，把 js13kGames 2026 的 Unicorns and Rainbows 主題接到台灣夜市：客人要的是彩虹套餐，吃到的是暗黑小吃。

## ADDED Requirements

### Requirement: Unicorn patron is visible
對局進行時，系統 SHALL 顯示一隻獨角獸顧客。獨角獸 MUST 以程式繪製呈現，不依賴外部圖片。

#### Scenario: Round shows the patron
- **WHEN** 一局開始
- **THEN** 畫面上看得到獨角獸顧客

### Requirement: Rainbow courage reacts to the serve
系統 SHALL 維護一條彩虹勇氣。成功的暗黑小吃 MUST 提升勇氣。太清淡 MUST 降低勇氣。太重口、烤焦、破裂或逾時 MUST 以更大幅度降低勇氣，並播放客人噴出彩虹逃走或退開的表現。

#### Scenario: Successful dark snack
- **WHEN** 這一客成功
- **THEN** 彩虹勇氣上升，獨角獸留在攤位

#### Scenario: Too mild
- **WHEN** 這一客因太生或太清淡失敗
- **THEN** 彩虹勇氣下降，表現為無聊或失望

#### Scenario: Too intense
- **WHEN** 這一客因太臭、烤焦、油溫不對、皮蛋破裂或逾時失敗
- **THEN** 彩虹勇氣下降得比太清淡更多，並出現彩虹噴出或退開

### Requirement: Night market reads as Taiwan at night
畫面 SHALL 呈現夜晚台灣夜市攤販：暖色燈、蒸氣或油煙，以及可辨認的小吃，而不是歐美市集或一般餐廳。文案 MUST 使用繁體中文。

#### Scenario: First screen
- **WHEN** 玩家看到標題或對局畫面
- **THEN** 能從燈光、攤販與繁體中文看出這是台灣夜市，而不是一般餐廳
