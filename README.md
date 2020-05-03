# 一、下載 anydesk

https://anydesk.com/zhs
IPC AnyDesk  

      ID: 876 250 353
      PWD: Siwei@MX2019

# 二、下載csv

a.於開始列表選擇 TablePlus
 




b.選擇ATT2000
 

c.右鍵點選 attendances > Export

 
 

d. anydesk傳送 csv 到本地端
 

 
# 三、取得所需日期的 csv

a開啟 google 試算表


b. 匯入第二步驟由 anydesk 取得的資料 .csv
 
將文字轉換成數字 日期和公式 須選否
 
 
c.只保留需要的日期 其餘刪除
如:需要時間 2020-04-01 ~ 2020-04-15
csv 時先需扣8 小時

早上是6:00～8:30.         22:00 - 00:30
午餐是11:00～13:00        03:00 - 05:00
晚餐是15:00～17:00       07:00 - 09:00

所以 2020-04-01 早上 6:00～8:30. 在 csv 中是 2020-03-31 22:00 開始

 

結束 2020-04-15 晚上 15:00～17:00 在 csv 中是 2020-04-14 09:00 結束
 
只保留此段 其餘刪除
 

e. 在將其下載成 csv
 

# 四、下載四維在 google drive 提供的 指紋機人員名單xlsx 
 


# 五、下載轉換程式
https://drive.google.com/file/d/1EonJ2zRDigW8V0aBHmPVefIW6FnWoLRq/view?usp=sharing
 

# 六、轉換報表
使用指令台進入到 report_tool  
a.	npm install  
b.	安裝nodejs  
c.	執行 node index.js report -r attendamce.csx  -l member.xlsx  
attendamce.csx 為步驟三取得csv  
member.xlsx 為步驟四取得xlse  
 
d.	查看 output 目錄取得報表  
 
