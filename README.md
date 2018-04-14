# git-yesterday-report
發送昨天的git紀錄

一、考備出設定檔模組
<pre>
cp env.py.example env.py
</pre>
二、依自己的環境，修改env.py

三、您可以透過如下方式測試執行。
<pre>./main.py</pre>
或
<pre>python main.py</pre>
或python3
<pre>pyton3 main.py</pre>

四、加入crontab每日執行
10 0 * * * /usr/local/scripts/git-yesterday-report/main.py
