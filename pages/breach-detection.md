# Determining the source of a leak

## Finding information about yourself in Leaked Data

Many sites allow you to search for yourself in leaked information and databases by phone, mail, or even your full name. Use them with caution because, behind any online search, there may be an additional goal in data enrichment. For example, **Collecting an IP address**, linking multiple searches for the same person to **collect information about their surroundings**. 

Therefore, the preferred option is always to *search the leak files yourself*.
But this can be difficult: you must find and download the leak's file (or many files if you need an exhaustive search), understand its structure, and perform an effective search.

If you chose an easier way, then I recommend using these resources in descending order of risk:

#### Commonly known secure sites

The best-known: [Have I Been Pwned](https://haveibeenpwned.com/), it's maintained by a renowned security company and providing assurances of privacy.

Other:
- https://monitor.firefox.com/

#### Commercial alternatives

Often they give conditional free access, you can find different sites by keywords check, leak:

- https://leakcheck.io/
- https://checkleaked.cc/

#### Telegram bots

- https://t.me/PhoneLeaks_bot - search only for leaks sources

Most bots do not indicate the source from which the information was obtained. List of some resources:
[Google Spreadsheet](https://docs.google.com/spreadsheets/d/1XerMPGwaDz1FG1gBumBp6jzOgSqhWcQWgZmhxoT60WA/edit#gid=0).


#### Notifications

Some of the sites listed above also can notify you by email if there is a new leak with your data. I highly recommend using such a service if you lead an active virtual life.

## Using aliases/fake mail addresses

Gmail and other most common mail services support special characters to create aliases for your mailbox. Mail sent to an alias will come to your primary email address, but you will clearly see where it came from in the Recipient field.

For example, `soxoj@protonmail.com` is equivalent to `soxoj+gitlab@protonmail.com`:

<img width="311" alt="Снимок экрана 2022-10-03 в 22 46 42" src="https://user-images.githubusercontent.com/31013580/193665517-c06dd5d4-1c6b-468d-8a16-34db0e0689a5.png">

It's **Strictly recommended** use this feature on all sites where it is supported.
Thus:
1. In case of leaks or spam, you'll know exactly where your mail came from.
2. In case of a targeted collection of information on your email, information from several sites will be less likely to be merged into one dossier.


Naturally, leak harvesting often uses mail normalization: removing similar parts of aliases and cleaning up the excess. So we can only talk about risk mitigation, not one hundred per cent protection.

Special mention should be made of providing mailing addresses **for sending receipts** for online purchases.
```
According to paragraph 2 of Art. 1.2 of the law № 54-FZ, the receipt must be sent electronically if the buyer has provided his subscriber number or an e-mail address before the payment.
```

This is used by major Telegram bots like the Eye of God: they store all your payment information, **connected to the specified email**, to the information the bot gives out.

So, if you are not interested in the receipt, then provide a knowingly wrong mailing address pointing to the source of the leak, e.g. eyeofgod@receipt.com. Or use the aforementioned aliases, explicitly revealing where the inbox was listed.

## Использование разных имён для отслеживания

So, if you are not interested in the receipt, then provide a knowingly wrong mailing address pointing to the source of the leak, e.g. eyeofgod@receipt.com. Or use the aforementioned aliases, explicitly exposing where the email account was listed.

Websites have different approaches to the accuracy of first and last names of accounts. Some require that they coincide with passport data ([e.g., in VK](https://roem.ru/21-06-2009/126784/v-v-kontakte-mojno-smenit-imya-lish-na-nastoyashchee/)), some only check them against documents in case of financial transactions, and most do not validate at all.

You can use the tricks listed below depending on the strictness of the service rules (ToS, Terms of Service). But before using them, I strongly advise you to study what sanctions are possible if you specify an invalid name and assess these risks for yourself.

#### Use names/surnames that are consonant or begin with the same letters as the site/company.
Таким образом, при утечке ФИО в связке с номером или почтой вы будете знать, откуда эта информация:

- Макдональдс: _Максим_
- ВКонтакте: _Вова_
- Одноклассники: _Олег_

#### Используем вариации имени кириллицей или латиницей
Прежде всего это относится к полной/сокращённой форме имени:

- Александр
- Саша
- Саня
- Шура

Но в силу различий между языками, у имени бывает по несколько "латинских" форм.
Даже банки часто дают возможность выбора правильной транслитерации имён.
Так, имя "Анатолий" может быть представлено как:

- Anatoly
- Anatolii
- Anatoliy

---

<details>
  <summary>🥷 Продвинутый уровень</summary>
  </br>

### Использование BitWarden для генерации алиасов электронной почты

Парольный менеджер BitWarden позволяет генерировать случайные алиасы почты с плюсом, а также адреса catch-all почтовых ящиков и даже почтовые ящики для пересылки.

Подробнее про эти возможности читайте в разделе "🥷 Продвинутый уровень" секции [Почтовый ящик](./email.md).

![image](../img/bitwarden_en.png)

</details>

---

[⬅️ Back](./breaches.md) | [⏫ Table of contents](../README.md) | [➡️ Next](./canary-tokens.md)
