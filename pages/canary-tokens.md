# Canary tokens

Canaries are very sensitive to impurities of dangerous gases in the air.
Therefore, for a long time the miners took them with them to the mines:
if the bird stopped singing, it meant that it became dangerous to breathe air.

A similar principle is used in the Internet. Many
companies use [user notification](https://en.wikipedia.org/wiki/Warrant_canary):
that no one is watching them, so that when receiving a court
order *to remove* this phrase. Thus, the company gives a signal to users
that the absence of surveillance is no longer guaranteed.

We are not going to hide from corporations, but from curious people.
What can we do?

## Canary tokens

You may have seen links in the biography on the VK page that
lead nowhere (or lead to the application "Find out who is spying on you" or
something like that). This is the simplest form of a canary.

There is a wonderful online service - [Canary Tokens](https://canarytokens.org/generate), which allows you to create your own canaries.

It allows you to create various kinds of canaries that we can use to detect curious employees of your organization or detect the compromise of your systems even before an attacker can perform some destructive actions.

<img width="550" alt="Disabling autofill in the search bar" src="../img/canary_token_flow.png">

What types can be generated and under what conditions will the notification be received:
- URL token. When clicking on the link.
- DNS token. When the domain name is resolved.
- AWS keys. When using an AWS key.
-  Microsoft Word/Excel Document. When opening the file.
-  Kubeconfing. When using Kubeconfig.
-  WireGuard VPN. When using the config.
-  Cloned Website. When cloning a website.
-  MySQL Dump. When loading a MySQL dump.
-  Windows Folder. When trying to open a folder.
-  Fast Redirect. When trying to visit the site, followed by redirection.
-  Slow Redirect. When trying to visit the site, followed by a slow redirect, to get more information.
-  Custom Image Web Bug. When viewing your picture.
-  Acrobat Reader PDF Document. When opening a PDF document in Adobe Reader.
-  Custom exe / binary. When running executable files.
-  SQL Server. When loading the SQL Server database.
-  SVN. When opening the SVN folder.
-  Unique email address. When sending mail to an email address.

Example of an email notification:

<img width="550" alt="Example of canary token report" src="../img/canary_token_example.png">

*The section will be updated*

## Difference from phishing and logger links

*The section will be updated*

---

[⬅️ Back](./breach-detection.md) | [⏫ Table of contents](../README.md) | [➡️ Next](./making-breaches-useless.md)