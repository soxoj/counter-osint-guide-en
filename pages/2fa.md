# Linking a phone number to an account

**Don't use phone number verification where it's not required.**

2FA is used to enhance security. Use an additional authentification factor to log into the site when you realize
that the account on a particular site is important to you (correspondence, purchases, finances), and that you will consciously confirm the entry every time.

However, if there is a choice of what to use for confirmation - a phone number or _something else_ - then use something else.
Companies are interested in knowing your number: send you SMS, verify your identity and link it with other sites accounts.
They easily will give out part of your number when somebody try to log into your account or when your friend gives the application access to their contacts.

It's also a bad idea to use someone else's phone. For example, linking your grandmother's phone to your Google account if Google for some reason required you to add a phone.
Knowing your account, it will be possible to get part of the grandmother's phone number through access recovery, for example.

#### Where is information about your accounts likely to be leaked?

* Login form. For example, the site may respond with the messages "The user with this email does not exist" and "Wrong password", which is unambiguous confirms the existence of your account.

* Registration form. A site will definitely not let you register an account on a phone that is already used: "This phone is already registered.". But if it is not used, then a notification will most likely be sent to the phone.

* Recovery form. Most often, one data is entered, for example, the account nickname, and the service responds with something like "a new password was sent to the iva*****ov@mail.com mailbox" or "We sent an SMS to a number ending in 93". Or the service asks to enter email, and then writes "If such an account exists, then we sent a notification.". Some sites like Meta only needs to know the account ID.

In all these places, the 2nd factor (phone number) that you bind to the account can leak.

---

[⬅️ Back](./development.md) | [⏫ Table of contents](../README.md) | [➡️ Next](./deleteme.md)
