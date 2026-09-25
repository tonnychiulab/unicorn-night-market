# Spec Delta

## Purpose

繪圖版的客人改用 OpenGameArt 上 CC0 的兩幀彩虹小馬，取代程式繪製的獨角獸，並在兩幀之間輪替。

## ADDED Requirements

### Requirement: Patron is the CC0 pony
繪圖版的顧客 SHALL 使用 Poney sprite（https://opengameart.org/content/poney-sprite）的 `poney_1.png` 與 `poney_2.png`。作者為 jrlapatate，授權為 CC0。繪圖版 MUST NOT 再畫幾何獨角獸當顧客。

#### Scenario: Pony is visible
- **WHEN** 玩家打開繪圖版的對局
- **THEN** 顧客是這張彩虹小馬的其中一幀，而不是圓形拼成的獨角獸

### Requirement: Two frames alternate
兩張小馬圖 SHALL 輪替播放，用來表現鬃毛與尾巴的晃動。輪替 MUST 在對局進行時持續，直到收攤。

#### Scenario: Frames change
- **WHEN** 對局進行超過一個輪替間隔
- **THEN** 顧客從一幀換成另一幀

### Requirement: Pony may live in the repo
這兩張 CC0 圖 MAY 提交進 repo。提交時 MUST 在素材說明標明來源頁與 CC0，不必強制署名。

#### Scenario: Credit file
- **WHEN** 小馬圖被放進專案
- **THEN** 同目錄或 README 有 OpenGameArt 頁面連結與 CC0

### Requirement: Reactions still read on the pony
成功、太清淡與太重口的勇氣規則 MUST 與 13KB 版相同。太重口或逾時時，繪圖版 SHALL 讓小馬退開或噴出彩虹，而不是換一隻別的角色。

#### Scenario: Intense fail moves the pony
- **WHEN** 這一客因太重口、烤焦、破裂或逾時失敗
- **THEN** 小馬退開或被彩虹蓋住，勇氣下降幅度與 13KB 版相同
