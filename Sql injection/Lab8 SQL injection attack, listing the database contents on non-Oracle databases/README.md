## Lab SQL injection attack, listing the database contents on non-Oracle databases ##

### Lab Description ###

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/a7f954a8-304c-4a29-9f1c-ca542ffdc8ea)

> First we have to check how many columns are present in database.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/58f4336f-61b0-4c36-85eb-ca287e8055e7)

> So we add the union with single null it gives internal server error so there are more than 1 column in the database.
  lets try adding 2 null values in the payload and see the result.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/93f489d6-9ef6-4627-b46f-e31dfbc149e1)

> So when we added 2 null values there was no error generated so we can confirm that there are 2 columns.

> Lets try to find out the tables in the database. So we used the payload `'union select table_name,NULL from information_schema.tables--` so what it does it select all the tables in the database.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/d42479aa-a670-4800-ac05-48877bd4e4c9)

> We found there table name called `users_dtzmmf` know see the content of the tables using the query `'union select column_name,NULL from information_schema.columns where table_name='users_dtzmmf'--`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/44d686b4-475a-4539-bd68-86b1baa70925)

> So we found out there is username feild and password feild we just need to view that columns to get admin account.
  `' union select password_euapwj,username_ctfksb from user_dtzmmf--`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/6aa83502-22d2-46fc-82ee-c44022634228)

> So we managed to get the admin details so our attack was sucessful.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/9f1b2913-e6f6-4cea-a8b0-0066fd68e82e)

> And we logged in sucessfully.


