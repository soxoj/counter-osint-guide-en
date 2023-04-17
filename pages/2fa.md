# Linking a phone to an account is not always a good idea

**Do not use confirmation via phone number where it is not necessary.**

2FA is used to enhance security. Use an additional factor to log in to the site when you realize
that an account on a particular site is important to you (correspondence, purchases, finances), and that you will consciously confirm the login every time.

However, if there is a choice of what exactly to use for confirmation - a phone number or something else - then use something else.
Companies are interested in knowing your number: sending you SMS, verifying your identity, linking it with other sites.
Just as easily, they will give out part of your number when trying to log in to your account or when your friend gives the app access to his contacts.

It's also a bad idea to link someone else's phone. For example, you can link your grandmother's phone to your Google account, because Google for some reason required you to add a phone.
Knowing your account, it will be possible to get part of your grandmother's phone number through, for example, restoring access.

#### Where are information leaks about your accounts possible at all?

* Login form. For example, the service may respond with the messages "a user with such an email does not exist" and "you entered the wrong password", which clearly
confirms the presence of an account with your mailbox.

* Registration form. The site will not allow you to register an account for a phone that is already in the system: "this phone is already in use." And if it's not there, then a notification will most likely be sent to the phone.

* Access recovery form. Most often, some data is entered, for example, the account nickname, and the service responds with something like `A new password has been sent to the mailbox*****ov@mail.com ` or `We sent an SMS to a number ending in 93`. Or asks you to enter an email, and then writes "if such an account exists, then we have sent a notification." And Meta (Facebook) only needs to know the account ID.

In all these places, there may be a leak of the second factor (phone number) that you link to your account.

---

<details>
  <summary>🥷 Advanced level</summary>
  </br>

### Using BitWarden to generate email aliases

The BitWarden password manager allows you to generate random aliases of plus mail,
as well as catch-all mailbox addresses and even mailboxes for forwarding.

Read more about these features in the section "🥷 Advanced level" of [Mailbox](./email.md).

![image](bitwarden_ru.png)

</details>


[⬅️ Back](./development.md) | [⏫ Table of contents](../README.md) | [➡️ Next](./deleteme.md)
