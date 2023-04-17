# Determining the source of the leak

## Finding yourself in leaks

There are many sites that allow you to find yourself by phone, mail, or even full name yourself in information leaks and merged databases. They should be used with caution, because any online search may have an additional purpose in enriching data. For example, **collecting an IP address**, linking several searches of one person to **collect information about his environment**.

Therefore, the preferred option is always *independent search in leak files*.

But it can be difficult: you need to find a file (or a lot of files if you need an exhaustive search), understand its structure, perform an effective search.

If you went the simpler way, then I recommend using such resources in descending order of risks:

#### Well-known safe sites

The most famous: [Have I Been Pwned](https://haveibeenpwned.com/), supported by a well-known
security guard and giving guarantees of privacy.

Other:
- https://monitor.firefox.com/

#### Commercial alternatives

They often give shareware access, you can find different sites by the keywords check, leak:

- https://leakcheck.io/
- https://checkleaked.cc/

#### Bots in Telegram

- https://t.me/PhoneLeaks_bot - search for sources of leakage

Most bots do not indicate the source from which the information is obtained. List of some resources:
[Google Spreadsheet](https://docs.google.com/spreadsheets/d/1XerMPGwaDz1FG1gBumBp6jzOgSqhWcQWgZmhxoT60WA/edit#gid=0).


#### Notifications

Some of the sites listed above also can notify you by email if there is a new leak with your data. I highly recommend using such a service if you lead an active virtual life.

## Using aliases/fake mail addresses

Gmail and other most common mail services support special characters to create aliases for your mailbox. Mail sent to an alias will come to your primary email address, but you will clearly see where it came from in the Recipient field.

For example, `soxoj@protonmail.com` is equivalent to `soxoj+gitlab@protonmail.com`:

<img width="311" alt="Email aliases" src="https://user-images.githubusercontent.com/31013580/193665517-c06dd5d4-1c6b-468d-8a16-34db0e0689a5.png">

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

## Using different names for tracking

So, if you are not interested in the receipt, then provide a knowingly wrong mailing address pointing to the source of the leak, e.g. eyeofgod@receipt.com. Or use the aforementioned aliases, explicitly exposing where the email account was listed.

Websites have different approaches to the accuracy of first and last names of accounts. Some require that they coincide with passport data ([e.g., in VK](https://roem.ru/21-06-2009/126784/v-v-kontakte-mojno-smenit-imya-lish-na-nastoyashchee/)), some only check them against documents in case of financial transactions, and most do not validate at all.

You can use the tricks listed below depending on the strictness of the service rules (ToS, Terms of Service). But before using them, I strongly advise you to study what sanctions are possible if you specify an invalid name and assess these risks for yourself.

#### Use names/surnames that are consonant or begin with the same letters as the site/company.
That way, if that name will be leaked in conjunction with a number or mail, you'll know where the information came from:

- McDonald's: _Maxim_
- VKontakte: _Vova_
- Odnoklassniki: _Oleg_

#### Use variations of the name in Cyrillic or Latin
First of all, this applies to the full/abbreviated form of the name:

- Alexander
- Sasha
- Sanya
- Shura

But because of language differences, a name can have several "Latin" forms.
Even banks often give the option of choosing the correct transliteration of names.
Thus, the name "Anatoly" can be expressed as:

- Anatoly
- Anatolii
- Anatoliy

---

<details>
  <summary>🥷 Advanced level</summary>
  </br>

### Using BitWarden to generate email aliases

The BitWarden password manager allows you to generate random email aliases with a plus, as well as catch-all mailbox addresses and even mailboxes for forwarding.

Read more about these features in the "🥷 Advanced level" section of the [Mailbox](./email.md) section.

![image](../img/bitwarden_en.png)

</details>

---

[⬅️ Back](./breaches.md) | [⏫ Table of contents](../README.md) | [➡️ Next](./canary-tokens.md)
