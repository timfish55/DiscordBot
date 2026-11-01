<img width="1080" height="720" alt="triangle-pattern-image-2560x1440-1" src="https://github.com/user-attachments/assets/68442515-823c-41d7-8c29-1c113bda5b3e" />

# 開源機器人1.0.5更新內容
# 0.小更新
1. `music.py`新增Spotify平台
2. 狀態輪播最短改為` 5 `秒
3. AI 使用 Groq ，AI 錯誤訊息更詳細

# 1.每日簽到
`/checkin_setup` 設定基本點數、連續加成、加成上限和換日時區。`/checkin_reward` 和 `/checkin_reward_off` 管理「連續 N 天」的獎勵身分組，`/checkin_status` 查看。
# 2.伺服器備份
`/backup_auto` 設定自動備份的間隔與保留份數，只有管理員能用。原本的全域設定改成每個伺服器各自排程。
# 3.管理與審核
`/warn_setup` 設定警告累積幾次自動禁言、禁言多久。

## ★ 上列三項**不改參數都能看目前設定**。
# 4.持久化
 `/help` 選單、投票、開發者伺服器列表都**更新為持久化**，`/help` 選單現在改用只有自己看得到的訊息回覆，因為持久化後同一則訊息是大家共用的。投票資料存在 `data/polls.json`，重啟後可繼續投票，到時間會自動結束。新增了「結束投票」按鈕（發起人或有管理訊息權限的人可按）和 `hours` 欄位（預設 `24` 小時，最長 `168`）。
# 5.歡迎、離開系統
每個伺服器各自設定，存在 `data/settings.json`
`/welcome_status`：查看目前設定，以及可用的變數清單。
`/welcome_setup`：開關、頻道、是否在訊息外提及成員、是否顯示頭像、歡迎限定的私訊歡迎詞。
`/welcome_edit`：用表單改標題、內容（可換行）、顏色和大圖網址。
`/welcome_preview`：用你自己預覽，不會真的發送。
`/welcome_reset`：恢復預設。
內容可用 `{user}`、`{name}`、`{server}`、`{count}`、`{created}`、`{joined}`、`{date}` 等變數，也可以直接寫 <#頻道ID>。圖片目前只支援貼網址，因為 Discord 上傳檔案的連結會過期。
# 6.未來會有的新東西
<img width="20" height="20" alt="forum_30dp_ECA1DB_FILL1_wght400_GRAD0_opsz24" src="https://github.com/user-attachments/assets/3333cc77-33a5-4fa0-9980-ed7d031dfca1" />論壇（尚未開發完成）
<img width="20" height="20" alt="settings_30dp_ECA1DB_FILL1_wght400_GRAD0_opsz24" src="https://github.com/user-attachments/assets/a8f12d06-6a12-4fad-ad5a-d211b618091f" />Bot Consle（尚未開發完成）
# 7.加入我們的伺服器！
https://discord.gg/8EYwGb7f7D
# 8.Groq API Key 申請
https://console.groq.com/keys
