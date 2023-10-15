# Removing information about yourself

_The section will be updated_

## Deleting your own accounts

Despite the fact that the Internet remembers everything, deleting accounts remains one of the strongest means against basic intelligence on you.
It seems that this is a trivial topic, but there are several important nuances:

Before deleting:
1. Request the service **to upload your personal data** by GDPR. This will help in the next steps and give you an understanding of what
the service knows about you.
2. **Rename your account**, delete/change photos, wait a few days. This is necessary for indexer sites and search engines
we managed to update the information about your account, and subsequently you could not be found by its latest copy. Also, do not forget that
from now on you cannot leave any comments and messages publicly.
3. All old comments/tweets/messages **it is advisable to delete**. There are mechanisms in social networks and messengers that allow you to reach you even
after deletion: mentions (a link to your profile that looks like a name), a mark of authorship, reposts/retweets.
It's worth getting rid of all such leads.
4. Update the search results by asking them to reindex your **modified page** ([Google](https://developers.google.com/search/docs/advanced/crawling/ask-google-to-recrawl?hl=ru)) and wait for a while so that other systems that save information from social networks will also receive a new version of your account.

After that, the account can be deleted using the platform's built-in tools.

### Deletion request

Not in all services, deletion is possible by regular means. Or it is hidden so deep that it is impossible to find it.
Fortunately, there are auxiliary sites with information on how to retire.

- [JustDeleteMe](https://justdeleteme.xyz/) - an excellent directory for platforms, gives links and a description of the necessary actions,
shows the complexity of removal. The creators also have related sites [JustGetMyData](https://justgetmydata.com/) and
[JustWhatsTheData](https://justwhatsthedata.github.io/) to fulfill paragraph 1 above.

- [AccountKiller](https://www.accountkiller.com/en/all-sites) - removal instructions for a large number of sites, mainly Western.

Even if you couldn't find the removal instructions for the site you need, don't despair. There is always an opportunity to write
to support and request the deletion of your account according to GDPR.

## Deleting search results in search engines

Google offers a number of different forms through which you can request the removal and updating of content in search results.

- [Removing outdated content from search](http://search.google.com/search-console/remove-outdated-content) - well suited for pages that need to be reindexed (see above point 4 about deleting accounts).

- [Google Personal Data Deletion Request Form](https://reportcontent.google.com/forms/rtbf?hl=ru)

- [New request form for deletion of personal data](https://support.google.com/websearch/troubleshooter/9685456)

## Removing information about leaks

[Brief instructions for deleting your data from popular services](https://inteltechniques.com/exposure.html) - Have I Been Pwned, Leakcheck, IntelX, etc.

To make requests for services that are interested in storing your data, you need to prepare a complete list of all the information that you want to clean up. It should include:
- nicknames
- phones
- emails
- addresses
- car license plates
- government identifiers (passport number, social security number, taxpayer identification number, full name, etc.)
- any data from leaked database records.
   
### Removing yourself from the Telegram bot Eye of God

The Eye of God has implemented an automatic request to delete personal data in the menu item Account [bot](https://t.me/fandorin_search_bot):

<img width="358" alt="image" src="https://user-images.githubusercontent.com/31013580/193659086-ae6369c4-7fb4-4b2e-a9f3-4e62386816fc.png">
<img width="485" alt="image" src="https://user-images.githubusercontent.com/31013580/193659203-8293ccb8-9991-4ee3-8127-287234a92db4.png">
<img width="736" alt="image" src="https://user-images.githubusercontent.com/31013580/193660218-16fef90a-5eb0-414b-b405-15f60d9681fa.png">
<img width="758" alt="image" src="https://user-images.githubusercontent.com/31013580/193660613-ffa757fc-461e-485c-8092-38356c5120fd.png">

### Hiding the search by itself from the Telegram bot TELESINT

[TeleSINT](https://t.me/telesint_bot) [provides an opportunity](https://telesint.xyz/2021/10/05/service/) hide yourself from the search, send alerts
if they try to find you through the bot, and also view the list of those who were looking for you. Unfortunately, this **requires a paid subscription**.

<img width="487" alt="image" src="https://user-images.githubusercontent.com/31013580/193661209-f9f9430a-be3c-461a-84c5-f322865210a8.png">
<img width="332" alt="image" src="https://user-images.githubusercontent.com/31013580/193661708-142aaa48-0b7e-4c12-98fc-01b6b4b33ce3.png">

### Telegram bot Quick OSINT

In the Personal Data Processing Policy [of the service](http://quickosint.com) said:

```
The period of processing of personal data is unlimited. The User can withdraw his consent to the processing of personal data at any time by sending a notification to the Operator @Quick_OSINT_support marked "Withdrawal of consent to the processing of personal data".
```

All requests for deletion are processed manually, it is necessary to fill out an application for blocking data from publicly available sources
with full passport data, the bot's address, as well as identifiers for blocking, and then send its photo or scanned image to [the Operator](https://t.me/Quick_OSINT_support). The data will be deleted within 7 days.

### Telegram bot Insight

To hide data about yourself in the bot [Insight](https://t.me/eyeofbeholder_bot) it's necessary:
- to have at least ₽1000 deposits for the entire time from the account
- contact @tginsighter with a request to delete your data

### Telegram bot GTA

To hide data about yourself in the bot [GTA (Global Tech Aggregator)](https://t.me/globaltechagr_bot) it's necessary:
- to start the bot
- "Мой аккаунт" - "Удалить информацию" - "Удалить запись"
- individually enter the identifiers of interest
- replenish the wallet in TON (for deletion for a year - 1 TON for 1 ID, permanently - 5 TON for 1 ID)

<img width="176" alt="gta_1" src="https://github.com/soxoj/counter-osint-guide-ru/assets/137871056/bd243977-9a9b-48de-b820-3e6f0817ac7b">  

<img width="315" alt="gta_2" src="https://github.com/soxoj/counter-osint-guide-ru/assets/137871056/274abf57-d2c2-43ed-8b96-bd4c0e19e40b">  

<img width="371" alt="gta_3" src="https://github.com/soxoj/counter-osint-guide-ru/assets/137871056/54bc61eb-b6d0-4f69-bc48-c194d8095223">  

### Telegram bot Zernenda

To hide data about yourself in the bot [Zernenda](https://t.me/Zernerda_bot) it's necessary:
- to start the bot, verify your account
- check what data the bot knows about you and from what leaks (to do this, pay several requests for your phone number, full name, etc.; write out to yourself what data the bot has found)
- "Мой аккаунт" - "Удалить данные о себе"
- send your phone number to confirm your account
- send a detailed request indicating which data you own

Sample application form:

ФИО: Пушкин Владимир Владимирович
Телефон: +79999999999
Telegram: tg1569113435
ВКонтакте: vk10419593
Паспорт: 1234 567890
Я подтверждаю, что приведённые выше данные принадлежат мне и прошу удалить их из поисковой выдачи бота.

<img width="317" alt="Zernenda_1" src="https://github.com/soxoj/counter-osint-guide-ru/assets/137871056/15171573-caae-4899-90d1-023d0a227354">  

<img width="380" alt="Zernenda_2" src="https://github.com/soxoj/counter-osint-guide-ru/assets/137871056/2b9dc6bd-d20d-4b4e-a2f4-60e29596f8fa">

### Telegram-bot Angel (Архангел)

To hide data about yourself in the bot [Angel (Архангел)](https://t.me/Angel_SystemBot) it's necessary:
- to start the bot
- "Профиль" - "Приобрести запросы"
- buy requests (the option "800 запросов - 5760 руб." is required)
- start the bot: https://t.me/AngelSystemSupportBot
- write "Пополнил на 800 запросов. Прошу удалить мои данные из вашей системы (you should write what kind of data - phone, mails, social networks, documents, addresses, etc.)"

<img width="317" alt="angel" src="https://github.com/soxoj/counter-osint-guide-ru/assets/137871056/b514f608-8d72-4b2a-9684-2b90c9b50494">  

### Telegram-bot Cerberus

To hide data about yourself in the bot [Cerberus](https://t.me/iscerberusbot) it's necessary:
- to start the bot
- "Аккаунт" - "Защитить данные" - "Создать"
- enter the data that you are asked to enter one by one

### GetContact

In GetContact, it is possible to arbitrarily disable the display of names that are known by your number, or disable the search altogether.

To do this, follow [this link](https://www.getcontact.com/en/manage/profile) and log in via messenger, then turn it off.

It should also be noted that in this section of the site you can track search queries by your number. If you disable the search, this feature is lost
as well as receiving notifications about finding you from the app. However, when you log in to the GetContact application again, this feature is returned.

<img width="918" alt="GetContact1" src="https://user-images.githubusercontent.com/31013580/193679883-e7a24933-cc95-4354-993d-b02c3b9c8a11.png">

<img width="471" alt="GetContact1" src="https://user-images.githubusercontent.com/31013580/193679897-e84664b5-8bc1-4f77-a5b1-ee39e5eac965.png">

---

[⬅️ Back](./2fa.md) | [⏫ Table of contents](../README.md) | [➡️ Next](./screen-sharing.md)
