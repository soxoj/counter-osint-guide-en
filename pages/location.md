# Address and location

To begin with, we will highlight several criteria that it makes sense to pay attention to from the point of view of OPSEC.

These are:
- geolocation: your real-time location, which most often leaks through digital channels; it can be both coordinates and the address to the apartment;
- permanent registration address: what is most often called a "residence permit" is an anachronism of post-Soviet Russia, required in many state systems, but almost everywhere superseded by the following address
- address of actual residence: the address at which you are "temporarily registered", also required by various laws and acts to be able to provide you with various services.

Unfortunately, unlike in the USA, where your address = your mailbox, in Russia the address is strictly tied to physical real estate. Therefore, we cannot have tricks with "nomadism" as in Texas or South Dakota, where you do not necessarily have a place of residence. However, it is possible to use subscriber boxes, as described below.

## How to prevent address leaks

- Do not publish photos in a "raw" form, files. They often contain information about the shooting location.
- If you use delivery, specify the minimum required amount of information in the standard address fields.
The most preferable option is to specify only the house number and meet the courier outside.
Write everything else (floor / apartment / intercom) in the additional information field — the courier will easily read it, but such unstructured information is less likely to get into the database with your address.

## Using subscriber boxes

In Russia there is a single state operator of the postal network: Russian Post. He carries out most of the mail.

For delivery, the address of the person's stay and his name are usually used, i.e., it is necessary to specify the full name, postal code, as well as the full address, including the apartment number. Ordinary letters or notices of registered letters/parcels are delivered by postmen up to the mailbox on the door of the house or in the entrance of an apartment building.

However, there is a possibility of anonymous mail delivery for the sender using [subscriber ящиков](https://ru.wikipedia.org/wiki/%D0%90%D0%B1%D0%BE%D0%BD%D0%B5%D0%BD%D1%82%D1%81%D0%BA%D0%B8%D0%B9_%D1%8F%D1%89%D0%B8%D0%BA).
This is a dedicated mailbox for mail in a specific mail division. Each box has its own number, online you can choose any unoccupied, for example, `777`.
Also, under the lease agreement, it can be assigned an arbitrary name - this is a paid (and relatively expensive) service.
The only disadvantage from the point of view of privacy is that to rent a mailbox, you need to create an account on abox.pochta.ru by specifying your phone number and passport details.

After signing the contract, you will receive the key to the mailbox, and you can open it at any time. But it is important to understand that the boxes are located on the territory of post offices, and access to them is regulated by its working hours.
Therefore, it is more convenient to choose the largest branches where the subscriber department works around the clock. In Moscow, for example, this is a post office on Myasnitskaya Street, index `101000`.

How do I send emails now? As an address, ask your correspondents to specify only the index and the mailbox number. Let's take the examples above.

Canonical entry: `101000, subscriber/mailbox 777`

Or in short: `101000, 777`

And if you have assigned the name "Dump" to the box, then: `101000, Dump`

---

The rules for the delivery of shipments also apply to subscriber boxes. This means that only notifications will be sent to you for registered letters,
and to receive them, you need to dictate the phone number to the employee of the subscriber department, receive an SMS, and only after that you will be given a letter.
But ordinary letters, of course, will be put directly in the mailbox.

---

[⬅️ Back](./fio-birthday.md) | [⏫ Table of contents](../README.md) | [➡️ Next](./password.md)
