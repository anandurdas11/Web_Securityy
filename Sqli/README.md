## Lab SQL injection vulnerability in WHERE clause allowing retrieval of hidden data ##


![Screenshot 2024-01-31 222335](https://github.com/anandurdas11/Web_Securityy/assets/83402050/31973451-40a4-45fe-a690-3d5a9f23d353)


We have to retrieve the data that is not listed in the given categories.

So the target website is below

![Screenshot 2024-01-31 223046](https://github.com/anandurdas11/Web_Securityy/assets/83402050/85e76a3d-bfe1-4f4d-a84d-ff65d19f5d6d)


> So when we click on the gifts we get following url `https://0a3600cb041d07798750061000ff00cf.web-security-academy.net/filter?category=Gifts`
> So we try **_sqlinjection_** on this url.

![Screenshot 2024-01-31 225115](https://github.com/anandurdas11/Web_Securityy/assets/83402050/010bc7f8-1dc8-4fc7-be94-380a387e72e7)


Let's try check sqli possible or not add `'` to the url let see the result.

![Screenshot 2024-01-31 225224](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e682bdd7-a7f6-4180-b4bc-bedd24e99854)


> So it's giving and internal server error so the query is being executed when we add `'` and it's causing error. So we can try perform sql injection.

![Screenshot 2024-01-31 230224](https://github.com/anandurdas11/Web_Securityy/assets/83402050/333b9f8a-9ece-4e5f-9b7c-89901606a6a5)


> So we modified the url and added `+OR+1=1--` `+` used for appending the characters and `--` for commenting the rest of the query.

![Screenshot 2024-01-31 230341](https://github.com/anandurdas11/Web_Securityy/assets/83402050/55e7c84b-08cd-4094-a95c-3d4e3a50b4e2)


> Get the unknown info !!!!
