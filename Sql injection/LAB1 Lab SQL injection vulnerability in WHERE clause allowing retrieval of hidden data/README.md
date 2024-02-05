## Lab SQL injection vulnerability in WHERE clause allowing retrieval of hidden data

![Alt text](<Screenshot 2024-01-31 222335.png>)

We have to retrieve the data that is not listed in the given categories.

So the target website is below

![Alt text](<Screenshot 2024-01-31 223046.png>)

> So when we click on the gifts we get following url `https://0a3600cb041d07798750061000ff00cf.web-security-academy.net/filter?category=Gifts`
> So we try **_sqlinjection_** on this url.

![Alt text](<Screenshot 2024-01-31 225115.png>)

Let's try check sqli possible or not add `'` to the url let see the result.

![Alt text](<Screenshot 2024-01-31 225224.png>)

> So it's giving and internal server error so the query is being executed when we add `'` and it's causing error. So we can try perform sql injection.

![Alt text](<Screenshot 2024-01-31 230224.png>)

> So we modified the url and added `+OR+1=1--` `+` used for appending the characters and `--` for commenting the rest of the query.

![Alt text](<Screenshot 2024-01-31 230341.png>)

> Get the unknown info !!!!
