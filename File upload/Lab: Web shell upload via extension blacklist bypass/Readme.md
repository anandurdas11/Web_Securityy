# Lab: Web shell upload via extension blacklist bypass #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e778bd7d-d764-4ee6-85bc-e3e9afb89493)

> File upload page

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/7314e403-6c81-4893-aea3-50c48f246804)

> First we will be uploading the php file

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e8b670cd-5a01-4867-8ef0-dc75e3a1c430)

> So we can upload the php file

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/ccbee88a-1b59-48c5-a3e7-4e4ff9aae66c)

> lets try with a different extension

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/0bab70b1-46de-46d5-921d-4443df4fe86d)

> But now in post request it is saying it php files are not allowed.

So we will be changing the value of the filename parameter to .htaccess.

Change the value of the Content-Type header to text/plain. ANd Replace the contents of the file (your PHP payload) with the following Apache directive:

AddType application/x-httpd-php .shell

`This maps an arbitrary extension (.shell) to the executable MIME type application/x-httpd-php. As the server uses the mod_php module, it knows how to handle this already.


![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/108c5c5d-5e7a-49f8-971f-86311f0e8152)


>After that we will upload the exploit.php and read the content 

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/437b6f2c-cc9a-4381-b476-7aa18d31b905)


![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/8384243f-d4db-454b-ab4a-5019924cd547)
