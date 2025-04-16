#資料工程師日常常用 Linux 指令包

head -n 10 data.csv          # 查看前 10 筆資料

tail -n 10 data.csv          # 查看最後 10 筆資料

wc -l data.csv               # 計算資料筆數（行數）

cat data.json | jq '.'       # 美化顯示 JSON（需安裝 jq）

grep "error" log.txt         # 尋找 log 中出現 error 的行

mkdir -p /data/input         # 建立資料夾（可巢狀）

cp /source/*.csv /data/input/   # 複製全部 CSV 檔到目標資料夾

mv old_data.csv backup/      # 移動或重新命名

rm *.tmp                     # 刪除所有 .tmp 臨時檔案

find . -name "*.csv"         # 尋找所有 CSV 檔

tar -czvf backup_$(date +%Y%m%d).tar.gz /data  # 備份整個 /data 資料夾

unzip dataset.zip            # 解壓縮 ZIP

7z a archive.7z /data/*      # 使用 7zip 壓縮（需安裝 p7zip）

python3 -V                   # 查看 Python 版本

python3 script.py            # 執行 Python 腳本

pip install pandas           # 安裝套件

pip list                     # 列出已安裝的套件

python3 -m venv venv

source venv/bin/activate

deactivate

scp file.csv user@remote:/home/user/   # 傳檔案到遠端

rsync -avz data/ user@server:/backup/  # 備份/同步資料夾

gcloud auth login                      # 登入 GCP CLI

gsutil cp data.csv gs://your-bucket/   # 上傳到 GCS（Google Cloud Storage）

crontab -e                   # 編輯排程任務

0 2 * * * /home/user/mongo_backup.sh >> /home/user/backup.log 2>&1

chmod +x script.sh           # 給予可執行權限

chmod 755 my_folder          # 設定資料夾執行與讀寫權限

chown user:group file.txt    # 改變檔案擁有者

cut -d',' -f1,3 data.csv > new.csv    # 只取第1與第3欄

awk -F',' '$3 > 50' data.csv          # 第3欄數字大於 50 的資料

