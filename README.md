# Steel5Store deployment guide
This document expains (hopefully) in detail how to deploy our online shop to a dedicated server.  
**Required server extensions:**
 - Web Server (Apache suggested)
 - PHP 5.4+
 - Database (MySQLi suggested)
 
**Required PHP libraries / modules:**
 - Curl
 - ZIP
 - Zlib
- GD Library
- Mcrypt
- Mbstrings
- Xml

#### Step 1. Creating a Database
To deploy OpenCart you have to have a pre-existing dedicated MySQL database.Although it is theoretically possible to use different DBMS, most OpenCart modules only support MySQL, so this is the preferred option.  
In order to create a database using XAMPP/phpMyAdmin GUI, press the **Admin** button in XAMPP control panel under MySQL service to open your phpMyAdmin page. I hope you`ll be able to help yourself from there.
**DB Parameters**:
 - Encoding: utf8_general_ci
#### Step 2. Installing basic OpenCart
In order to install OpenCart on your server you have to upload the contents of the **upload** folder from the installer archive(ocStore-3.0.2.0.zip) to a folder that will contain all of your content(f.e. www_html if you`re using Apache). Now, go to your website and follow the instructions. Once done, remove  the **install** folder and **turn off the cache**. 
#### Step 3. Uploading the Shop
To upload your shop, just **git clone** this repo into your server`s root directory. Since you'll get a clean db, you will have to add the content for the site(categories, goods and stuff) by yourself through the admin page. 

![That`s all folks](https://a.d-cd.net/jIAAAgHt-uA-1920.jpg)
