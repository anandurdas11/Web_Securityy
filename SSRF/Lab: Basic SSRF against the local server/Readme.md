# Lab: Basic SSRF against the local server #

## Lab description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/932137cf-052f-40e2-bd84-2e6cb638ebc2)

## Target website ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e748c3ae-10de-4b62-b740-0c7f7ed5efab)

> We are intercepting the request while checking the stock.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e1530ce9-a408-4130-8d5c-30226bfc59ea)


> We are Forging the request in stockapi parameter.
> stockapi = `http://localhost/admin`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/50893a7b-b462-4465-bd11-43b19cad77b1)

> After that we got the admin page we have to delete the user `calaros`.

> Now we have to forge we have to forge a request to delete the user.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/8a027b71-f3ef-4b78-89ef-e936be66494f)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/fdb5878e-5f38-4e30-b955-9c6551afe692)


