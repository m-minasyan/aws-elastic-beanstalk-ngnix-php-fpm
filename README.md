## Replace Apache with Nginx and PHP-FPM 7.2, turn on gzip, expires headers on AWS Beanstalk:

If you discover yourself needing to use Nginx and PHP-FPM rather than apache for your AWS stem PHP App, well it's great!
This is a sample deployment with all of the .ebextensions to try and do therefore without having to create a custom AMI.

## What's performed here:

1. Install nginx, php-fpm 7.2.
2. Stop Apache and hold it from starting up again.
3. Turn on gzip, expires headers.
4. Turn on Cloudwatch logs.

## How to use it:

You can download this repository, zip up the contents, ensuring you consist of the .ebextensions directory and set up to your AWS Elastic Beanstalk app.

## Nginx and PHPFPM config changes:

You'll locate the config files in ".ebextensions\setup\config\nginx" folder.

## Why not create a custom AMI:

You can cross this path, but then in a few months when you want to use the contemporary model of Amazon Linux you'll need to absolutely recreate your custom AMI all over again.  That receives to be a pain over the path of time. So, why now not simply stay with the default AMI and deal with all of your setups via .ebextensions?
