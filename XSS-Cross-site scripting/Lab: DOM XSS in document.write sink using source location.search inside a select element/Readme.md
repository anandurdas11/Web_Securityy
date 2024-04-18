# Lab: DOM XSS in document.write sink using source location.search inside a select element #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/2b423702-4463-4855-84e7-e1db4a359bce)
> On the product pages, notice that the dangerous JavaScript extracts a storeId parameter from the location.search source. 
  It then uses document.write to create a new option in the select element for the stock checker functionality.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/118b573f-d203-4abc-a014-049f7aef04df)

> So we can see that check.js is called

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/8745f767-82aa-4a03-b6d4-a3189960daf2)

> Add a storeId query parameter to the URL and enter a random alphanumeric string as its value. Request this modified URL.
  In the browser, notice that your random string is now listed as one of the options in the drop-down list.

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/3855b2f4-5ae6-4fc0-bb65-26f7c5d3348b)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/8e62ae64-4e62-4512-80ae-df3bb86743c5)

> Right-click and inspect the drop-down list to confirm that the value of your storeId parameter has been placed inside a select element.

 ![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/8875a1c0-579c-4b4c-960a-a866af54889f)

> Change the URL to include a suitable XSS payload inside the storeId parameter as follows:
  `"></select><img%20src=1%20onerror=alert(1)>`

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/780f3d9c-2b9a-402d-8b7f-48200286a935)

> We got the alert message

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/d108ceb4-d5f1-42c4-b4e0-dbbd977ffdf1)

 
