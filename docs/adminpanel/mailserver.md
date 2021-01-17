---
id: mailserver
title: Mail Server Configuration
---

## Why I need it
 
You will need to have SMTP ( way to send mail ) because the system will use it to send password reset email

### SMTP from shared hosting

This is probably the easiest way to obtain SMTP data. Create an email in your host and get note of the credentials. You will need them in the install process.

![alt-text](assets/img/mailserver/1.png)

![alt-text](assets/img/mailserver/2.png)

Here are some examples how it may look

```
MAIL_DRIVER=smtp
MAIL_HOST=smtp.hostinger.com
MAIL_PORT=587
MAIL_USERNAME=foodrecipe@royhayek.com
MAIL_PASSWORD=*********
MAIL_ENCRYPTION=ssl

MAIL_FROM_ADDRESS=foodrecipes@royhayek.com
MAIL_FROM_NAME="${APP_NAME}"
```

You can test your SMTP [here](https://www.smtper.net/)

And if still doesn't work contact your host support and they will provide you the mail server credentials

```
MAIL_DRIVER=
MAIL_HOST=
MAIL_PORT=
MAIL_USERNAME=
MAIL_PASSWORD=
MAIL_ENCRYPTION=
MAIL_FROM_ADDRESS=
MAIL_FROM_NAME=
```
