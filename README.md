# git-yesterday-report
發送昨天的git紀錄

#### 一、拷貝出設定檔模組
<pre>
cp env.py.example env.py
</pre>
#### 二、依自己的環境，修改env.py
<pre>
#寄件者
me = "me@exampl.test"

#收件者需使用串列。
you = ['user1@exampl.test','user2@exampl.test']

#要切換的工作目錄，即是Git Source目錄
path = "/dlaravel/sites/ccc"

#郵件主機設定
mail_host = "mail.example.test"
mail_port = 25
mail_username = "admin"
mail_password = "admin"
</pre>
#### 三、您可以透過如下方式測試執行。
<pre>./main.py</pre>
或
<pre>python main.py</pre>
或python3
<pre>pyton3 main.py</pre>

#### 四、加入crontab每日00:10分執行，例如:
<pre>
10 0 * * * /usr/local/scripts/git-yesterday-report/main.py
</pre>
