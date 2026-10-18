# Database leaks and "probiv" (unauthorized data lookup)

It started back in the nineties: across the former USSR, state databases began leaking out
piece by piece — passport records, address registries, registration data, telecom operator
databases. Later came an enormous number of leaks from ordinary websites: shops, delivery
services, forums, food delivery apps. And at some point services appeared that search all
of it at once.

In this guide, "probiv" means exactly that — **the practice of looking a person up across
many databases, websites and registries at the same time**. Not a single break-in, but an
established industry that takes one phone number or name of yours and gathers everything
that has ever leaked anywhere or sits in public view.

## Do this today

Four things you can finish in an evening. The explanations come later in this chapter,
but you can start with these.

1. **Look yourself up** by phone number and by email in leak-checking services. You will
find out which databases you are already in — and that tells you what to fix first.
2. **Change any password you have reused.** In Russian leaks the password almost always
sits right next to the login, so one exposed password opens all of your accounts at once.
3. **Turn on login codes** — two-factor authentication — everywhere it is offered. Then a
stolen password alone is no longer enough.
4. **Set up a separate email address** for shops, deliveries and one-off sign-ups. Those are
the databases that leak most often, so let the address that leaks be one that is not tied
to your main accounts.

The rest of this chapter explains why it works this way, and what to do if your data has
already leaked.

## Check what has leaked about you specifically

Start by checking rather than reading: by phone, email or full name you can see which known
leaks you are already in. The services for this, and the risk of each one, are covered in
[Finding yourself in leaks](./breach-detection.md#finding-yourself-in-leaks).

The key point from there: behind any online lookup there may be a wish to enrich your
profile — to record the address your request came from, to link several of your searches
together and work out who you are looking for. So searching the leak files themselves is
safer than using someone else's website, even though it is harder.

## You cannot delete your data from leaks

**You can't.** That is the unpleasant core fact of this chapter, and there is no way around it.

You can ask the popular services to [remove your record](./deleteme.md#removing-information-about-leaks)
from their search, and it is worth doing. But the database itself does not disappear: by the
time a leak becomes public, dozens of people have downloaded it, it has spread to private
services and closed bots, and recalling every copy is impossible. A removal request takes you
out of one window, not out of the data.

There is a theoretical way to get deleted, and it is worth knowing about — if only to see who
it is available to. People with high status, or those serving in the security services, get
themselves removed from search results by pressuring the services that sell those results.
But only people with leverage get deleted that way — and it has an awkward side effect:
**the deletion itself works as a marker.** If a person shows up in one service and is missing
from another, that reveals both which services clean their results and that someone came
looking for that particular person. And complete deletion still does not work: there are too
many databases, and nobody can come to terms with all of them at once.

That is not a reason to do nothing — it is a reason to do something else.

### What works instead of deletion

- **Work out where the leak came from.** Once you know which service gave you away, you stop
feeding it new data, and you also see which of your traces are already linked together.
How to find out — [Determining the source of a leak](./breach-detection.md).
- **Learn about the next leak before everyone else.** This is what canary tokens are for — a
decoy address or a special link that lets you know the moment somebody starts looking for you.
How to set them up — [Canary tokens](./canary-tokens.md).
- **Devalue what has already leaked.** If ten plausible but false or borrowed contacts are
attached to your name in the databases, the price of that record drops.
Techniques — [Making leaks useless](./making-breaches-useless.md).
- **Remove yourself from the services that trade in these databases.** Many of them have a
removal procedure: a form in some cases, a written application with passport details in
others, a paid subscription in a few.
Instructions for specific services and bots — [Removing information about leaks](./deleteme.md#removing-information-about-leaks).

## What usually leaks

It is not only logins and passwords. To show how much wider it goes, we will take one real
database apart field by field, and then look at the rest.

![image](https://user-images.githubusercontent.com/31013580/148645741-47de48bc-af8c-45db-bf1c-3e7004f4ff95.png)

*This is only part of a single database — and hundreds of them have been collected across
all regions of Russia.*

### What one row of a leak looks like

In the abstract, "personal data was leaked" does not sound frightening. So here is the actual
list of fields from one database — the medical lab chain Gemotest, published on 1 May 2022:

```
name · sex · date of birth · place of birth · citizenship
passport · passport issuing authority
birth certificate · certificate issuing authority
SNILS (social security number) / INN (taxpayer number)
insurance policy number · insurance company
address · phone · email
link to a relative · customer number
record created at · record updated at
```

Stop for a second and look at what this set is. A person went in for a blood test — and a
single row ended up holding their **passport**, **birth certificate**, **SNILS**, insurance
policy, citizenship, place of birth, address and phone. That is enough to pass for you in a
conversation with a bank or a mobile operator: these are exactly the details they ask for
when verifying that you are really you.

Two of these fields deserve separate attention.

**The link to a relative.** Your leak automatically becomes a leak about your child or your
parent, even if they never went to that lab themselves.

**The created and updated timestamps.** They show not only what is known about you, but when
you came in — which reconstructs a timeline of your life.

And above all: this is a laboratory. Not a bank, not a government office, not a social
network — a place you visit once to give blood.

### Known major leaks

A few Russian databases that sit in open access. The last column shows the fields, which is
where you see what actually ended up outside.

| When | Source | Records | What was in the fields |
|---|---|---|---|
| July 2021 | Delivery Club | 1.8M | email, name, phone, address, **the network address of the computer** and **exact coordinates of the home** |
| 2022 | CDEK, two different copies | 66.9M and 104.6M | email, name, phone, address, **apartment number**, **the name as registered with the tax service**, record creation time |
| February 2022 | Yandex.Eda | ~7M | names, phones, full delivery address, order comments |
| May 2022 | Gemotest | 31M | the full identity set (see the field breakdown above) **and medical test results** |
| 2023 | Rosreestr (state property register) | 3.0M | name, address, phone, taxpayer number, passport |
| January 2025 | Rosreestr | 25.1M | the same plus email, date of birth, SNILS and **a link to a company** |
| July 2025 | EMIAS, Moscow public health records | about 17 TB | patient data and internal databases |

For scale: the January Rosreestr leak holds 25 million records. As of 2024, about 146 million
people lived in Russia and about 13 million in Moscow. So that one database is twice the size
of the entire population of Moscow.

Three of these fields are worth a closer look, because they change what counts as "personal
data" in the first place.

**Exact coordinates from a food delivery service.** Not a text address that can be written
imprecisely, but a point on the map accurate to the building entrance. Plus, in the same row,
the network address of your computer — so both where you live and where you went online from.

**Apartment number and the tax-registered name from a courier service.** The delivery company
kept not just an address but the apartment, and separately your name exactly as the tax service
records it. That is no longer a contact detail for the courier, that is identification.

**The link to a company at Rosreestr.** A person, their passport, their property and their firm
in one row. For anyone building a dossier this is the most valuable connection of all: it joins
private life to business life.

### Nobody knows how much has leaked in total

This is worth saying plainly, because you will meet the "how much" figure in the news many
times, and it will be different every time.

Even the numbers for **one specific leak** disagree. Rosreestr, January 2025: the intruders
claimed two billion rows, the news reported a published fragment of 82 million, and in the
lookup services that database sits at 25 million records. An eighty-fold spread — for a single
event. CDEK is similar: the news cited 19 and 25 million, while two different copies sit in
open access at 67 and 105 million, labelled as "two versions of the alleged breach" — so even
the fact itself is disputed.

The annual totals disagree just as much. For the same year, 2025, the state regulator counted
slightly over 52 million leaked records, independent researchers put it between 145 and 767
million, and the relevant ministry announced that leaks had dropped thirteen-fold compared to
the year before. The spread between the extremes is more than tenfold, and it is not anyone's
bad faith: the counting methods differ, and above all — **not every leak becomes known**.

There is one practical conclusion, and it is unwelcome: the absence of a news story about a
leak at a service you use tells you nothing about whether your data leaked.

## How this differs between countries

It helps to separate two different things here: how much data has leaked, and how people get
access to it.

### Russia against the global picture

A warning first: **different measurements give opposite answers to the question of where
there is more.**

By one count Russia is first in the world in leaked accounts per person. By another the US is
ahead, and by a wide margin: around 14.6 billion records against Russia's 4.3 billion. France,
which comes first in the first ranking, lands almost six times below Russia in the second.

The contradiction is not anyone's mistake, it comes from **what exactly is being counted**.
These tallies mix very different things: genuine breaches, hand-assembled password lists,
the results of automated collection of public profiles, mailing lists and exports of public
registries. They are not comparable in how dangerous they are, yet they all feed one counter.
On top of that, it reflects the attention of whoever maintains the collection: English-language
databases are gathered more actively.

Hence a conclusion that matters more than any ranking position: **"which country has more
leaks" is a badly posed question.** The answer changes with the counting method. What matters
for you is not your country's rank but which specific databases holding your data sit in open
access — and that is found by searching for yourself, not by reading statistics.

What is visible consistently is the structure, and it differs among neighbours. Russia and
Ukraine both have finance and retail at the top, but Ukraine has **government databases** in
second place and automotive ones in the top five. In Kazakhstan the top spot is shared by
**government databases and education**. Belarus has the smallest collection of all, and it
consists entirely of breaches.

The gap between Russia and its neighbours is enormous, but reading it as "Belarus is a
thousand times safer" would be wrong: a small collection may simply mean the country has had
less attention from the people who assemble these databases.

And one figure that is more useful than any overall ranking: **in Russian leaks there are 89
stolen passwords for every 100 stolen accounts.** The password almost always sits next to the
login — which is why [reusing a password](./password.md) costs more here than it does on
average worldwide.

### Where these services get their data

The pile being searched has two sources.

**State and corporate databases.** The ones that have been leaking since the nineties, and
the ones access to which is sold today — through a person with legitimate rights: an employee
of an operator, a bank, a government agency. Most deals here are not technical attacks but
betrayal: passport details and records from police databases go for **ten dollars a lookup
and up**.

It is telling how the attempt to shut this down ended: the campaign announced in Russia against
the probiv market hit the security officials who were trading in it themselves, while the
sellers moved abroad and carried on from there. The availability of the data did not drop.

**Leaks from ordinary websites.** There are more of these by volume, and they are what gives
lookup services the chains of "phone — email — username — delivery address". One online shop's
database is harmless on its own; ten such databases joined by a shared phone number map out a
decade of your life.

**The country Russia resembles in how this market works is India.** The same thing happens
there: not a break-in, but paid access through an intermediary with legal rights. In one
documented case a company officially authorised to verify citizens' identities let an access
key out, and strangers used it for two years to check other people's documents at six cents a
query — with nobody noticing.

At the same time India is nowhere near Russia in sheer volume — 562 million records against
4.3 billion. Which means **the volume of leaks and the structure of the access market are
independent things**: a country can leak less and still trade access just as freely. You have
to defend against each of them separately.

### What this means in practice

If you are in Russia or another country with a developed probiv market, the "don't give away
your data" defence works less well: the main databases are governmental and banking, and you
are required by law to give your data to them. What remains is the second approach: watch
which of your traces — phone, email, username, address — are linked to each other, and avoid
letting them be glued into a single dossier.

What exactly is for sale in each country, and which documents work as the key to your dossier,
is covered separately:

- [Russia](./russia.md)
- [Ukraine](./ukraine.md)
- [Belarus](./belarus.md)
- [Kazakhstan](./kazakhstan.md)

---

[⬅️ Back](./photo.md) | [⏫ Table of contents](../README.md) | [➡️ Next](./breach-detection.md)
