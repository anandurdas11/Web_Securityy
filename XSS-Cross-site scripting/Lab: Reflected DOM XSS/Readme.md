# Lab: Reflected DOM XSS #

## Lab Description ## 

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/edae390a-a161-4b7e-bfdf-8ddbb63f484b)

 > In the target website and use the search bar to search for a random test string, such as "hsdfhiu".

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/44696f92-1c1e-44ec-bb34-1df81e2d5d7a)

> We have intercepted the request

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/d52abfcb-177b-4685-820f-5f026f95133b)

> On the Intercept tab, notice that the string is reflected in a JSON response called search-results.

> Lets try this payload `\"-alert(1)}//`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/232dad17-0d20-462c-8b55-9608198eb23f)

> We got a alert message

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/60e2440d-fcea-4148-9051-d3031b3ee6fd)
