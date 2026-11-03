# 大白飯王國 海關審查官
每 10 分鐘由 GitHub Actions 執行 `customs.py`,審查入境與外交論壇的新貼文。
- 入境:欄位完整性由程式檢查;內容由 NVIDIA NIM 判斷。通過則給「移民」身分組。
- 外交:只做初審分類並通知所有者,不自動承諾任何事。
- `state.json` 記錄已處理貼文(冪等)。機密存於 Actions secrets,不在程式碼中。
