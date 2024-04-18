# Lab: Reflected XSS into a JavaScript string with angle brackets HTML encoded #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/af3c109c-9da6-496e-b311-908d760258d5)

> Submit a random alphanumeric string in the search box, then use Burp Suite to intercept the search request and send it to Burp Repeater.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/8a03243d-7e5f-49ea-b741-0f891f25039a)

> Observe that the random string has been reflected inside a JavaScript string.
  Replace your input with the following payload to break out of the JavaScript string and inject an alert: `'-alert(1)-'`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e2bb1174-1dc3-4eac-abf4-83c18cc0bcf3)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/c163bf1c-588a-4107-97ba-972b28e8e66c)

> We got a alert message

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/a4e6100c-b026-4f3f-850d-cd72eb864399)
