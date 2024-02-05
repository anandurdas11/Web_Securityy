## Lab OS command injection, simple case ##

### Lab Description ###

![Alt text](image.png)

> So we have retrieve the username using the linux command `whoami`.

![Alt text](image-1.png)

> So this target website.

![Alt text](image-2.png)

> So we are try to inject os command in this feild but it did'nt work.

![Alt text](image-3.png)

> When try to intercept the following request that is used for checking for stock we get the following output below.

![Alt text](image-4.png)

> We will try to inject os command in storeid field.

![Alt text](image-5.png)

> So we injected the `whomai` command here let's forward it see the output.

![Alt text](image-6.png)

> So we get the username!!!.