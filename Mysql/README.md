### Mysql-flask語法

## 設定Conn資訊

>def getConn() -> Any:  
    >return connector.connect(  
        >host=Sqlstuff.host,  
        >user=Sqlstuff.user,  
        >password=Sqlstuff.password,  
        >database=Sqlstuff.database  
    >)  

## 資料庫連接(新增東西上去)

def createUsers(sqlQuery) -> Any:  
    conn = getConn() //指定conn給予getConn()設定的資訊  
    cursor = conn.cursor()  //呼叫cursor要使用它了  
    cursor.execute(sqlQuery)  //cursor.execute把資料傳上去的位置  
    conn.commit()  //上傳資料  
    conn.close()  //關閉資料庫  