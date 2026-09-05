# Photo

Unfortunately, photos (and any images in general) have long been easily recognized and indexed content.
Search engines can search for similar photos, distinguish text, objects, and specific people on them. Social
networks can recognize you in an arbitrary photo and put a mark there with a link to you even without your knowledge.

But, fortunately, in recent years, the trend towards privacy has intensified, and therefore social networks are introducing reasonable restrictions
on recognizing people. General-purpose search engines refuse to do exact face search too: Google does not look up
people by face as a matter of policy, and while Yandex searches for similar images and in practice often does find
the person, it has no dedicated "search by face" feature. This reduces the likelihood of
malicious use of such functions, but does not prevent the use of such technologies in general.
Now recognition tools can be easily created independently or use freemium alternatives.

*The section will be updated*

## How to test yourself

In the post-Soviet space, you can still use [Yandex](https://images.yandex.ru/).
But it alone is not enough: below are the services that search for faces specifically, not for similar pictures.

If you have actively used social networks, you can find not only your account, but also photos with your face
in the accounts of your friends, acquaintances or other people who are not even related to you. Of course,
it is extremely difficult to delete such photos, and if you do not want them to link to you, then you should competently [delete account](./deleteme.md).

<img width="1123" alt="image" src="https://user-images.githubusercontent.com/31013580/193446993-ae071840-49f2-45f3-b517-6b1e2a97a510.png">

### Specialized face search engines

The niche abandoned by general-purpose search engines has been taken over by dedicated services. By definition
they have no restrictions on searching for people — that is their entire point. It is worth checking yourself
with each of them: their indexes are different, and an empty result in one says nothing about the others.

- [Search4Faces](https://search4faces.com/) — **free, no registration needed** (only its API is paid).
Searches avatars and profile photos from VKontakte, Odnoklassniki, TikTok and Clubhouse — that is, exactly
where PimEyes and FaceCheck.ID do not look. Its databases are outdated, most of the data was collected in 2022
or earlier, and this cuts both ways: an avatar you changed ages ago is still sitting there, but an empty result
today does not mean you are not in it. The database is incomplete, and for an unfamiliar face the service often
just returns people who happen to look alike.
- [VK.watch](https://vk.watch/) — a VKontakte archive: profiles, their edits, friends, photos and comments,
including the ones you deleted long ago. It has face search too, as a separate button. That is exactly what
makes the service unpleasant: deleting a photo on VKontakte does not remove it from an archive made earlier.
Access is by paid subscription, and according to its own FAQ its subscribers include lawyers, recruiters
and private detectives.
- [Geometria](https://srl.geometria.ru/) — search over an archive of event photo reports: clubs, parties,
city events. You upload a selfie and find yourself in other people's shots from events you simply attended
without giving the photographer a thought. Face recognition is paid.
- [PimEyes](https://pimeyes.com/) — indexes the open web: news sites, blogs, stock photo banks, forums.
A free search will show you that matches exist, but the previews will be blurred; unblurred images and links
to the source pages are available by subscription.
- [FaceCheck.ID](https://facecheck.id/) — positions itself as an "is this person a scammer" check, indexes
social networks, police photos and public registries. The service shows its counter of indexed faces right
on the front page: at the time of writing it is over 1.4 billion.

The last two find you where Yandex and the Russian archives do not reach: in other people's photo reports,
on a conference website, in a sports club gallery, in a group photo from work.

And something common to all of them: by checking yourself you upload your face to a face search engine.
It is a sensible trade — you learn what is already known about you — but it is still a trade.

## How to remove yourself from face search engines

The terms vary a lot: from free removal by selfie in a minute to an email to an anonymous owner at gmail.
And one service offers no such option at all.

**FaceCheck.ID.** Removal is free and, according to the service, instant: find yourself by searching with your
own photo, mark your shots on the [Remove My Photos](https://facecheck.id/en/RemoveMyPhotos) page and confirm
your identity with a selfie right in the browser.

**PimEyes.** The [opt-out form](https://pimeyes.com/en/opt-out) requires several photos of your face from
different angles and a scan of your passport or ID. That is, to stop being found by your face you have to hand
the service additional photos of your face and a document. They ask you to anonymize the scan by covering
everything unnecessary, but whether the trade is worth it is still yours to decide.

**Geometria.** Here the path is lawful but paper-based: the operator is a Russian legal entity, OOO Geopromedia,
and you can withdraw your consent to data processing by sending a scan of a written application to law@geo.pro,
or the original by registered mail. Withdrawal deletes your account and the records containing your personal
data, but not the photos themselves: they stay in the reports, and under the agreement the administration
removes content solely at its own discretion.

**Search4Faces.** There is no form, but there is an email: the service states outright that you can request
removal of your images from search results by writing to search4faces@gmail.com, and promises to reply within
24 hours. There are no guarantees beyond that promise — who owns the service is unknown, its domain is
registered through a Bahamas-based privacy registrar, and the correspondence goes through an ordinary
gmail mailbox.

**VK.watch.** The service does have a privacy policy, and it even describes the right to request deletion
of your data by writing to support@vk.watch. But it is worth reading carefully: it describes subscriber
data — email, billing details, technical logs, search history. Archived VKontakte profiles are not in the
list of collected data at all, and there is no obligation to remove you from the archive either. The right
to deletion here belongs to the one who searches, not to the one who is found.

Prevention is more reliable than any email anyway: the archive keeps the snapshot that was taken when it was
collected, and changing your avatar after the fact is useless — that is the whole point of an archive.

The main thing: removal from an index does not remove the photo itself. It stays where it was — in someone
else's album, on an event website, in a news story — and the next service will index it again. Only removing
the original source works reliably: [delete your account](./deleteme.md) or ask the site owner to take the
photo down.

And these services are not all of them, only the ones visible from the outside. Clearview AI, for example,
builds a similar index but sells access only to government customers, and there is no way to check yourself
in it. There are other closed services that search an index of photos from social networks and even from
messengers popular in particular countries — WhatsApp, Telegram and others. And there your profile photo is
open by default: it is visible to anyone who came across your account in a shared group or found you by phone
number, so [closing it in the privacy settings](./telegram.md) is worth doing not only against people you know.

## Face photo as biometrics

*The section will be updated*

### Cloaking

To combat the tools for recognizing people in images, so-called cloaking is used.
The essence of the method is to distort the photo in such a way that visually we perceive it as the original,
but the programs did not see a person or a face there.

Methods for distortion can be both manual (blurring / retouching / distortion of individual parts of the photo) and automatic.
Of the latter, special programs that use face recognition algorithms in the opposite direction can be noted,
modifying the photo so that the search is not possible. An example of such a program: [Fawkes](https://github.com/Shawn-Shan/fawkes).

Of course, such post-processing of photos or videos will not help proactively. To make it difficult to recognize faces with "smart cameras" in
real life, original and not very good ways are invented, examples can be read from the links at the end of the page.

## Photo metadata

*The section will be updated*

## Materials used and useful links

- [Big Brother is (so far) blind](https://habr.com/ru/post/586094/)
- [King's new makeup](https://telegra.ph/Novyj-makiyazh-korolya-07-14)
---

[⬅️ Back](./password.md) | [⏫ Table of contents](../README.md) | [➡️ Next](./breaches.md)
