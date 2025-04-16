# Linux

功能 | 指令語句 | 說明

顯示目前所在路徑 | pwd | Print Working Directory

查看目錄內容 | ls / ls -l / ls -a | 普通列出 / 詳細模式 / 包含隱藏檔案

變更目錄 | cd 路徑 | 例如 cd /home/user

回到上一層目錄 | cd .. | 

建立資料夾 | mkdir 資料夾名 | 

刪除資料夾 | rm -r 資料夾名 | 遞迴刪除

建立檔案 | touch 檔案名 | 

編輯檔案 | nano 檔案名 / vim 檔案名 | 使用編輯器編輯

查看檔案內容 | cat 檔案名 / less 檔案名 / head / tail | 一次看完 / 分頁 / 看前幾行 / 看後幾行

功能 | 指令語句 | 說明

複製檔案或資料夾 | cp 檔案A 檔案B / cp -r 資料夾A 資料夾B | -r 表示遞迴處理資料夾

移動/重新命名 | mv 原名 新名 | 可用來移動檔案或重新命名

刪除檔案 | rm 檔案名 | 小心使用！無法復原

搜尋檔案 | find /路徑 -name 檔案名 | 例如 find . -name "*.log"

搜尋內容 | grep "關鍵字" 檔案名 / grep -r "關鍵字" 資料夾名 | 搜尋文字內容

功能 | 指令語句 | 說明

查看目前使用者 | whoami | 顯示目前登入的使用者

查看登入紀錄 | last | 顯示登入歷史

查看系統資訊 | uname -a | 查看核心版本與系統類型

查看 CPU/記憶體 | top / htop / free -h | 系統效能與記憶體使用量

查看磁碟空間 | df -h | 檢查磁碟使用狀況

查看目前執行程序 | ps aux / top | 顯示所有執行中程序

關閉程序 | kill PID / kill -9 PID | 強制關閉指定程序

功能 | 指令語句 | 說明

查看 IP | ip a / ifconfig（有些系統需安裝） | 查看目前網路 IP

測試連線 | ping google.com | 測試網路是否暢通

檢查連接埠 | netstat -tulnp / ss -tuln | 查看哪些 port 被佔用

下載檔案 | wget 網址 / curl -O 網址 | 下載檔案用

sudo apt update           # 更新套件庫

sudo apt upgrade          # 升級所有套件

sudo apt install xxx      # 安裝套件

sudo apt remove xxx       # 移除套件

sudo yum install xxx      # 舊版系統

sudo dnf install xxx      # 新版系統

功能 | 指令語句
壓縮 tar | tar -czvf 檔案名.tar.gz 資料夾/
解壓 tar | tar -xzvf 檔案名.tar.gz
壓縮 zip | zip -r 檔案名.zip 資料夾/
解壓 zip | unzip 檔案名.zip
