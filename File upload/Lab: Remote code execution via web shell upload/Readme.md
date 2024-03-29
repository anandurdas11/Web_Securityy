# Lab: Remote code execution via web shell upload #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/5fe8c671-bbd6-49d3-9a1f-47f8fe24ba05)

## Target website ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/41b18c86-18ac-4271-980a-36a37ba18269)

> We have intercepted the file upload and get request from brupsuite

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/749aebfc-d125-43f4-9450-dfba0b9d2726)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/bddca818-35e1-4894-b219-14bdbb1f3bb2)

> Lets modify the requests to desiered content

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/11bfad4f-ae1c-4a51-997b-89b7adc2923c)

> Here we change the content of  the file to read the desired that we want to read .

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/ab242470-cb49-41a2-b0bb-6d2673aa6e43)

> We can see that the file was uploaded sucessfully lets try to execute the payload

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/4ca8244f-c6b4-453d-af3f-2653ce3c4848)

> When changed the reading file name to 1.php we where able to read the content of /etc/passwd

> But we read the content of `/home/carlos/secret` lets modify payload and send.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/901c9b66-9df7-4066-8afd-ecac08079004)

> We modified the payload and the upload was successful lets try to read the seceret.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/75125488-581d-4745-ab67-5e01d3a3389c)

> We got the secret `81wPRF2FJGNt2zKyHq5uMPBpM28e1U3b`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/5a80acb8-a003-4f3d-acda-9be66de4c2f6)

