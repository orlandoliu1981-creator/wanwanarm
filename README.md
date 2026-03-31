# 旺旺軍團動畫指揮室 v1

GitHub Pages 友好的純前端原型（HTML/CSS/JS，無外部依賴）。

## 目前內容
- `index.html`：卡通動態辦公室 / 指揮室 UI
- `data/army.json`：展示資料（之後可改接 live session / cron / alerts）

## 這版重點
- 旺旺在中央中控台
- 其他 agent 各有工位 / 座位
- 狀態用動畫與光效表示：
  - `busy`：藍色光圈 + 忙碌感
  - `working`：綠色工作狀態
  - `warn`：黃燈 / 抖動感
  - `idle`：輕微漂浮，像在待命發呆
- 右側保留任務 / 警報面板，仍可作為 operational dashboard

## 後續升級路線
1. 接 `sessions_list` / `cron` / `session_status` 產出真實 JSON
2. 把狀態 mapping 從假資料改成 live data
3. 再補角色 pose、切換動畫、更多房間元素

## 注意
目前仍是**動畫展示版**，不是 live truth source。
若畫面與真實 agent 狀態衝突，**以 live session 為準**。
