### cici(測試，部屬)

## 上傳檔案
確定整包專案完成後將檔案壓縮成一包(.zip檔) -> 打開Windows PowerShell ->scp 壓縮檔路徑 傳送位置 (example : scp .\company-website-fullstack.zip jingze_system@10.13.10.5:~/)
Are you sure you want to continue connecting? YES ->上傳完成

## 使用MobaXterm連進server並mounting到Docker
點開Mobaxterm點選session -> 點選ssh -> RemoteHost:目標IP 打完按OK -> 輸入帳號密碼進入terminal並sudo su ->  
ls檢查檔案室否有傳進去 -> mkdir一個新資料夾並解壓縮檔案進去(此步驟去確認檔案數量，避免解壓縮完大量檔案放在外面，確認完可略過) ->  
進到project file，docker compose up -d -> 確認上傳完docker是否有正常run  

## docker compose 基本指令
> docker compose up -d: 將docker建置並啟動至容器(-d 為背景執行)  
> docker compose stop: 停止compose(可藉由start重啟)  
> docker compose down -v: 將所有的compose停止並移除container(-v 為連volumes也移除)  
> docker images: 查詢目前有的image  
> docker rmi "image_id": 刪除image  
> docker rm $(docker ps -a -q): 停用以及刪除所有的container
