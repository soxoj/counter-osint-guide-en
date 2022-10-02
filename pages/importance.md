# Why is it important

It's difficult to stay out of reach in our digital time. A hermit may have an emergency phone, and a dog, although not every dog, may have an Instagram account.

The development of social networks and means of communication could be extremely positive if it did not lead to a lot of sad consequences. For example, calls from fake bank employees asking them to dictate a one-time code from SMS or collectors suddenly demanding to pay back the loan taken on your passport.

In recent years, there has been a trend towards privacy and protection of user information: GDPR, CPA, LGBD. The companies were obliged to take care of the safety of personal data and to prevent their leaks. But did they start collecting less information about us? Absolutely not. For them, our data is a source of profit.

But the tightening of legal norms for companies is not enough. You probably left a lot of "breadcrumbs" to your identity, because you have been living in the Internet for years: old accounts, ads, forums, photos. Following these traces, it's possible come close to you and use your personal information for any purpose.

---

*Interesting fact: in 2017, a journalist [found the anonymous accounts of the FBI director](https://gizmodo.com/this-is-almost-certainly-james-comey-s-twitter-account-1793843641) in just a couple of hours. It was enough to get a tip about his existence, information about his son and about his thesis in theology.*

---

A huge amount of data about people, which can be easily collected by improvised means, has led to the popularity of OSINT, a methodology for collecting data from open sources. Often, this term is using as "spying on people" or "deanonymization", although initially it is a general intelligence methodology. Any tool can be used for both good and bad purposes — this should not be forgotten.


Therefore, it is important to have **Counter-OSINT** tools to protect your data and ensure privacy.

## What will happen in the next sections

We will study simple but effective actions that make it very difficult for an external observer to collect information about you.

The guide will be useful to a wide range of interested people — not only those who have heard something about OSINT, but also friends, acquaintances, relatives. An investment of half an hour for thoughtful reading and conscious actions will bring peace of mind and protection from fraud, surveillance, harassment, blackmail.

At the same time, we will not ignore the comfort. Many guides concentrate on protecting to the maximum (even if it is unjustified). We will start from the need to maintain **a balance between privacy and comfort**, so the use of the Internet will not be complicated.

---

Let me remind you that OSINT is about collection of information from open sources. Unfortunately, such sensitive data as phone numbers, passports and so on often get into the Network, to the public domain.

Moreover, in Russia, through "probiv", you can get detailed information about the owner of a phone number, car, apartment from official state registers and databases. Many people are providing access for money to what should be carefully protected.

We will take this into account: it is impossible to ensure complete anonymity and remove yourself from all registries, but it is possible to complicate the search process so much that an attacker will not be able to cling to the some information about you.

Thus, the purpose of the guide is to teach how to protect publicly available information and complicate the process of finding other information about you.

### Defining important information

Чтобы понять, какие данные важнее и что следует больше защищать, необходимо знать современные реалии с поправкой на Рунет. Это мы и разберём далее, и чтобы попытаться быть объективными, используем OPSEC.

Термин OPSEC, как и OSINT, пришёл из американской разведки. Он означает процесс анализа и защиты критически важной информации.

![Болтать - врагу помогать!](../img/37ddd605b06fdfb1793be.png)

Для начала перечислим все **первичные данные**, которые так или иначе раскрывают нашу личность, но *существуют физически вне Интернета*. 

- Фамилия, имя, отчество
- Дата рождения
- Паспортные данные (серия, номер и т.д.)
- Физический адрес
- Личные документы (водительское удостоверение и т.д.)
- Биометрические данные
- Прочая личная и идентифицирующая информация

Таких данных не так много. Но, имея хотя бы часть, можно притвориться вами и обмануть третих лиц. Например, разослать знакомым сообщение с просьбой срочно перевести деньги из-за трудной ситуации.

При этом мошенники не обязательно будут заинтересованы конкретно в вашей личности. Например, они могут купить базу и сотни "свежих" паспортов, чтобы привязывать паспортные данные к электронным кошелькам QIWI для увеличения лимитов по выводу денег.

Любые личные данные могут быть использованы. Например, восстановление доступа к аккаунтам социальных сетей часто требует ответить на контрольный вопрос. Таким образом, знание девичьей фамилии матери или любимого музыканта повышает шансы взломать вас.

---

*Интересный факт: [в 2012 произошел громкий случай](https://habr.com/ru/post/149179/) захвата сразу 4 аккаунтов человека при знании только лишь адреса, имени и email. Элегантная цепочка восстановления доступа — сначала использовать известные данные, потом привязать фальшивые — позволяла сначала завладеть доступом в Amazon, GMail, Apple, Twitter, а потом и вовсе удалённо стереть данные с устройств человека.*

---

Возможно, вас смутил пункт "биометрические данные", но, увы, их использование уже давно вошло в нашу жизнь. Уже давно распространены средства поиска по лицу, которые используют те же технологии, что и для разблокировки личного телефона через переднюю камеру, а также обширные базы данных из социальных сетей. Когда вы оставляете свою фотографию в Сети, вы оставляете возможность найти себя.

### Анализируем угрозы

В соответствии с процессом OPSEC проанализируем, кто может быть заинтересован в подобных действиях и как может использовать информацию о нас. Давайте рассмотрим популярные случаи использования первичных данных на схеме ниже и попробуем сделать выводы. 

![Что можно сделать с нашими данными?](../img/0869d0a1e60173af48378.png)

Что можно сделать с нашими данными?
Наверняка вы обратили внимание, что большинство пунктов связано с **получением денег**. Думаю, финансовая мотивация мошенников не требует объяснения. Единственное, что следует отметить — деньги могут быть похищены не только у вас, но и у других лиц. В этом случае критичным для нас становится участие в уголовном процессе, куда могут привлечь как свидетелем, так и обвиняемым. 

Выгода от сбора полной информации о вас, включая доступ к перепискам, менее определена. Это может быть как бытовое преследование, так и шпионаж, шантаж и прочее. Ясно только, что в большинстве случаев это **причинение личного вреда и вторжение в частную жизнь**.

Эти угрозы понятны и объяснимы, а во многих случаях регулируются законом. Статьи, связанные с финансовыми потерями, перечислять нет смысла, настолько их много; а сбор личных данных — это 137 УК РФ. Однако, давайте взглянем правде в лицо: требуется серьёзная причина, чтобы идти и самостоятельно форсировать возбуждение дела, а участие в таких процессах — стресс. Поэтому вернёмся к уже озвученной выше позиции: наша цель в том, чтобы защитить свои данные и избежать угроз.

---

Очевидно, что знания первичных данных недостаточно для проведения мошеннических схем. Таковые обычного основаны на социальной инженерии и предполагают дистанционное взаимодействие через звонок или сообщения. То есть, мы неявно подразумеваем, что у недоброжелателям уже известны наши **вторичные данные, виртуальные идентификаторы** — номер телефона, электронная почта, адрес аккаунта социальной сети. Таким образом, получение информации об этих данных несет в себе не меньшую угрозу.

Про каждый из типов данных дальше будет рассказано подробнее. А пока оставим своё внимание на том, что чем больше данных попадает в чужие руки, тем серьёзнее может быть исход. Отсюда вывод — количество данных о вас необходимо контролировать, не разбрасывать их где не следует и следить за их использованием.

Поговорим о **цифровой гигиене**.

---

[⬅️ Back](./intro.md) | [⏫ Table of contents](../README.md) | [➡️ Next](./hygiene.md)

