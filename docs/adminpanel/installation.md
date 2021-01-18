---
id: installation
title: Installation
---

## Requirements 

The followings are required to install the admin panel on a host:
* PHP Version: 7.4 or 8.0
* MySQL Version: >= 5.x
* Application server: Apache, Nginx
* IMPORTANT: The script can only be installed directly in domain or subdomain.

### Prepare to install

Installing the panel is very easy and you'll be able to install it without any coding knowledge. The installation process includes three major steps:
1. Creating domain or subdomain
2. Creating a database
3. Uploading script files to the host

### Installation on Shared Hosting
Plesk, cPanel, hPanel and other hosting managers are recommended. In this guide, we will use Plesk but similar should be for others.

<b>1. Create your domain or subdomain in your shared hosting</b>

After you have created that, you will be able to access the file manager for that domain/subdomain
Delete any default files that are maybe added.

<b>2. Create a database</b>

Create an empty database in your shared hosting and remember this credentials

* db name
* db username
* db user pass

as shown in the picture below:

![alt-text](assets/img/adminpanel/1.png)

<b>3. Upload the source code you have downloaded from CodeCanyon and unzip it (in the admin_panel folder)</b>

<b>4. Now navigate to the web url where your project is located </b>

ex. mydomain.com or subdomain.mydomain.com <b>(If the installation page doesn't show navigate to /install ex. mydomain.com/install or subdomain.mydomain.com/install)</b>

Click on the "Check Requirements" If some requirements is missing it will be noted out.

![alt-text](assets/img/adminpanel/2.png)

Now let's check folder permissions. If some folder is noted as not writable, please check his permission. It should be 775 or 777

![alt-text](assets/img/adminpanel/3.png)

Now we need to set up the environment. This tells Laravel how to work.

![alt-text](assets/img/adminpanel/4.png)

Select the classic text editor.

![alt-text](assets/img/adminpanel/5.png)

<b>5. Environment Configuration</b>

<blockquote>Note: This configuration requires many steps so we will explain this more detail.</blockquote>

As we already mentioned environment configuration requires many steps but just for the beginning we will need only several configurations:

* Applications Basics These are the first variables you will need to change.

```
APP_NAME=Application name goes here
APP_ENV=production
APP_URL=Your website url goes here
```

* Database Configuration Click on the article below to continue with the database configuration.

 [Database Configuration](adminpanel/databaseconfig.md)

 When you finish with this configuration don't forget to save the .env file.

![alt-text](assets/img/adminpanel/6.png)

Click on Save and install

Now the install process will begin

It will install all the necessary configurations. If some error occurs, the next screen will tell you that.

If all goes okay, you can click on "Finish".

Now you have your own instance but the configuration is not over. Now you need to continue with the other environment configuration.

You will have the option to modify and add .env values later on.


