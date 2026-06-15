# obs-camera

🛠️ 第一階段：上傳網頁（只要做一次）
下載檔案：

打開該 Gist 網址。

點擊右上角的 「Raw」 按鈕。

在畫面上點右鍵 ➡️ 選擇 「另存新檔」，將檔案名稱命名為 index.html。

上傳至 GitHub：

登入你的 GitHub 帳號，建立一個新的公開儲存庫（Repository），名字可以叫做 obs-camera。

將剛剛的 index.html 上傳進去並提交（Commit）。

開啟網頁功能：

進入該儲存庫的 Settings（設定） ➡️ 左側選單找到 Pages。

在 Build and deployment 底下的 Branch，將 None 改成 main (或 master)，然後點擊 Save。

稍等 1 分鐘，重新整理網頁，上方就會出現一串專屬網址（例如：https://你的帳號.github.io/obs-camera/）。

📱 第二階段：手機端發送畫面
⚠️ 重要前提：手機和電腦必須連接到同一個 Wi-Fi 基地台（區域網路）。

用手機打開剛剛得到的 GitHub Pages 網址（例如 https://你的帳號.github.io/obs-camera/）。

網頁會跳出權限請求，請允許相機與麥克風權限。

權限允許後，你會在手機網頁畫面上看到兩個重點：

自己的畫面（預設會開啟後置主鏡頭）。

畫面下方會顯示一串 Your Peer ID: xxxxxx（這串 xxxxxx 是隨機生成的英數字，請把它記下來）。

💻 第三階段：OBS 端接收畫面
打開電腦上的 OBS Studio。

在下方「來源」視窗點擊 + 號 ➡️ 選擇 「瀏覽器」 (Browser)，並給它一個名字（例如：手機相機）。

在設定視窗中，修改以下參數：

URL（網址）：輸入你的網址，並在後面加上 ?peerId=手機顯示的ID。

範例：如果手機顯示 Your Peer ID: abc123，那網址就輸入 https://你的帳號.github.io/obs-camera/?peerId=abc123

寬度 (Width)：設定為 1920。

高度 (Height)：設定為 1080（或依你手機錄影比例調整）。

勾選下方的 「透過 OBS 控制音訊」（如果你需要手機麥克風的聲音）。

點擊 確定。
