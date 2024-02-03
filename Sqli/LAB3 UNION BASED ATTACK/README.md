## Lab: SQL injection UNION attack, determining the number of columns returned by the query ##

### Lab Description ###

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/65ff6e5f-939a-4220-8d1b-3db55b1d6420)

So the target website is shown below 

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/4a92a703-e7f8-4932-8e4c-7f5c1580d475)

> So we have to determine the number of columns returned by the query by performing a SQL injection UNION attack that returns an additional row containing null values.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/29fddeee-4554-4656-8d1c-3f7cf219553e)

> So this actually the url that it shows while viewing the gift category let's try to modify the url by adding `'`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/f6d90c6e-7ca8-43ad-ba40-7e2864e6df27)

> So we are getting internal server error. So this site might be vulnerable.

We will try to perform union attack give feild below.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/af4ddb7e-7d4c-4e44-859a-f93c16c17d78)

> So keeping the Gifts constant we will add `UNION` query into send the request.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e020360b-8c08-4644-a6a3-247a9ee09a70)

> So in the above image the query is `UNION SELECT NULL--` unfortunately it returns error so it means there are more than 1 column so we keep on adding the `NULL` until the attack is sucessful.

 ![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/8a827a91-ca0a-407f-811e-ace73e141e60)

> So we can see after adding 3 NULL values to the payload we were able manage to execute the query sucessfully which means there are 3 columns.




