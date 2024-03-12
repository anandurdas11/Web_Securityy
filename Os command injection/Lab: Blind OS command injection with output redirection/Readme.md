# Lab: Blind OS command injection with output redirection #

# Lab Description #

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/381fdd1a-5e4c-4238-a2d1-0e55aed29118)

> So we have intercepted the request and try to manipulate to get the whoami output

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/809fbba3-183b-4584-8704-4b0b35618564)

> Here we are using the payload `|| whomai>/var/www/images/output.txt||` using this payload we are storing the output
  of the command whoami in output.txt

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/30cc6d75-7ea6-40c3-9960-91a0d59e5ec1)

> It was successful and we got the 200 ok

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/35155b21-42ab-4bd4-9fe5-d0d1ca11be1f)

> When try to read file using filename we get the following output

 ![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/1dcf733d-3405-48b1-8389-b0d50651eeb6)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/79053f79-634f-4eee-8ac6-a10a1ed3eaac)
