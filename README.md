# 資料工程師日常常用 Linux 指令包

# 查看前 10 筆資料
 
head -n 10 data.csv    

# 查看最後 10 筆資料

tail -n 10 data.csv   

# 計算資料筆數（行數）

wc -l data.csv 

# 美化顯示 JSON（需安裝 jq）

cat data.json | jq '.'  

# 尋找 log 中出現 error 的行

grep "error" log.txt      

# 建立資料夾（可巢狀）

mkdir -p /data/input 

# 複製全部 CSV 檔到目標資料夾

cp /source/*.csv /data/input/   

# 移動或重新命名

mv old_data.csv backup/  

# 刪除所有 .tmp 臨時檔案

rm *.tmp     

# 尋找所有 CSV 檔

find . -name "*.csv"   

# 備份整個 /data 資料夾

tar -czvf backup_$(date +%Y%m%d).tar.gz /data 

# 解壓縮 ZIP

unzip dataset.zip         

 # 使用 7zip 壓縮（需安裝 p7zip）

7z a archive.7z /data/*    

# 查看 Python 版本

python3 -V   

# 執行 Python 腳本

python3 script.py 

 # 安裝套件

pip install pandas      

# 列出已安裝的套件

pip list                 

python3 -m venv venv

source venv/bin/activate

deactivate

# 傳檔案到遠端

scp file.csv user@remote:/home/user/ 

# 備份/同步資料夾

rsync -avz data/ user@server:/backup/  

# 登入 GCP CLI

gcloud auth login                    

# 上傳到 GCS（Google Cloud Storage）
 
gsutil cp data.csv gs://your-bucket/）

# 編輯排程任務

crontab -e             

0 2 * * * /home/user/mongo_backup.sh >> /home/user/backup.log 2>&1

# 給予可執行權限

chmod +x script.sh    

# 設定資料夾執行與讀寫權限

chmod 755 my_folder   

# 改變檔案擁有者 

chown user:group file.txt    

# 只取第1與第3欄

cut -d',' -f1,3 data.csv > new.csv  

# 第3欄數字大於 50 的資料

awk -F',' '$3 > 50' data.csv       
