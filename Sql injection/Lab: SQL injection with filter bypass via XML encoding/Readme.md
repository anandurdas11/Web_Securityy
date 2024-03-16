![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/b83b8637-b8cb-4308-9efc-e9a60af7f7c7)# Lab: SQL injection with filter bypass via XML encoding #

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


