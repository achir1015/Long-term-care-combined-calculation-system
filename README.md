# Long-term-care-combined-calculation-system 長照組合計算系統 https://achir1015.github.io/Long-term-care-combined-calculation-system/
<img width="1878" height="960" alt="image" src="https://github.com/user-attachments/assets/75217186-cfea-4085-b7cc-c5c5532ecfab" />
<img width="1882" height="791" alt="image" src="https://github.com/user-attachments/assets/9a6522f2-1b25-47b6-b501-136b5c91b8f3" />
v2.0 新增功能說明：

⚙ 管理服務項目（頁首按鈕）
開啟後進入獨立管理面板，有四個工具列按鈕：
按鈕功能＋ 新增服務項目開啟表單填寫新代碼⬇ 匯出 JSON下載目前資料備份（檔名含日期）⬆ 匯入 JSON從備份 JSON 還原或跨機器同步↺ 還原預設資料回到系統內建的原始資料

📝 新增／修改表單欄位
代碼、類別、服務名稱、單價、每月上限次數、特殊計算方式、政府全補、喘息額度、資格條件、互斥代碼、備註

💾 資料持久化設計
資料存於瀏覽器 localStorage，重整頁面不會消失。類比 Google Sheets 的邏輯：

SERVICES_DATA = 純資料表（可序列化存儲）
SERVICES = 加上計算函式的執行物件（衍生自資料表）
修改任何服務後，計算器即時同步更新
