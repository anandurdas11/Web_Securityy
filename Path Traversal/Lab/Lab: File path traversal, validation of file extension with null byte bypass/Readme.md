# Lab: File path traversal, validation of file extension with null byte bypass #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/db10054a-0dd1-472e-8924-bffd0a3c5497)

## Target Website ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e9bca77a-8f29-451f-a279-5c38b93845cb)

> So we intercepted the request for seeing the image.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/2f84deb4-4b71-429c-a9ec-5be60ff4c034)

> Let's try the normal payload `../../../etc/passwd`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/a2a30454-d959-4868-b098-d78af37cde85)


> So it's giving output as file not found lets try adding null value to bypass sanitication.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e68d046d-4dcd-406e-98ab-cdcf585ea5fc)

> So after adding the null character we get the content of thev /etc/passwd file

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/fef3a361-d7f6-4207-923e-ec5e0e7b0e51)
