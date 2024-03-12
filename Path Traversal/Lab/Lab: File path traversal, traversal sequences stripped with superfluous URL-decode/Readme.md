# Lab: File path traversal, traversal sequences stripped with superfluous URL-decode #

## Lab  Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/683a1d69-3d8b-44b8-be9e-30b7d39a9a77)

## Target website ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/f5bd731b-049a-44c8-a432-1f0b6d830302)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/bcd221ea-8c01-4574-89b9-f06d9116504d)

> So in the above image we can see the request going through the burpsuite and we send it to repeater
  try modify the request and get the content of `etc/passwd` file.

Lets try the first payload `../../../etc/passwd` 

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/2611699b-f1b5-49df-bcb6-d9ba2cfb62a7)

> We are getting the output as no such file is present.

Lets try with encoded url 

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/c41e6cf0-cc25-475c-af32-14f1e9b60c7d)

> But still we can see it's not working so lets try to encode it again and see the output

So When we encode the url again the payload becomes `..%252F..%252F..%252F..%252Fetc%252Fpasswd`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/9498db44-39b2-43fd-808d-f2736b7a9673)

> And we where able to see the contents of the file.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/86e30e5b-f329-492d-bf09-00d39cc30d62)

