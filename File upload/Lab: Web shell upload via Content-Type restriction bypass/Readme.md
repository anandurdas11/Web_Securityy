# Lab: Web shell upload via Content-Type restriction bypass #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/07e126dd-438e-4197-916d-09874fa1cddc)

> We have got the upload file page we upload file but it's not possible because file flitering is on

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/bf3b5ba7-3a32-412a-8642-a8c2c416d0ab)

> For that we change the content type while uploading the file

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/69bd53fa-2e8d-4c68-8e02-dd472886f721)

> Now if try to read the content we will be able to read the content.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/a0911223-ea10-435e-b708-a318a63f629b)

> So this content of /home/carlos/secret and the payload used here is `<?php echo file_get_contents('/home/carlos/secret'); ?>`.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/edfaaf5c-e467-44a8-8ff1-f8229e7f41c4)
