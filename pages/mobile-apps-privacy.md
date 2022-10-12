# Phone privacy

The topic of privacy on mobile devices deserves a separate large guide. User data is of too great financial interest for all vendors. And if there are moves towards privacy in the Western market (for example, Apple reduces the ability to collect data for all third-party applications, and Google improves access management to applications every version of Android), then in the Asian market (Samsung, Xiaomi and a lot of small vendors) user data settles in large quantities and uncontrollably.

What can be done with this in a short time and without complex manipulations like getting root or jailbreak? Unfortunately, we can do only the minimum: to keep track of which applications you install and what permissions you give them. Let's analyze the most obvious cases.

## Phone contacts

Many applications have done their business only on access to the user's phone book. The most known is GetContact, which was popular with Russian users. The mechanism is simple - a bunch of the contact's name and phone number from your phone transfer to the GetContact servers, where they are combined into one database. After that, it becomes possible to find out full name by phone number by requesting directly in the database (also a profession, and age, and anything at all). For example: "Ivan FSB", "Alexander Client", "Valeria Khrushchev 42", "Masha Petrova Model". Now all this data can be easily obtained through Telegram bots.

Some other applications (for example, quite official ones like Sberbank) request access to the phone book in order to shorten the movements for bank transfers by phone number by a couple of clicks. At the same time, obviously, the contacts will be uploaded to their server anyway, and what will happen to them there is unknown.

Therefore, the first and obvious step towards privacy (both yourself and your familiars) will be to restrict access to the phone book totally - we do not give it to applications on request, because they must function without it (Sberbank does fine without it). Otherwise, we carefully study the application and look for alternatives if it unconditionally requires you to give your phone numbers.

## Installed applications

Continuing the topic from the previous paragraph: applications for collecting contacts worked not only explicitly, but covertly, being introduced for money into other, free applications.
Thus, a large number of inattentive people themselves leaked their data, not paying attention to the fact that the next game from Google Play requests too many extensions. And few people read license agreements nowadays, unfortunately.

## Used materials and useful links

- [List of free, open source and privacy respecting services and alternatives to privative services](https://github.com/pluja/awesome-privacy)

---

<details>
  <summary>🥷 Advanced level</summary>


## Wi-Fi

Каждый телефон, который может подключиться к беспроводной интернет-сети, обладает MAC-адресом. Этот адрес используется телефоном
не только во время подключения, но и даже при поиске "знакомых" Wi-Fi-сетей вокруг.

Этим пользуются компании, организующие интернет в общественных пространствах. Они настраивают свои устройства на сбор всех MAC-адресов
проходящих вокруг людей. Таким образом, становится возможным не только отслеживать перемещения и посещения, но даже следить за конкретными
людьми до места жительства. А если человек подключился к "опасной" точке доступа, то становится возможным связать телефон с ним напрямую.

Отдельная заметка касательно сбора MAC-адресов телефонов, находящихся в режиме поиска сетей. Устройства Apple по умолчанию поддерживают
создание случайных MAC при поиске, с версии iOS 14 также делают случайные адреса для каждой сети Wi-Fi при подключении. Устройства Android
менее приватны, возможность использования случайных идентификаторов появилась только с версии Android 10.

**Придерживайтесь следующих правил:**
- Выключайте Wi-Fi на устройстве, когда он вам не нужен.
- Не подключайтесь к публичным беспроводными сетям.
- Периодически очищайте список известных Wi-Fi в телефоне.

*The section will be updated*

- [Прошли мимо кафе, а вам тут же показали его рекламу? Это не паранойя](https://meduza.io/feature/2018/10/24/proshli-mimo-kafe-a-vam-tut-zhe-pokazali-ego-reklamu-eto-ne-paranoyya)
- [Telegram-канал про защиту смартфонов на Android](https://t.me/tvoijazz)

</details>

---

[⬅️ Back](./making-breaches-useless.md) | [⏫ Table of contents](../README.md) | [➡️ Next](./platforms.md)
