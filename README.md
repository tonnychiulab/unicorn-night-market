# Unicorn Night Market

[English](#english) · [正體中文](#正體中文) · [日本語](#日本語)

A one-file timing game set at a Taiwanese night market. A unicorn tourist orders a “rainbow set.” You serve pig blood cake, stinky tofu, and fried century egg before the courage meter runs out.

Built to the [js13kGames 2026](https://js13kgames.com/2026/games) rules: theme **Unicorns and Rainbows**, a single offline web page, zip ≤ 13,312 bytes. The 2026 submission window is closed; this repo is the playable game.

## English

### Play

Open `index.html` in a browser. No install, no network, no extra assets.

| Action | Control |
| --- | --- |
| Start, serve, play again | Space, Enter, click, or tap |
| Hit the green zone | Release the serve while the marker is inside it |

Each order is one snack. The marker sweeps back and forth. Serve inside the green zone to succeed.

| Snack | Too early | On time | Too late |
| --- | --- | --- | --- |
| Pig blood cake (豬血糕) | Too raw | Just right | Burnt |
| Stinky tofu (臭豆腐) | Too mild | Just right | Too funky |
| Fried century egg (炸皮蛋) | Oil not ready | Intact | Egg cracks |

A good serve adds 15 rainbow courage and 100 points. Too raw or too mild costs 10 courage. Anything harsher, including a timeout, costs 25 and the unicorn spits a rainbow and steps back. At 0 courage the stall closes. Play again resets score and courage.

### Package

`unicorn-night-market.zip` contains only `index.html` and stays under the 13 KB limit. Graphics and sound are drawn and synthesized in the page. Traditional Chinese text uses fonts already on the system.

## 正體中文

台灣夜市的單檔時機遊戲。獨角獸遊客點了一份「彩虹套餐」，你要在勇氣條歸零前端出豬血糕、臭豆腐和炸皮蛋。

依 [js13kGames 2026](https://js13kgames.com/2026/games) 的規則製作：主題是 **Unicorns and Rainbows**，單一可離線網頁，zip 不超過 13,312 bytes。2026 投稿窗口已關閉，這個 repo 是可玩的成品。

### 怎麼玩

用瀏覽器打開 `index.html`。不用安裝，也不用網路。

空白鍵、Enter、點擊或觸控都可以開始、端出、再來一局。標記左右來回，在它進入綠色區間時端出。

| 小吃 | 太早 | 剛好 | 太晚 |
| --- | --- | --- | --- |
| 豬血糕 | 太生 | 成功 | 烤焦 |
| 臭豆腐 | 太清淡 | 成功 | 太臭 |
| 炸皮蛋 | 油溫不對 | 成功 | 皮蛋破了 |

成功 +15 彩虹勇氣、+100 分。太生或太清淡 −10。其餘失敗（含逾時）−25，獨角獸會噴出彩虹並退開。勇氣到 0 就收攤。再來一局會把分數和勇氣清回開局。

`unicorn-night-market.zip` 裡只有 `index.html`，低於 13KB。畫面和音效都在頁面裡產生，繁體中文用系統已安裝的字型。

## 日本語

台湾の夜市を舞台にした、ファイル1枚のタイミングゲームです。ユニコーンの観光客が「レインボーセット」を注文します。勇気ゲージが尽きる前に、豚の血餅（豬血糕）、臭豆腐、揚げピータンを出してください。

[js13kGames 2026](https://js13kgames.com/2026/games) の規則に合わせて作りました。テーマは **Unicorns and Rainbows**、オフラインで動くウェブページ1枚、zip は 13,312 バイト以下。2026年の提出期間は終了しています。このリポジトリは遊べる完成版です。

### 遊び方

ブラウザで `index.html` を開きます。インストールも通信も不要です。

スペース、Enter、クリック、タップで開始・提供・リトライができます。マーカーが左右に往復するので、緑の区間に入った瞬間に出してください。

| おやつ | 早すぎ | 成功 | 遅すぎ |
| --- | --- | --- | --- |
| 豬血糕（豚の血餅） | 生焼け | ちょうどよい | 焦げ |
| 臭豆腐 | 薄味 | ちょうどよい | 臭すぎ |
| 炸皮蛋（揚げピータン） | 油の温度が足りない | 殻が無事 | 皮蛋が割れた |

成功するとレインボー勇気 +15、得点 +100。生焼けか薄味は −10。それ以外の失敗（時間切れを含む）は −25 で、ユニコーンが虹を吐いて後退します。勇気が 0 になると閉店です。リトライで得点と勇気は最初の値に戻ります。

`unicorn-night-market.zip` の中身は `index.html` だけで、13KB 未満です。絵と音はページ内で生成し、繁体字は端末に入っているフォントで表示します。
