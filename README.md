# Word And Excel Search - 文件搜尋工具

這是一個跨平台的文件搜尋工具，支援搜尋 Word 和 Excel 文件中的內容。

## 功能特點

- 支援 .docx、.doc、.xlsx、.xls 檔案格式
- 可同時搜尋多個關鍵字
- 支援區分大小寫搜尋
- 即時顯示搜尋進度
- 支援 Windows 和 macOS 系統

## 系統需求

- Node.js 14.0.0 或更高版本
- npm 或 yarn 套件管理器

## 安裝步驟

1. clone此專案到本地：
```bash
git clone https://github.com/TJJAom/WordAndExcelSearch.git
cd document-search
```

2. 安裝依賴套件：
```bash
npm install
# 或使用 yarn
yarn install
```

3. 執行應用程式：
```bash
npm start
# 或使用 yarn
yarn start
```

## 開發執行

如果您想要進行開發或修改，可以使用以下指令：

```bash
# 執行開發模式
npm run start
# 或
yarn start
```

## 打包應用程式

若要建立獨立的應用程式檔案：

```bash
# 對當前平台進行打包
npm run build
# 或
yarn build
```

## 使用說明

1. 啟動應用程式
2. 點擊「選擇資料夾」按鈕選擇要搜尋的目錄
3. 在搜尋關鍵字欄位中輸入要搜尋的字詞（多個關鍵字請用逗號分隔）
4. 選擇是否要區分大小寫
5. 選擇要搜尋的檔案類型（Word 和/或 Excel）
6. 點擊「開始搜尋」按鈕
7. 等待搜尋完成，結果會顯示在下方

## 注意事項

- 在 macOS 系統上首次執行時，可能會出現安全性警告，請在「系統偏好設定」→「安全性與隱私權」中允許應用程式執行
- 搜尋大量檔案時可能需要較長時間，請耐心等待
- 建議不要同時搜尋太多檔案，以免影響效能

## 常見問題

Q: 為什麼我的 Mac 無法開啟應用程式？
A: 這是因為 macOS 的安全性設定，請在「系統偏好設定」→「安全性與隱私權」中允許應用程式執行。

Q: 搜尋速度很慢怎麼辦？
A: 搜尋速度主要取決於檔案數量和大小，建議：
- 縮小搜尋範圍
- 減少同時搜尋的關鍵字數量
- 選擇特定的檔案類型進行搜尋

## 錯誤處理
```bash
# 進入專案目錄
cd D:\myWorkSpace\excelSearch

# 停止所有可能的 node 進程
taskkill /F /IM node.exe

# 刪除 node_modules 資料夾（使用系統命令）
if (Test-Path -Path "node_modules") { Remove-Item -Path "node_modules" -Recurse -Force }

# 刪除 package-lock.json（如果存在）
if (Test-Path -Path "package-lock.json") { Remove-Item -Path "package-lock.json" -Force }

# 清除 npm 快取
npm cache clean --force

# 重新安裝套件
npm install electron electron-builder --save-dev
```

## 作者

Tom.Tang
