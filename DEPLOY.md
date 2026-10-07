# GitHub Pages 部署指南

本專案：<https://github.com/yehwanlan/TempleEasyPdf>
網站網址：<https://yehwanlan.github.io/TempleEasyPdf/>

網站檔案放在 `docs/` 資料夾（`docs/index.html`），GitHub Pages 從這裡發佈。

## 🔄 更新網站（日常使用）

修改 `docs/index.html` 後，在專案資料夾開啟終端機執行：

```bash
git add .
git commit -m "更新說明"
git push
```

GitHub Pages 會自動重新部署，通常 1-3 分鐘後生效。

## 🆕 第一次部署（或換一個新儲存庫）

### 1️⃣ 在 GitHub 建立新儲存庫

1. 前往 [GitHub](https://github.com)
2. 點擊右上角 `+` → `New repository`
3. 填寫資訊：
   - Repository name: `TempleEasyPdf` (或你想要的名稱)
   - Description: `宮廟小編神器 - Temple Marketing Generator`
   - 選擇 `Public`
   - **不要**勾選 "Add a README file"
4. 點擊 `Create repository`

### 2️⃣ 推送程式碼

```bash
git remote add origin https://github.com/yehwanlan/TempleEasyPdf.git
git branch -M main
git push -u origin main
```

### 3️⃣ 啟用 GitHub Pages

1. 在 GitHub 儲存庫頁面，點擊 `Settings`
2. 左側選單找到 `Pages`
3. 在 `Source` 區域：
   - Branch: 選擇 `main`
   - Folder: 選擇 `/docs`
4. 點擊 `Save`

### 4️⃣ 等待部署完成

- 通常需要 1-3 分鐘
- 部署完成後，GitHub 會顯示網址：
  ```
  https://yehwanlan.github.io/TempleEasyPdf/
  ```

## ⚠️ 常見問題

### Q: 推送時要求輸入帳號密碼？
A: GitHub 已不支援密碼驗證，需使用 Personal Access Token：
1. GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Generate new token → 勾選 `repo` 權限
3. 複製 token，在推送時當作密碼使用

### Q: 網頁顯示 404？
A: 確認：
- GitHub Pages 是否已啟用
- Folder 是否選擇 `/docs`（不是 `/ (root)`）
- 等待 3-5 分鐘讓部署完成

### Q: 想使用自訂網域？
A: 在 GitHub Pages 設定中的 `Custom domain` 填入你的網域，並設定 DNS CNAME 記錄。

## 📱 分享你的網站

部署完成後，你可以：
- 分享網址給宮廟使用
- 在社群媒體宣傳
- 加入到你的個人網站

---

需要協助？歡迎在 GitHub Issues 提問！
