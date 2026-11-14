# Password

The main principle: **never use the same or similar passwords.**

For two reasons:
- Having your email and password from site 1, someone will definitely try them on site 2 — and it
is not about you personally: the market for hacked accounts is very large, and your login is
a commodity there.
- If your accounts and passwords surfaced in [leaks](./breaches.md), a shared password ties
together even completely different emails and phone numbers
([a good example](https://meduza.io/feature/2022/02/07/eto-pohozhe-na-krik-dushi-no-ya-ne-znayu-o-chem-on-krichit)).

The second reason matters more for privacy. A shared password links your accounts as firmly as
a shared phone number: it works as one more identifier of yours.

You do not have to remember all your passwords. One is enough — the one for your password manager.
The rest are made up by the program, and you will never even see them.

## How to come up with strong passwords

"Eight characters, letters, digits and a special character" is a poor requirement: `P@ssw0rd`
meets it.

Passwords are not guessed character by character. A dictionary is taken — words and passwords from
earlier leaks — and the usual rules are applied to every word: append a year, capitalise the first
letter, replace letters with lookalike digits. The closer your password is to that pattern, the
faster it is found.

### LEET does not help

Replacing letters with lookalike digits — `password` as `p@ssw0rd`, `NETWORKHYGIENE` as
`N3TW0RKHY6I3N3` — is often recommended as a trick. Everyone knows the trick, and the programs
that guess passwords know it first. Having taken a word from a dictionary, such a program
immediately tries every way of writing it with digits.

The list of substitutions is short, because there are few digits and signs that look like letters:

| letter | replaced with |
|---|---|
| a | 4, @ |
| b | 6 |
| c | <, { |
| e | 3 |
| g | 9 |
| i | 1, ! |
| o | 0 |
| q | 9 |
| s | 5, $ |
| t | 7, + |
| x | % |

This is not our example but a file that ships with hashcat, the best known password-guessing
program. It sits there ready and is switched on with a single checkbox. So remembering the password
got harder for you, while guessing it stayed just as easy as before.

### Words typed in the wrong keyboard layout do not help either

A Russian phrase typed on a Latin keyboard turns `ехалгрекачерезреку` into `t[fkuhtrfxthtphtre`.
It looks like a random string, but switching the layout is just as ordinary a guessing rule. And
the trick is so popular that layout-shifted passwords already sit in the dictionaries as ready
strings.

Kaspersky went through 231 million passwords from leaks of 2023–2026, Russian ones among them.
The most frequent included **`gfhjkm` (the Russian for "password" typed on a Latin keyboard),
`vfvf` ("mum"), `gfgf` ("dad"), and the reverse direction — `мдфв` from `vlad`.** The same study
found that length alone does not save you: one in five 15-character passwords is guessed in under
a minute if it was built from a familiar pattern.

### What does work: a password of random words

The advice "think of three random words" breaks on the word "random". People do not invent
randomness: the words that come to mind are from one topic, from a recent conversation, or start
with the same letter. Such combinations are guessed quickly.

So the words have to arrive ready-made. Every password manager has a button that assembles
a password out of random words — something like `cactus-ribbon-mellow-otter-salt-fabric`. Press,
copy, paste. Three rules:

- take six words, five is already too few;
- keep the words that came up: replacing one with your favourite makes the password predictable;
- separate the words with hyphens or spaces if the site allows it.

If you would rather do without a program, the same words can be picked with a dice roll from
an open [word list](https://www.eff.org/dice): the roll gives the number of the word. That is how
the method was invented, back when password managers did not exist.

A phrase of six random words cannot be guessed, even by someone who knows how you built it. And
you only have to remember one such phrase — the one for your password manager.

## Check your passwords against leaks

You can check a password at [Pwned Passwords](https://haveibeenpwned.com/Passwords), a database of
passwords from known leaks. The password itself is not sent there: the browser turns it into
a fingerprint and sends only the beginning of that fingerprint. From such a fragment the service
cannot tell what exactly you were checking, and the answer is compared on your side. The same
check is built into password managers, Bitwarden among them.

If your password is found, it is already in the guessing dictionaries. Change it everywhere you
used it. For what else about you is in the leaks, see the [Data leaks](./breaches.md) chapter.

## Signing in without a password

A passkey replaces the password with a pair of keys. The private key stays on your phone or
computer and is unlocked with your fingerprint, face or PIN. The site only gets the public key,
and it cannot be used to sign in.

Hence two upsides:

- **if the site leaks, your password will not be in the leak** — it was never there;
- **phishing does not work**: the key is bound to the site's address, and on a fake page the
browser will not offer it.

But there are two privacy caveats as well. The keys are stored in a Google or Apple account, or in
a password manager. They end up with a list of the sites where you set up a sign-in, and that
account itself becomes the key to everything else.

The second caveat is about Russia. "Passwordless sign-in" in Russian services usually means not
a passkey but a QR code, a code over SMS or biometrics. That is, a binding to your phone number or
to your face — for privacy that is a step back.

Support changes fast, so check for yourself: look for "passkey" in the service's security settings.

## Password managers

This is something everyone should use. Recall the main principle from the first line, and
a question comes up straight away: "So am I supposed to remember a hundred passwords?" No, you
need to remember one — the one for your password manager.

A manager comes up with strong passwords and keeps them in one protected place. And it does one
more thing, less noticeable: it fills in a password only on the site it was saved for. If you open
a sign-in page and the manager does not offer the password, the address is not the one you saved.
People rarely spot the difference between `vk.com` and `vk-com.ru` by eye, while the manager
compares the whole address.

The personal recommendation of the compilers of this guide is [Bitwarden](https://bitwarden.com/).
For personal use it is more than enough: the free version stores any number of passwords, works on
any number of devices, can keep card numbers and notes, generates both passwords and passphrases,
and checks passwords against leaks.

### LessPass

What if it is difficult for you to store passwords and sync them between different devices?
Password managers that do not need to store anything come to the rescue.

LessPass is not the only such program, but one of the most famous. Its concept is that passwords
are generated on the fly by a function whose result is always the same given the same parameters.

The program needs to be told:
- the master password
- your login on the website
- the site address

After that it will generate your password without sending any data or saving anything anywhere. At
any time on any device you can run this program — and get your password for a specific site.

This approach has a downside too. The master password cannot be changed on its own: change it, and
all your passwords change at once. And if some site demands a password change or does not accept
the generated one, you will have to remember an exception for it.

<img width="499" alt="image" src="https://user-images.githubusercontent.com/31013580/194948775-cfe3987f-acde-456a-a78b-5281dd06171e.png">

<img width="499" alt="image" src="https://user-images.githubusercontent.com/31013580/194949724-dc26b60c-4607-40cf-a101-ead867dea009.png">

## Useful materials and links to sources

- [Free LessPass password Manager runs on pure function](https://www.pvsm.ru/open-source/207324)
- [Overview of password managers](https://habr.com/ru/company/cloud4y/blog/581916/)

---

[⬅️ Back](./location.md) | [⏫ Table of contents](../README.md) | [➡️ Next](./photo.md)
