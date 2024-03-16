# Lab: SQL injection with filter bypass via XML encoding #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/3d962caf-a474-49e0-870b-be0eb00679c0)


## Target website ##


We have intercepted we try bypass xml in stock id 

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/5ddb8253-02e8-4e9e-978f-4406d824cbc2)

When replace stockid feild with 1+1 it get the same results and it get executed correctly 

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/2f2cb118-3700-49a2-a58f-84ba70779f52)

> When we use this payload `1 UNION SELECT NULL` to determine the no of columns we get error it's attack

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/99bcf8f2-488f-4a88-8451-c33b0a5b4507)

> We try encode in hexa try again

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/66274d52-22db-4c7e-a46c-cdfc08f60050)

> We got the results so it worked

> When we use payload 1 UNION SELECT NULL NULL we got 0 units which means there 2 columns

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/af347f5a-7203-49ae-a9f0-3efa8cab74da)

> when we used the payload 1 UNION SELECT username || '~' || password FROM users we got all user details

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/744baf69-cd3b-4f4b-b22a-85dfd462bada)

> admin details administrator~xjgi2jjtoj6909lmpr76

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/83282a5a-488b-47e1-a1cd-776660fd0077)
