### cici(測試，部屬)

## 上傳檔案
確定整包專案完成後將檔案壓縮成一包(.zip檔) -> 打開Windows PowerShell ->scp 壓縮檔路徑 傳送位置 (example : scp .\company-website-fullstack.zip jingze_system@10.13.10.5:~/)
Are you sure you want to continue connecting? YES ->上傳完成

## 使用MobaXterm連進server並mounting到Docker
點開Mobaxterm點選session -> 點選ssh -> RemoteHost:目標IP 打完按OK -> 輸入帳號密碼進入terminal並sudo su ->
ls檢查檔案室否有傳進去 -> mkdir一個新資料夾並解壓縮檔案進去(此步驟去確認檔案數量，避免解壓縮完大量檔案放在外面，確認完可略過) ->
進到project file，docker compose up -d -> 確認上傳完docker是否有正常run



