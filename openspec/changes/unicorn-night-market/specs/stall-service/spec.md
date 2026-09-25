# Spec Delta

## Purpose

讓玩家在台灣夜市攤位上，依訂單把豬血糕、臭豆腐或炸皮蛋做到可端出的狀態，並用可觀察的成功或失敗結束這一客。

## ADDED Requirements

### Requirement: Three dark snacks are distinct orders
系統 SHALL 提供三種可點的暗黑小吃：豬血糕、臭豆腐、炸皮蛋。每一筆訂單 MUST 只指定其中一種，並且在畫面上用台灣夜市攤販能辨認的方式標出品名。

#### Scenario: Order names a snack
- **WHEN** 新的一客開始
- **THEN** 畫面顯示豬血糕、臭豆腐、炸皮蛋三者之一，且玩家能看出現在要做哪一種

### Requirement: Pig blood cake is a heat timing serve
豬血糕訂單 SHALL 要求玩家在火候窗口內完成。過早端出 MUST 算太生，過晚 MUST 算烤焦，兩者都是這一客失敗。

#### Scenario: Serve inside the heat window
- **WHEN** 玩家在豬血糕的火候窗口內端出
- **THEN** 這一客記為成功

#### Scenario: Serve outside the heat window
- **WHEN** 玩家在火候窗口之外端出豬血糕
- **THEN** 這一客記為失敗，並指出是太生或烤焦

### Requirement: Stinky tofu is a funk dosing serve
臭豆腐訂單 SHALL 要求玩家把臭度加到可接受區間。低於區間 MUST 算太清淡，高於區間 MUST 算臭到客人受不了，兩者都是這一客失敗。

#### Scenario: Funk lands in range
- **WHEN** 玩家在臭度區間內端出臭豆腐
- **THEN** 這一客記為成功

#### Scenario: Funk misses the range
- **WHEN** 玩家在臭度區間外端出臭豆腐
- **THEN** 這一客記為失敗，並指出是太清淡或太臭

### Requirement: Fried century egg is a integrity serve
炸皮蛋訂單 SHALL 要求玩家在油溫窗口內起鍋，且蛋體保持完整。油溫不對或蛋體破裂 MUST 使這一客失敗。

#### Scenario: Fry and lift intact
- **WHEN** 玩家在油溫窗口內起鍋且蛋體未破裂
- **THEN** 這一客記為成功

#### Scenario: Oil or shell fails
- **WHEN** 玩家在油溫窗口外起鍋，或蛋體破裂
- **THEN** 這一客記為失敗，並指出是油溫不對或皮蛋破了

### Requirement: Each order has a time limit
每一客 SHALL 有可見的剩餘時間。時間歸零前玩家沒有端出 MUST 使這一客失敗。

#### Scenario: Time runs out
- **WHEN** 剩餘時間歸零且玩家尚未端出
- **THEN** 這一客記為失敗，原因是逾時
