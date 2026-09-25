# Unicorn Night Market

[English](#english) · [正體中文](#正體中文) · [日本語](#日本語)

[![Play now](https://img.shields.io/badge/Play_now-GitHub_Pages-c4552a?style=for-the-badge&logo=github)](https://tonnychiulab.github.io/unicorn-night-market/)

A one-file timing game set at a Taiwanese night market. A unicorn tourist orders a “rainbow set.” You serve pig's blood cake, stinky tofu, and fried century egg before the courage meter runs out.

Built to the [js13kGames 2026](https://js13kgames.com/2026/games) rules: theme **Unicorns and Rainbows**, a single offline web page, zip ≤ 13,312 bytes. The 2026 submission window is closed; this repo is the playable game.

Three snacks that outsiders put on “gross” lists — and Taiwan still loves:

- **Pig's blood cake** — 2009 VirtualTourist No. 1 most unusual food. Looks scary. Tastes delicious.
- **Century egg** — CNN (via [Liberty Times](https://news.ltn.com.tw/news/world/breakingnews/512660)) called it the world’s most disgusting food. Taiwan fries it golden.
- **Stinky tofu** — Takeo Koizumi’s Alabaster meter: surströmming 8070 AU is No. 1; stinky tofu is No. 10 at 420 AU. Taiwan still queues.

## English

### Play now

[![Play now](https://img.shields.io/badge/Play_now-open_the_stall-c4552a?style=for-the-badge&logo=github)](https://tonnychiulab.github.io/unicorn-night-market/)

Open the live build on GitHub Pages: [https://tonnychiulab.github.io/unicorn-night-market/](https://tonnychiulab.github.io/unicorn-night-market/)

Or open `index.html` in a browser. The game starts in English. No install, no extra assets.

The title screen explains the keyboard before the stall opens.

| Action | Control |
| --- | --- |
| Language, title screen only | 1 English, 2 繁體中文, 3 日本語, or click EN / 繁中 / 日本語 |
| Start, serve, play again | Space, Enter, click, or tap |
| Hit the green zone | Serve while the marker is inside it |

Each order is one snack. The marker sweeps back and forth. Serve inside the green zone to succeed.

| Snack | Too early | On time | Too late |
| --- | --- | --- | --- |
| Pig's blood cake (豬血糕) | Too raw | Just right | Burnt |
| Stinky tofu (臭豆腐) | Too mild | Just right | Too funky |
| Fried century egg (炸皮蛋) | Oil not ready | Intact | Egg cracks |

A good serve adds 15 rainbow courage and 100 points. Too raw or too mild costs 10 courage. Anything harsher, including a timeout, costs 25 and the unicorn spits a rainbow and steps back. At 0 courage the stall closes. Play again resets score and courage.

### Package

`unicorn-night-market.zip` contains only `index.html` and stays under the 13 KB limit. Graphics and sound are drawn and synthesized in the page. Traditional Chinese text uses fonts already on the system.

## 正體中文

[![立即玩](https://img.shields.io/badge/%E7%AB%8B%E5%8D%B3%E7%8E%A9-GitHub_Pages-c4552a?style=for-the-badge&logo=github)](https://tonnychiulab.github.io/unicorn-night-market/)

台灣夜市的單檔時機遊戲。獨角獸遊客點了一份「彩虹套餐」，你要在勇氣條歸零前端出豬血糕、臭豆腐和炸皮蛋。

依 [js13kGames 2026](https://js13kgames.com/2026/games) 的規則製作：主題是 **Unicorns and Rainbows**，單一可離線網頁，zip 不超過 13,312 bytes。2026 投稿窗口已關閉，這個 repo 是可玩的成品。

三道小吃都上過「最怪／最噁」榜單，台灣人照樣愛：

- **豬血糕** — 2009 VirtualTourist 全球最怪食物第一名。看起來嚇人，吃起來超香。
- **皮蛋** — [自由時報轉 CNN](https://news.ltn.com.tw/news/world/breakingnews/512660) 說是全球最噁食物。台灣人炸成金黃照樣吃。
- **臭豆腐** — 小泉武夫 Alabaster：Surströmming 8070 AU 第 1，臭豆腐 420 AU 第 10。台灣夜市照樣排隊。

### 立即玩

線上版：[https://tonnychiulab.github.io/unicorn-night-market/](https://tonnychiulab.github.io/unicorn-night-market/)

也可以用瀏覽器打開 `index.html`。遊戲預設是英文。不用安裝。標題畫面會先說明鍵盤，再按空白鍵或 Enter 才開始。按 1 英文、2 繁體中文、3 日本語，或點 EN / 繁中 / 日本語。

空白鍵、Enter、點擊或觸控都可以開始、端出、再來一局。標記左右來回，在它進入綠色區間時端出。

| 小吃 | 太早 | 剛好 | 太晚 |
| --- | --- | --- | --- |
| 豬血糕 | 太生 | 成功 | 烤焦 |
| 臭豆腐 | 太清淡 | 成功 | 太臭 |
| 炸皮蛋 | 油溫不對 | 成功 | 皮蛋破了 |

成功 +15 彩虹勇氣、+100 分。太生或太清淡 −10。其餘失敗（含逾時）−25，獨角獸會噴出彩虹並退開。勇氣到 0 就收攤。再來一局會把分數和勇氣清回開局。

`unicorn-night-market.zip` 裡只有 `index.html`，低於 13KB。畫面和音效都在頁面裡產生，繁體中文用系統已安裝的字型。

## 日本語

[![今すぐ遊ぶ](https://img.shields.io/badge/%E4%BB%8A%E3%81%99%E3%81%90%E9%81%8A%E3%81%B6-GitHub_Pages-c4552a?style=for-the-badge&logo=github)](https://tonnychiulab.github.io/unicorn-night-market/)

台湾の夜市を舞台にした、ファイル1枚のタイミングゲームです。ユニコーンの観光客が「レインボーセット」を注文します。勇気ゲージが尽きる前に、豬血糕（ジューシュエガオ）、臭豆腐、揚げピータンを出してください。

[js13kGames 2026](https://js13kgames.com/2026/games) の規則に合わせて作りました。テーマは **Unicorns and Rainbows**、オフラインで動くウェブページ1枚、zip は 13,312 バイト以下。2026年の提出期間は終了しています。このリポジトリは遊べる完成版です。

どれも「変・最悪」とランクされても、台湾は愛します：

- **豬血糕（ジューシュエガオ）** — 2009 VirtualTourist で世界一変わった食べ物第1位。見た目は怖い。味はうまい。
- **ピータン** — [自由時報経由の CNN](https://news.ltn.com.tw/news/world/breakingnews/512660) が世界一まずい食べ物と報道。台湾は衣揚げ（揚げピータン）にして食べる。
- **臭豆腐** — 小泉武夫の Alabaster：シュールストレミング 8070AU が第1位、臭豆腐は 420AU で第10位。それでも行列する。

### 今すぐ遊ぶ

公開ページ：[https://tonnychiulab.github.io/unicorn-night-market/](https://tonnychiulab.github.io/unicorn-night-market/)

またはブラウザで `index.html` を開きます。初期言語は英語です。インストールも不要です。タイトル画面でキーボード操作を説明してから、Space か Enter で開始します。1 英語、2 繁體中文、3 日本語、または EN / 繁中 / 日本語 をクリックします。

スペース、Enter、クリック、タップで開始・提供・リトライができます。マーカーが左右に往復するので、緑の区間に入った瞬間に出してください。

| おやつ | 早すぎ | 成功 | 遅すぎ |
| --- | --- | --- | --- |
| 豬血糕（ジューシュエガオ） | 生焼け | ちょうどよい | 焦げ |
| 臭豆腐 | 薄味 | ちょうどよい | 臭すぎ |
| 揚げピータン | 油の温度が足りない | 殻が無事 | 皮蛋が割れた |

成功するとレインボー勇気 +15、得点 +100。生焼けか薄味は −10。それ以外の失敗（時間切れを含む）は −25 で、ユニコーンが虹を吐いて後退します。勇気が 0 になると閉店です。リトライで得点と勇気は最初の値に戻ります。

`unicorn-night-market.zip` の中身は `index.html` だけで、13KB 未満です。絵と音はページ内で生成し、繁体字は端末に入っているフォントで表示します。
