
# CrateLab - Smm Panel Script

CrateLab – SMM Panel Script is an online social media marketing tool (web application) that allows and helps you to sell your Social Media Marketing Services with an easy to use panel. You can provide quality and cheap SMM Services to your customers, they can buy all packages or services like Facebook likes, Instagram followers, Twitter followers, Youtube Viewers and many more using your the panel. You can create as many as services & packages according to your expertise, this is a completely dynamic panel. Whether it is something you need for your social media accounts or you are an SMM services reseller, you will find it all here.
## Requirements

- Domain. 
- Litespeed Hostings (Free / Cheap Hostings Doesn't support the script. )
- MariaDb
- Hosting should have ( Server - Apache/Nginx, ionCube Loader, PHP Version >= 7.3, OpenSSL PHP Extension, PDO PHP Extension, Mbstring PHP Extension, Tokenizer PHP Extension, XML PHP Extension, Mod Rewrite Enabled). 

  
## Installation

Upload the Script in public_html and extract it, Now make a database with database user. Then edit this two files in file manager

```
public_html/smm/config/!database.php
public_html/smm/config/database.php
```
On line number 59 Change it to you required details on both the files

```
'database' => 'Enter Your Database Name', 
'username' => 'Enter Your Database Username', 
'password' => 'Enter you database Password',
```
On line number 59 Change it to you required details on both the files

```
'database' => env('Enter Your Database Name', 'forge'),
'username'' => env('Enter Your Database Username'', 'forge'),
'password' => env('Enter you database Password', ''),
```
Now just go to PHP my Admin and upload the .sql file and you're done with installation
## Cron jobs and addressing times

A cron job is a Linux command used for scheduling tasks to be executed sometime in the future. This is normally used to schedule a job that is executed periodically basically to be able to send order, order status, Refill. Cron task must be configured on your hosting. Here are the cron jobs with addressing time.

`cd $HOME/public_html/smm && /opt/alt/php71/usr/bin/php artisan orders:send >/dev/null 2>&1`

 1 minute

`cd $HOME/public_html/smm && /opt/alt/php71/usr/bin/php artisan status:check >/dev/null 2>&1`

1 minute

`cd $HOME/public_html/smm && /opt/alt/php71/usr/bin/php artisan send-status-report >/dev/null 2>&1`

1 day



  
## Admin credentials

Email `CrateLab@gmail.com` 

Password `CrateLab`

  
## About this Web Application

**Client:** PHP, CSS, JavaScript

**Server:** PHP and Laravel as Framework

  
## Contact Developer

- [@CrateLab](https://t.me/CrateLab) on Telegram

  