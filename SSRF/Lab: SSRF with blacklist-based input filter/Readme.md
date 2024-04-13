# Lab: SSRF with blacklist-based input filter #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/fb247514-afb2-478a-9a83-cfd7b956da18)

## Target website ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/1d90ea4b-ecaa-420a-9f63-1465101c7e68)

> We have intercepted the request

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/de08f677-f52e-4eec-b3f4-ec2602cbbb6c)

> Now we will try to modify the stockapi feild

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/15aaa181-987a-4f15-9905-19b22161725e)

> So we can see that `http://127.0.0.1/admin` is not working lets try change paylaod

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/5413a541-5ad4-4fb7-b2d4-9fdc519d0946)

> When we added the html encoding it worked and we got the admin panel.

> Now try delete users carlos in same way

