---
description: >-
  Two-factor authentication (2FA) is a security method that requires two forms
  of identification to access resources and data.
---

# 🔑 2FA

**Motivation**

Even if somebody knows your login/password pair – 2FA protects your data, because it's more difficult to stole 2FA factor

What is 2FA? In most cases, it is just OTP (One Time Password) that depends on a shared secret (that is known for server and clients) and a current time; all generated OTP may be applied only during a restricted time

For example

| Method                       | Description                                                                                                                                                                                                                                                                        |
| ---------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `SMS`                        | when a server sends OTP by a shared "secret" (phone number), it is not a very good way, just because somebody may steal your phone and view the content of the SMS on a locked screen                                                                                              |
| `Email`                      | like SMS, but less secure, and the content may be viewed on a locked screen, and your email may be hacked easily                                                                                                                                                                   |
| `OTP Applications`           | perfect choice for most people, for example, [https://googleauthenticator.net/](https://googleauthenticator.net/) or [https://authy.com/](https://authy.com/); it's impossible to catch OTP because there is no sending, and it's not possible to view the code on a locked screen |
| `U2F (Universal 2nd Factor)` | something more difficult than OTP, usually it is a unique cryptography module in a dedicated device like yubico or a chip in your phone/laptop                                                                                                                                     |

**How to**

In a common way, you have to search for "`<name of your website> + 2FA`" and follow the instructions

But I'll try to help you with the most popular services

Install any application that supports OTP

1. [https://googleauthenticator.net/](https://googleauthenticator.net/)
2. [https://authy.com/](https://authy.com/)
3. Or a Password Manager, [read more here](passwords.md)&#x20;

**Example via Google**

1. Go to [https://myaccount.google.com/signinoptions/two-step-verification](https://myaccount.google.com/signinoptions/two-step-verification)
2. Click "Authenticator app"
3. Follow the instructions, scan the QR code, and backup "Backup codes"

That's all, seriously!&#x20;

Your account is very protected now

Research more possibilities on this page and think about one – what will you do when you lost 2FA? Make all possible backups! Add more devices as 2FA

**Other useful links for popular services**

* Facebook [https://www.facebook.com/settings?tab=security ](https://www.facebook.com/settings?tab=security)
* Instagram [https://www.instagram.com/accounts/two\_factor\_authentication/](https://www.instagram.com/accounts/two\_factor\_authentication/)
* Twitter [https://twitter.com/settings/account/login\_verification ](https://twitter.com/settings/account/login\_verification)
* Proton [https://account.proton.me/u/2/mail/account-password](https://account.proton.me/u/2/mail/account-password)







