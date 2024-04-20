# Lab: CSRF where token validation depends on token being present #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/adc638e3-941c-476d-b598-27422a412495)

> Open Burp's browser and log in to your account. Submit the "Update email" form, and find the resulting request in your Proxy history.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/fb0ab9ea-fb5f-48a4-adb3-889bfa273b3c)

> We can see that after removing the csrf token email is updated

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/d7c1b15a-a52c-4224-81f8-abdc1b4154e4)

> We generate the payload and send to exploit server

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/9974dfac-2618-41bf-aea8-cd73128e5eb8)

> We have added in the exploit server we store and send to victim

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/48b7f156-39e9-48d9-8379-af6170d32064)

> The email will be updated

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/f3cd5a31-c77e-4237-a364-6e911dbfdc3c)
