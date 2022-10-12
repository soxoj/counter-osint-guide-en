# Canary tokens

Canaries are very sensitive to impurities of dangerous gases in the air.
Therefore, for a long time the miners took them with them to the mines:
if the bird stopped singing, it meant that it became dangerous to breathe air.

A similar principle is used in the Internet. Many
companies use [warrant canary](https://en.wikipedia.org/wiki/Warrant_canary):
a notification for users that there were no subpoenas; receiving a subpoena
lead to removing this notification. Thus, the company gives a signal to users
that the absence of surveillance is no longer guaranteed.

We are not going to hide from corporations, but from curious people.
What can we do?

## What are canary tokens

Возможно, вы видели ссылки в биографии на странице ВК, которые никуда
не ведут (либо ведут в приложение "Узнай, кто за тобой шпионит" или
вроде того). Это простейшая форма канарейки.

Существует замечательный онлайн-сервис - [Canary Tokens](https://canarytokens.org/generate), который позволяет создавать своих собственных канареек.

Он позволяет создать различного рода канарейки, которые мы можем использовать для детектирования любопытных сотрудников вашей организации или обнаружить компрометацию ваших систем еще до того как злоумышленник сможет выполнить некоторые деструктивные действия.

<img width="550" alt="Выключение автозаполнения в поисковой строке" src="../img/canary_token_flow.png">

Какие виды можно сгенерировать и при каких условиях будет получено уведомление:
-  URL-токен. При переходе по ссылке.
-  DNS-токен. При разрешение доменного имени.
-  AWS-ключи. При использовании ключа AWS.
-  Microsoft Word/Excel Document. При открытии файла.
-  Kubeconfing. При использовании Kubeconfig.
-  WireGuard VPN. При использовании конфига.
-  Cloned Website. При клонировании веб-сайта.
-  MySQL Dump. При загрузке дампа MySQL.
-  Windows Folder. При попытке открыть папку.
-  Fast Redirect. При попытке посетить сайт, с последующим перенаправлением.
-  Slow Redirect. При попытке посетить сайт, с последующим медленным перенаправлением, для получения большей информации.
-  Custom Image Web Bug. При просмотре вашей картинки.
-  Acrobat Reader PDF Document. При открытии PDF документа в Adobe Reader.
-  Custom exe / binary. При запуске исполняемых файлов.
-  SQL Server. При загрузке базы данных SQL Server.
-  SVN. При открытии папки SVN.
-  Unique email address. При отправке почты на электронный адрес.

Пример уведомления на почту:

<img width="550" alt="Example of canary token report" src="../img/canary_token_example.png">

*The section will be updated*

## Difference between canary tokens and phishing tools

*The section will be updated*

---

[Back](./breach-detection.md) | [Table of contents](../README.md) | [Next](./platforms.md)