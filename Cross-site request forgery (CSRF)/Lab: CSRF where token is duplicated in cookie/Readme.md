# Lab: CSRF where token is duplicated in cookie #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/25436ee2-c688-4d21-9303-7a48b525d670)

> Open Burp's browser and log in to your account. Submit the "Update email" form, and find the resulting request in your Proxy history.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/bcc21a82-6c11-4adf-96f8-40e6b4834cc5)

> Here we can see that crsf token and csrf key are same

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/fe90b71f-75f1-436a-bec1-d5d7eec1c5eb)

> We generate the payload with fake csrf token

> We store and deliver exploit in exploit server

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/8eb073d6-0708-47c5-88a5-6c57c95ed097)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/9653af3a-6311-442e-8a84-73f8f7c6a493)
