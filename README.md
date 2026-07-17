# Master 智能行事曆轉換器

一個可直接在瀏覽器執行的單一 HTML 靜態網站，可將 LINE 訊息、公文內容或截圖中的行程資訊，整理成日曆事件並匯出 ICS 檔案。

## 功能特色

- LINE 訊息行程解析
- 公文開會資訊解析
- 截圖影像 AI 解析
- 本地規則解析，不需 API 金鑰
- 可選擇使用 Gemini API 進行進階解析
- 產生與下載 ICS 行事曆檔案
- 支援手機與桌面瀏覽器
- 不需要後端伺服器或資料庫

## 線上使用

本專案為純靜態網站，可部署至 GitHub Pages、Cloudflare Pages、Netlify、Vercel，或直接下載 `index.html` 後以瀏覽器開啟。

## 使用方式

1. 下載此專案。
2. 直接開啟 `index.html`。
3. 貼上 LINE 訊息或公文內容。
4. 選擇「本地」或「AI（Gemini）」解析模式。
5. 檢查解析結果並下載 ICS 檔案。

## Gemini API 金鑰

AI 解析功能需要使用者自行申請並輸入 Gemini API 金鑰。

- 金鑰不包含於本專案原始碼中。
- 金鑰只儲存在使用者目前瀏覽器的 LocalStorage。
- 請勿在公開電腦輸入私人 API 金鑰。
- 請勿將自己的 API 金鑰寫入原始碼或提交至 GitHub。
- 純前端網站無法完全隱藏 API 金鑰；正式大量使用時，建議改用後端代理服務並加入存取限制。

## GitHub Pages 部署

1. 建立新的 Public repository。
2. 將本專案所有檔案上傳至預設分支。
3. 前往 `Settings` → `Pages`。
4. 在 `Build and deployment` 選擇 `Deploy from a branch`。
5. 選擇 `main` 分支與 `/ (root)`。
6. 儲存後等待 GitHub Pages 產生公開網址。

## 專案結構

```text
.
├── index.html
├── README.md
└── LICENSE
```

## 技術

- HTML
- JavaScript
- Tailwind CSS CDN
- Font Awesome CDN
- Google Fonts
- Gemini API（選用）

## 隱私說明

本地解析功能在瀏覽器端執行。啟用 Gemini AI 模式時，使用者輸入的文字或圖片會傳送至 Google Gemini API 進行處理，使用者應自行確認資料內容是否適合傳送至第三方服務，避免上傳機密、公文個資或敏感資訊。

## 開源授權

本專案採用 MIT License。您可以自由使用、修改、散布與再製，但需保留原授權聲明。

## 作者

Master
