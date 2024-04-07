# Lab: Web shell upload via path traversal #

## Lab description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/f69fa024-9753-4c16-92e7-401dc68d4551)

### Target website ###

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/dd9cfa26-f091-4f5f-a068-ee17ca890872)

> So this the file upload page of the website we upload file here.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/018e69a7-0830-4184-8cff-bea098782aff)

> We uplaod the payload exploit.php content is `<?php echo file_get_contents('/home/carlos/secret'); ?>`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/6520f6ff-9277-483f-878b-f574f1585f4a)

> We can see that file was uploaded sucessfully.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/f3e79e0b-fb1e-4b3e-a032-fe951c5f4355)

> We have intercepted the request and try directory travesal.

> We have changed the post request and try get content of the secret

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/87490f68-b3c5-460d-bd6d-fac0afeab47c)

> So we go to get request fo getting the content we can see the content

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/d1d5546c-3f5f-4858-bfed-1ed916868d5a)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/7eb90afe-10d9-4835-b8a0-d226ed742f81)


