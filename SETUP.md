# 部署說明

## 快速上線步驟

1. 把這個資料夾上傳到 GitHub（新建 repo：southbound-tools）
2. 到 repo Settings → Pages → Branch: main → Save
3. 網址：https://yourusername.github.io/southbound-tools/

## Google Forms 串接（Lead Form 收資料）

### 步驟 1：建立 Google Form
前往 https://forms.google.com 新建表單，依序加入：
- 問題1：公司名稱（簡答）→ 必填
- 問題2：職稱（簡答）→ 必填
- 問題3：聯絡電話（簡答）→ 必填
- 問題4：電子郵件（簡答）
- 問題5：最想進入的市場（核取方塊）選項：馬來西亞、新加坡、泰國、越南、印尼、還不確定
- 問題6：目前最大的困難（選擇題）選項：不知道哪個產品適合出海、法規文件不知道怎麼準備、Halal認證不了解、找不到當地通路夥伴、沒有資源做市場調查

### 步驟 2：取得 Form ID 和欄位 entry ID
1. 點「預覽」表單（眼睛圖示）
2. 在瀏覽器網址列看到：https://docs.google.com/forms/d/e/[FORM_ID]/viewform
3. 複製 FORM_ID
4. 右鍵「檢視原始碼」，搜尋 entry. 找到各欄位的 entry.XXXXXXX

### 步驟 3：填入 lead-form.html
打開 lead-form.html，找到第 10 行，填入你的值：
- GOOGLE_FORM_ID：你的 Form ID
- entry.XXXX：各欄位對應的 entry ID

### 步驟 4：測試
填寫並送出，確認 Google Sheet 有收到資料即完成。

## 頁面網址
- Lead Form（QR碼用）：.../lead-form.html
- Checklist（現場展示）：.../checklist.html
- 話術 & Email（自用）：.../cta-email.html
- 首頁：.../index.html
