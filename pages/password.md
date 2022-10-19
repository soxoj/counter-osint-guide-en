# Passwords

Main principle: **Never use the same or similar passwords**

There are two reasons for this:
- If someone has your email address and password from one site, they will definitely try to go to a second site with those details. It's not personal, the market for selling hacked accounts is very large, and this is a valuable commodity.
- If data about your accounts, along with your passwords happened to [leak](./breaches.md), then it would be possible to compare different emails and phone numbers with one another ([a good example](https://meduza.io/feature/2022/02/07/eto-pohozhe-na-krik-dushi-no-ya-ne-znayu-o-chem-on-krichit)).

But how do you manage to remember a multitude of passwords? I advise you not to treat all passwords as data that should always be in your head. Save space in your memory.

The best way is to create one passphrase long enough for the password store (or for the account that your browser is linked to, where all passwords are stored).

*The section will be updated*

## How to come up with strong passwords

The standard guidelines for using eight characters, which include special characters, letters, and numbers, do not work! After all, `P@ssw0rd` also meets these requirements, and this is not the coolest password. So, let's analyze the best methods for creating a strong password.

### Three random words
There is a simple but effective method for creating passwords - the method of 3 random words

What is this method? When we register a new account, we just come up with 3 random words and put them as our password, for example: `NETWORKINGHYGIENEDEVELOPMENT `
I’m sure you would agree, this is much easier to remember than `asndjBDHJBSDhjSBADHJadbzhjF`, and it will be quite difficult to bruteforce this password by a simple dictionary attack.

Such passwords can be strengthened even further using [LEET](https://ru.wikipedia.org/wiki/Leet), replacing *some* letters with numbers, that is, our password will look like this: `N3TW0RKHY6I3N3D3V3L0PM3NT`
This way, our password becomes stronger, and its complexity for memorization does not increase by much., And if you are familiar with [LEET](https://ru.wikipedia.org/wiki/Leet), this will make it even easier for you.

For even greater durability, you can separate words using different special characters, such as: `-`, `~`, `=`.

### Russian words in English layout

Another simple but effective method is to use random Russian words in the English layout.

Just take random words in Russian and write them in English. For example, from `ехалгрекачерезреку` (a Russian paraphrase
 part), we can get the following:
`t[fkuhtrfxthtphtre`.

It looks interesting and is quite stable, and you can add symbols and numbers at the end. Here’s an example:
`t[fkuhtrfxthtphtre123!`
`t[fkuhtrfxthtphtre34345!`

*The section will be updated*

## Password managers

This is something everyone should use! If you recall the main principle from the first line, the following question immediately comes to mind, "Well, what should I do now, remember 100 passwords?!". But don’t worry, you don't need to remember 100 passwords only one. And this is the password for the password manager.

The password manager will allow you to generate strong passwords and store them in one (and most importantly) safe place.

An synopsis of popular password managers can be found in this article: [Overview of password managers](https://habr.com/ru/company/cloud4y/blog/581916/).

The personal recommendation of the compilers of the guide will be the [Bitwarden](https://bitwarden.com/) service. For personal use, it's more than enough. The free version includes unlimited password storage, use of an unlimited number of devices, and all the basic functions of password managers. In addition to storing passwords, you can also store your bank card numbers and notes. The password generator allows you to generate a strong password and check it in leaks, which is undoubtedly one of the "Killer Features".

### LessPass

What if you find it difficult to store passwords and sync them across devices? Password managers come to the rescue without having to store anything!

LessPass is not the only such program, but one of the most well-known. Its concept is that one-time passwords are generated on the fly using a function, the result of which is always the same, provided the parameters are the same.

The program must be given the following details:
- master password
- site login
- website address

After that, it will generate your password without sending any data or saving anything anywhere. You can run this program at any time, on any device, and get your password for whichever particular site necessary.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/31013580/194948775-cfe3987f-acde-456a-a78b-5281dd06171e.png">

<img width="499" alt="image" src="https://user-images.githubusercontent.com/31013580/194949724-dc26b60c-4607-40cf-a101-ead867dea009.png">

## Useful materials and links to sources

- [The free password manager LessPass runs on pure function](https://www.pvsm.ru/open-source/207324)

---

[⬅️ Back](./location.md) | [⏫ Table of contents](../README.md) | [➡️ Next](./photo.md)
