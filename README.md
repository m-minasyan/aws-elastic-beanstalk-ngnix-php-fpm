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

_
## Замена Apache на Nginx и PHP-FPM 7.2, включите gzip, expires headers на AWS Elastic Beanstalk:

Если вы думаете, что вам нужно использовать Nginx + PHP-FPM, а не Apache + PHP для своего приложения AWS, то это то что вам нужно.
Это пример развертывания со всеми .ebextensions, которые можно попробовать и сделать без необходимости создания пользовательского AMI.

## Что здесь делает этот скрипт:

1. Установливает nginx, php-fpm 7.2.
2. Останавливает Apache и не пускает его повторно запускаться.
3. Включите gzip, expires headers, ssl redirection.
4. Включите логи CloudWatch.

## Как эиспользовать:

Вы можете скачать этот репозиторий, разархивировать его содержимое, скопировать файлы с каталога .ebextensions в ваш и настроить конфигурации ngnix для своего приложения AWS Elastic Beanstalk.

## Изменения конфигурации Nginx и PHPFPM:

Вы найдете файлы конфигурации в папке ".ebextensions\setup\config\nginx".

## Почему бы не создать пользовательский AMI:

Вы можете сделать это, но затем, через несколько месяцев, когда вы захотите использовать новую версию Amazon Linux, вам нужно будет каждый раз обновлять ваш пользовательский AMI. Это дает вас танцы с бубном. Итак, почему бы просто не остаться с AMI от Amazon-а и работать со всеми вашими настройками через .ebextensions?
