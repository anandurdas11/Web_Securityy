# Lab: Reflected XSS into a JavaScript string with single quote and backslash escaped #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/bdd2c2d5-7b70-4cd0-bf1e-d76a53cb7002)

> Submit a random alphanumeric string in the search box, then use Burp Suite to intercept the search request and send it to Burp Repeater

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/6c0ac9f8-0354-4703-8cfa-21651b5a3bb2)

> this js file

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/c8585807-527b-4230-a3e3-89c56a325997)

> First we will try with testpayload

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/198cdff2-2000-455b-a246-86e2cb4cd546)

> It does'nt work lets try different payload `</script><script>alert(1)</script>` this payload close pervious script
  tag create new script

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/df43dc0f-a5aa-425a-9680-0b8b5d56ca8b)

> We got the alert message

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/86295501-e88a-4e05-97b7-da72acf50cc3)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/0c9f2615-3250-49fa-9fba-5c8b8b1f1627)

