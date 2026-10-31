# 音樂學習需求評估問卷

學生填完問卷後，答案會透過 Formspree 寄到老師的 Email。

## 檔案說明

| 檔案 | 用途 | 你常會改嗎 |
|---|---|---|
| `src/questions.js` | 所有題目選項 | ✅ 想改選項就改這裡 |
| `src/config.js` | Formspree 收件網址 | 換收件服務時才改 |
| `src/index.css` | 網站配色與字體 | 想換顏色時改 |
| `src/App.jsx` | 問卷畫面與流程 | 改題目文字時才需要 |

## 在自己電腦上執行

```bash
npm install     # 第一次才需要，安裝套件
npm run dev     # 開啟本機預覽，網址會顯示在終端機
```

## 部署到 Vercel

1. 在 GitHub 建立一個新的 repository（例如 `music-questionnaire`）。
2. 在這個資料夾裡執行：
   ```bash
   git init
   git add .
   git commit -m "音樂問卷第一版"
   git branch -M main
   git remote add origin https://github.com/你的帳號/music-questionnaire.git
   git push -u origin main
   ```
3. 到 Vercel 按「Add New → Project」，選這個 repository，框架會自動偵測為 Vite，直接按 Deploy。
4. 完成後會得到一個網址，把它給學生就可以了。之後每次 `git push`，Vercel 都會自動更新網站。

## 送出前要先做的事

第一次正式使用前，自己先填一份，確認 Formspree 有寄 Email 給你。
Formspree 第一次收到資料時，可能會要求你到信箱點確認。
