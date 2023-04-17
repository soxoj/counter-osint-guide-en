# Phone privacy

The topic of privacy on mobile devices deserves a separate large guide. User data is of too great financial interest for all vendors. And if there are moves towards privacy in the Western market (for example, Apple reduces the ability to collect data for all third-party applications, and Google improves access to applications with each version of Android), then in the Asian market (Samsung, Xiaomi and a lot of small vendors) user data settles in large quantities and uncontrollably.

What can be done with this in a short time and without complex manipulations like getting root or jailbreak? Unfortunately, the minimum is to keep track of which applications you install and what permissions you give them. Let's analyze the most obvious cases.

## Contacts from the phone book

Many applications have done their business only on access to the user's phone book. The most sensational is GetContact, which has gone through a wave of Russian users. The principle is simple - a bunch of the contact's name and phone number from your book leak to the servers, where they are combined into one database. After that, it becomes possible to find out the full name by phone number by requesting directly in the database. And sometimes a profession, and age, and anything at all. For example: "Ivan FSB", "Alexander Client", "Valeria Khrushchev 42", "Masha Petrova Allegedly Model". Now all this data can be easily obtained through Telegram bots.

Some other applications (for example, quite official ones like Sberbank) request access to the phone book in order to shorten the movements for transfers by phone number by a couple of clicks. At the same time, obviously, the contacts will be uploaded to their server anyway, and what will happen to them there is unknown.

Therefore, the first and obvious step towards privacy (both yourself and your loved ones and acquaintances) will be to restrict access to the phone book - we do not give it to applications on request, because they must function without it (Sberbank does fine without it). Otherwise, we carefully study the application and look for alternatives if it unconditionally requires you to give your numbers.

## Installed applications

Continuing the topic from the previous paragraph: applications for collecting contacts worked not only explicitly, but covertly, being introduced for money into other, free applications.
Thus, a large number of inattentive people themselves merged their data, not paying attention to the fact that the next game from Google Play requests
too many extensions. And few people read license agreements nowadays, alas.

## Materials used and useful links

- [List of alternative services and applications aimed at privacy](https://github.com/pluja/awesome-privacy)

---

<details>
  <summary>🥷 Advanced level</summary>


## Wi-Fi

Every phone that can connect to a wireless Internet network has a MAC address. This address is used by the phone
not only during connection, but even when searching for "familiar" Wi-Fi networks around.

This is used by companies that organize the Internet in public spaces. They set up their devices to collect all the MAC addresses
of people passing around. Thus, it becomes possible not only to track movements and visits, but even to monitor specific
people to the place of residence. And if a person has connected to a "dangerous" access point, then it becomes possible to connect the phone directly with him.

A separate note regarding the collection of MAC addresses of phones that are in network search mode. Apple devices by default support
the creation of random MACS when searching, since iOS version 14 they also make random addresses for each Wi-Fi network when connected. Android devices
are less private, the possibility of using random identifiers has appeared only since Android version 10.

**Follow the following rules:**
- Turn off Wi-Fi on your device when you don't need it.
- Do not connect to public wireless networks.
- Periodically clear the list of known Wi-Fi in your phone.

*The section will be updated*

- [Passed by a cafe, and you were immediately shown its advertisement? It's not a paranoia](https://meduza.io/feature/2018/10/24/proshli-mimo-kafe-a-vam-tut-zhe-pokazali-ego-reklamu-eto-ne-paranoyya)
- [Telegram channel about the protection of Android smartphones](https://t.me/tvoijazz)

</details>

---

[⬅️ Back](./making-breaches-useless.md) | [⏫ Table of contents](../README.md) | [➡️ Next](./platforms.md)
