---
description: PGP, disposable emails
---

# 👾 Emails encryption

What will happen if somebody (an attacker) receives access to your emails?

Answers:

1. Your online-social profiles are compromised – ok, not very good, but maybe it's not critical
2. In the usual case, the attacker may restore access to a lot of online services, like – bookings, rentals, online subscriptions, etc... Maybe it's ok still – you may just block your banking cards and continue live (if disclosed information is not a big secret)
3. But what about medical and governmental services? For someone disclosure, a piece of relevant information is a very sensitive action, for example, – visits to a phycologist or results of an analysis. Already warmer?
4. Bank and online exchange services – your bank statements, individual payments info, accounts info, balances, and all historical data are accessible to everyone who has access to your emails – it's very critical for someone, and I know it. Because sometimes it's enough to restore/receive full access to your money
5. Emails with your documents – some of you send/receive identity documents by email or just save them in the mailbox (like a draft) just in case, yeah?

If you say me "I am protected by 2FA" – please, stop it

This document is about a case when somebody already received access to your mailbox, and the way of attack is not important (unencrypted storage, stolen devices/cookies/session, phishing emails, 2FA bombing, device sharing, fake sim card, MitM, platform vulnerabilities, insider intrusion, shoulder observation, etc... there are many ways)

Let's talk about how to protect the content of your emails when somebody has access to your mailbox **already**

#### Encryption incoming emails

In a common case, any online service sends you emails as is – anyone may read your inbox

Many email clients support [PGP-encrypted](https://www.openpgp.org/) emails, and below is my easiest description of how to do it even if online service does not support PGP encryption

1. Register here [https://app.simplelogin.io](https://app.simplelogin.io/dashboard/)
   1. Add your main email here [https://app.simplelogin.io/dashboard/mailbox](https://app.simplelogin.io/dashboard/mailbox)
   2.  Go to the email edit page and turn on PGP\


       <figure><img src="../.gitbook/assets/image (10).png" alt=""><figcaption><p>As you can see – you have to add your public key, read below how to do it</p></figcaption></figure>

       Ok, now you have the email relay service, that supports encryption, but you do not have PGP keys!
2.  Install [the mailvelope.com](https://mailvelope.com/en) browser extension and open the key management page\


    <figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption><p>It is your web browser still, but the extension may work online and helps to decrypt emails</p></figcaption></figure>

    1.  Enter your email address (that waits for the PGP key on the SimpleLogin page)\


        <figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption><p>your password maybe not be very hard, seriously, but I recommend using a password manager</p></figcaption></figure>
    2.  Press ok, open the data of your new key, and press export to receive your public key\


        <figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>
3. Immediately this public key is a key that is required by SimpleLogin, just past it there and press save

So, now you may generate a new email-relay address and use it for service, the letters from the one you want to encrypt

Mailvelope helps to decrypt letters automatically

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption><p>Bank -> SimpleLogin -> Encrypts emails -> your gmail inbox</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption><p>Mailvelope (or k9mail/thunderbird) -> decrypts email content by your local key</p></figcaption></figure>

If you wanna save the possibility to read letters from mobile phones I may recommend [https://k9mail.app/](https://k9mail.app/) for Android users ([K-9 Mail is now part of the Thunderbird family](https://k9mail.app/2022/06/13/K-9-Mail-and-Thunderbird.html)[)](https://k9mail.app/2022/06/13/K-9-Mail-and-Thunderbird.html)

For desktop users, a good variant – thunderbird.net, just import your private key to the settings

Other applications you may find here [https://www.openpgp.org/software/](https://www.openpgp.org/software/)

**Just remember:**

1. If you lost your private key – all your emails are useless trash, and there is no way to decrypt them
2. If you forget your passphrase – the same result
3. So – you must save your keys and passphrase in a password manager or somewhere else (but not on paper under the keyboard, please)

There is an interesting possibility provided by the proton.me email clients (web/mobiles) – you already have a public key, and you haven't set it up in SimpleLogin, but... if somebody will receive access to your mailbox via login/pass/2fa – anyway all your emails are still in a readable format (except the keys when you switched on [two-password mode](https://proton.me/support/single-password))

So, I just showed a comfortable way for most of us I believe you will encrypt only the most important emails, to check them from protected devices For other services, a basic forwarding is enough

#### Outgoing emails

Sometimes you need to send secret info or documents by email

Most typical users just attach documents or secrets to the letter and that's all

But maybe the receiver does not think about security like you, so how to protect your data:

1. You may use a "Confidential emails" mode in Gmail with an expiration period, at least the letter will be deleted automatically in a few days, read more here [https://support.google.com/mail/answer/7674059?hl=en#zippy=%2Cim-using-another-email-account%2Cim-using-a-gmail-account](https://support.google.com/mail/answer/7674059?hl=en#zippy=%2Cim-using-another-email-account%2Cim-using-a-gmail-account)
2. Do not attach documents to emails, how to:
   1. Compress documents to archive with encryption, read more here [https://www.technewstoday.com/password-protect-a-zip-file/](https://www.technewstoday.com/password-protect-a-zip-file/)
   2. Upload this document to google drive and get a link to share
   3. Insert to email link to the document and the password (or pass the password by phone)
   4. Add to a calendar notification, that you have to close access to the document by link
3. And a very good choice - protom.me
   1. There are possible to create a password-protected email [https://proton.me/support/password-protected-emails](https://proton.me/support/password-protected-emails)
   2. Or email with expiration [https://proton.me/support/expiration](https://proton.me/support/expiration)
   3. Or use proton drive for files with pass/expiration date [https://proton.me/blog/file-sharing-proton-drive](https://proton.me/blog/file-sharing-proton-drive)
4. As well I have to mention the 1password possibility to share data for the first access only – after file downloading link fill expire automatically, it's a very good feature
