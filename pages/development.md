# Privacy for software developers

## Exposure of your personal/working email address

When working with program code and version control systems such as git, there is a risk of exposure
your personal mailbox. This often happens when working with personal/work projects
on the same device at the same time.

To avoid this, check that the global git settings are correct or the settings in the directory of the specific repository are set:
```
git config --global user.name
git config --global user.email
``` 

GitHub provides the ability to hide your email from the interface and block the "leakage" of the main mailbox associated with the account:

![Email adresses privacy settings in GitHub](../img/gh_emails.png)

*The section will be updated*

---

[⬅️ Back](./instagram.md) | [⏫ Table of contents](../README.md) | [➡️ Next](./2fa.md)
