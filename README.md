# 📂 檔案與資料夾操作

| 功能             | 指令                              

| 建立資料夾（可巢狀）     | `mkdir -p /data/input`    

| 複製所有 CSV 檔     | `cp /source/*.csv /data/input/` 

| 移動或重新命名檔案      | `mv old_data.csv backup/`  

| 刪除所有 `.tmp` 檔案 | `rm *.tmp`   

| 尋找所有 CSV 檔     | `find . -name "*.csv"` 

| 改變檔案擁有者        | `chown user:group file.txt`  

| 設定資料夾權限（執行與讀寫） | `chmod 755 my_folder` 

| 給予檔案執行權限       | `chmod +x script.sh`   

# 📄 資料處理與檢視

| 功能                    | 指令                                   

| 查看前 10 筆資料            | `head -n 10 data.csv`   

| 查看最後 10 筆資料           | `tail -n 10 data.csv`    

| 計算筆數（行數）              | `wc -l data.csv`    

| 美化顯示 JSON（需安裝 jq）     | `cat data.json \| jq '.'`  

| 搜尋 log 中包含 "error" 的行 | `grep "error" log.txt`   

| 只取第 1 與第 3 欄          | `cut -d',' -f1,3 data.csv > new.csv` 

| 第 3 欄數值大於 50 的資料      | `awk -F',' '$3 > 50' data.csv` 

# 📦 壓縮與備份

| 功能                  | 指令                                              

| 備份整個 `/data` 資料夾    | `tar -czvf backup_$(date +%Y%m%d).tar.gz /data` 

| 解壓縮 ZIP             | `unzip dataset.zip`    

| 使用 7z 壓縮（需安裝 p7zip） | `7z a archive.7z /data/*`  

# 🐍 Python 與虛擬環境

| 功能           | 指令                         

| 查看 Python 版本 | `python3 -V`     

| 執行 Python 腳本 | `python3 script.py`     

| 安裝套件         | `pip install pandas`   

| 列出已安裝套件      | `pip list`    

| 建立虛擬環境       | `python3 -m venv venv`    

| 啟用虛擬環境       | `source venv/bin/activate` 

| 停用虛擬環境       | `deactivate`    

# 🌐 遠端與同步

| 功能       | 指令                                      

| 傳送檔案到遠端  | `scp file.csv user@remote:/home/user/` 

| 備份/同步資料夾 | `rsync -avz data/ user@server:/backup/` 

# ☁️ GCP 相關

| 功能         | 指令                                     

| 登入 GCP CLI | `gcloud auth login`   

| 上傳檔案至 GCS  | `gsutil cp data.csv gs://your-bucket/` 

# 🕒 排程任務（crontab）

| 功能             | 指令                                                                   

| 編輯排程任務         | `crontab -e`                                                         

| 每天凌晨 2 點執行備份腳本 | `0 2 * * * /home/user/mongo_backup.sh >> /home/user/backup.log 2>&1` 
