# GitHub Pages 部署指南

## 📋 部署步驟

### 1️⃣ 初始化 Git 儲存庫

在專案資料夾中開啟終端機（命令提示字元或 PowerShell），執行：

```bash
git init
git add .
git commit -m "Initial commit: 宮廟小編神器"
```

### 2️⃣ 在 GitHub 建立新儲存庫

1. 前往 [GitHub](https://github.com)
2. 點擊右上角 `+` → `New repository`
3. 填寫資訊：
   - Repository name: `templetry` (或你想要的名稱)
   - Description: `宮廟小編神器 - Temple Marketing Generator`
   - 選擇 `Public`
   - **不要**勾選 "Add a README file"
4. 點擊 `Create repository`

### 3️⃣ 連結並推送到 GitHub

複製 GitHub 顯示的指令，或執行以下指令（記得替換成你的 GitHub 帳號）：

```bash
git remote add origin https://github.com/你的帳號/templetry.git
git branch -M main
git push -u origin main
```

### 4️⃣ 啟用 GitHub Pages

1. 在 GitHub 儲存庫頁面，點擊 `Settings`
2. 左側選單找到 `Pages`
3. 在 `Source` 區域：
   - Branch: 選擇 `main`
   - Folder: 選擇 `/ (root)`
4. 點擊 `Save`

### 5️⃣ 等待部署完成

- 通常需要 1-3 分鐘
- 部署完成後，GitHub 會顯示網址：
  ```
  https://你的帳號.github.io/templetry/
  ```

## 🔄 更新網站

之後如果要更新網站內容，只需：

```bash
git add .
git commit -m "更新說明"
git push
```

GitHub Pages 會自動重新部署。

## ⚠️ 常見問題

### Q: 推送時要求輸入帳號密碼？
A: GitHub 已不支援密碼驗證，需使用 Personal Access Token：
1. GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Generate new token → 勾選 `repo` 權限
3. 複製 token，在推送時當作密碼使用

### Q: 網頁顯示 404？
A: 確認：
- GitHub Pages 是否已啟用
- Branch 是否選擇正確
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
