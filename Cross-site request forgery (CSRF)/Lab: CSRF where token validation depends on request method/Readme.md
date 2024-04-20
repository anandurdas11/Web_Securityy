# Lab: CSRF where token validation depends on request method #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e3279bd4-700f-4dcd-8f63-1f4df891de6f)

> Open Burp's browser and log in to your account. Submit the "Update email" form, and find the resulting request in your Proxy history.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/a4425fe3-f2bd-4989-a3c6-a14724cb87bd)

> Use "Change request method" on the context menu to convert it into a GET request and observe that the CSRF token is no longer verified.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/13d95294-629e-4e03-8892-c01a21e80825)

> We give the payload to exploit server and send the payload to victim

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/c7a88211-5ebe-4f83-a8b7-34bea6063771)

> After sending the exploit email is changed

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/f252f993-003c-4ed0-9970-f63cf08207fa)
