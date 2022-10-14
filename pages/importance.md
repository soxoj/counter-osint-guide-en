# Why it is important

It's hard to stay off the grid in these digital times. A hermit may have an emergency phone, and a dog, though not every dog, may have an Instagram account.

The pervasiveness of social media and communications could be highly positive if it didn't lead to many unfortunate consequences. For example, fake Sberbank employees calling to ask you to dictate your password from a text message to debt collectors suddenly demanding the return of a loan taken out on the information extracted from your passport.

In recent years, there has been a trend towards privacy and protection of user information: GDPR, CCPA, and LGBD. Companies have been obliged to secure personal data and prevent leaks. But are they collecting less information about us? No. Our data is a source of profit for them.

But the tightening of regulations is not enough for companies. You probably left a lot of "breadcrumbs" because you've been on the Internet for years: Old accounts, advertisements, public correspondence, and photos. These traces can be used to get close to you and exploit it for whatever purpose.

---

*Interesting fact: in 2017, a journalist [found the anonymous accounts of the FBI director](https://gizmodo.com/this-is-almost-certainly-james-comey-s-twitter-account-1793843641) in just a couple of hours. It was enough to get a tip about his existence, information about his son and about his thesis in theology.*

---

The enormous amount of data about people that can easily be collected by improvised means has led to the popularity of OSINT, a methodology for collecting and analysing data from open sources. The term is now often used to refer to "spying on people" or "deanonymisation" techniques, even though it was initially an intelligence methodology. Any tool can be used for good and bad - this is something to keep in mind.

It is, therefore, essential to have "**Counter-OSINT**" means and tools to protect your data and ensure your privacy.

## What will happen in the next sections

We will study simple but effective steps that will make it very difficult for an outsider observer to gather information about you.

The guide will be helpful to the broadest range of people interested - not just those who have heard something about OSINT but also friends, acquaintances and parents. An investment of half an hour for thoughtful reading and deliberate actions will bring peace of mind and protection against fraud, surveillance, harassment, and blackmail.

At the same time, let's not neglect convenience. Many guides concentrate on keeping ourselves as safe as possible (even if it's not justified). On the other hand, We will start from the need to maintain **a balance between privacy and convenience**, in which Internet use is not complicated.

---

Let me remind you that OSINT is about collecting information from open sources. Unfortunately, our most sensitive data as phone number databases, passport data, and so on, often end up on the Net.

In the Russian Federation, through "probing", you can get detailed information about the owner of a phone number, car, or flat from official state registers and databases. Unfortunately, many people are willing to grant access for money to something that should be carefully protected.

Let's face it: it is impossible to ensure complete anonymity and remove yourself from all registers, but it is possible to complicate the search process so much that an intruder cannot cling to some information about you.

Thus, the purpose of the manual is to teach you how to protect publicly available information and make it harder to find other information about you.

### Defining important information

To understand which data is more critical and what should be protected more, you need to know the current realities, adjusted for Runet. That is what we will look at next, and to be objective, we will adopt [Operations Security (OPSEC) measures](https://en.wikipedia.org/wiki/Operations_security).

The term OPSEC, like OSINT, comes from US intelligence. It refers to the process that "_identifies critical information to determine if friendly actions can be observed by enemy intelligence, determines if information obtained by adversaries could be interpreted to be useful to them, and then executes selected measures that eliminate or reduce adversary exploitation of friendly critical information_".

![Болтать - врагу помогать!](../img/37ddd605b06fdfb1793be.png)

First, let's list all the **primary data** that reveals our identity in one way or another that *exists physically off the Internet*. 

- Surname, first name, patronymic
- Date of birth
- Passport details (series, number, etc.)
- Physical address
- Personal documents (driving licence, etc.)
- Biometric data
- Other personal information

There is not much data like that. But with at least some of it, a hostile actor could pretend to be you and deceive a third party. For example, he could send a message to someone you know asking them to wire you money urgently because of a problematic situation.

In doing so, fraudsters will not necessarily be interested in your identity. For example, they can buy a database containing hundreds of "fresh" passports to link passport details to [QIWI e-wallets](https://qiwi.com/) to increase withdrawal limits.

Any personal data can be exploited. For example, restoring access to social media accounts often requires answering a security question. Thus, knowing your mother's maiden name or your favourite musician will increase the chances that your profile will be hacked by a hostile actor.

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

