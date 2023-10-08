# Email address

The email address was and remains the most common identifier for an account on the Network. You may not have a phone number,
but you must have a mailbox - this is an unwritten rule.

The presence of an email in itself reveals some information about you. First of all, this is **alias**, the name of the box, to the left of
the symbol "@". The first and most obvious advice is not to choose your initials, surname and year of birth by name, unless it is a purely personal
or work mailbox.

The second, but important tip is to carefully study the email provider. The most well-known free mail services "in pursuit" of email give
you accounts in other products. This is especially true of Google and Yandex, as these companies conduct their business in a large number of
other areas, and to provide you with a free box for what you will become passive consumer of a dozen other services -- their bread and butter.

## Separation of accounts

To make it more difficult to find information about you, it is recommended to use email addresses wisely, using the technical ability to create their variations. According to RFCs, after the alias and before the @ sign, you can specify an additional suffix with "+", e.g `nickname+facebook@google.com`. Emails to such an email address will be sent to the owner of `nickname@google.com`, but from the point of view of sites, it will be a completely different email address. Google, in addition, has a feature: any dots in the alias are considered optional and work as suffixes after the “+”.

There are several usage schemes: a unique email address for each service, a unique email address for each “personality”, or use only for some services according to a scheme known only to you.

Additional benefits of using suffixes and dots are described [here](./breach-detection.md#using-aliasesfake-mail-addresses). Also, you can check the tool [mailto_analyzer](https://github.com/soxoj/mailto_analyzer) for analyzing of your email address exposure.

## Down with subscription boxes, trash and spam

Separately, it is worth noting the habit of a large number of people to use a separate "garbage" mailbox for non-critical services
and a variety of spam subscriptions. By itself, the separation of mailboxes is useful, but only if it is conscious (see above).

If you do not look into such a box, and the letters are lying there unread by thousands or more, then this is an important signal: figure
out whether you really need this box. If not, then unsubscribe from all mailings and delete the accounts associated with it,
to minimize the possibility of using this email address to collect information about you.

## Disposable email mailboxes

There are a large number of services that provide one-time mailboxes for 10-15 minutes.
They are good for one-time registrations on sites where you get to for the first time and most likely will not use them anymore.
Here we will consider those services that are created on random domains.

Services that generate plausible-looking aliases (first name. last name):

- [TemporaryMail](https://temporarymail.com/)
- [MinuteInbox](https://www.minuteinbox.com/)

Other popular services:
- [10minutemail](https://10minutemail.net)
- [TEMPMAIL](https://temp-mail.org/ru/)
- [Mohmal](https://www.mohmal.com/en)

## Public Email Mailboxes

Also on the Internet you can find services that make it possible to use **your alias** for a temporary mailbox.
Such email addresses are convenient to use for services in which email should look plausible.

Examples of such services:

- [Maildrop](https://maildrop.cc/)
- [Mailsac](https://mailsac.com/)
- [templail+](https://tempmail.plus)
- [Yopmail](https://yopmail.com/) - It can also support forwarding (see below)

## Forwarding mail from other mailboxes

Services that allow you to forward emails use so-called "masks" that allow you to hide your real email address.

The principle of operation is very simple:
- Address-Mask receives an email
- A letter is being forwarded from this address to your real address

Example based on Firefox Relay:

First, a mask is provided that hides the real address.

![firefoxrelay](/img/firefoxrelay.png)

Now, using this mask address, we can receive emails to our email address without showing it to the whole Internet.

![relayedemail](/img/relayedemail.png)

Apple provides an opportunity for its users to use anonymized mailboxes
that function in the same way. They look like this: `1v5zvsmkp6@privaterelay.appleid.com `.

*The section will be updated*

Examples of services:

- [SimpleLogin](https://simplelogin.io/)
- [AnonAddy](https://anonaddy.com/) - generates addresses according to a template `*@ivanov.anonaddy.com`
- [Firefox Relay](https://relay.firefox.com/) - generates random addresses on the domain `mozmail.com`
- [erine.email](https://erine.email/) - makes addresses according to a template `*.ivanov@erine.email`

---

<details>
  <summary>🥷 Advanced level</summary>


## Using a personal domain to create catch-all mailboxes

*The section will be updated*

## Using BitWarden to generate email aliases

The BitWarden password manager allows you to generate random "plus" aliases,
as well as catch-all mailbox addresses and even forwarding mailboxes.

![bitwarden_ru.png](https://github.com/soxoj/counter-osint-guide-en/blob/main/img/bitwarden_ru.png)

*The section will be updated*

</details>

---

[⬅️ Back](./phone.md) | [⏫ Table of contents](../README.md) | [➡️ Next](./fio-birthday.md)
