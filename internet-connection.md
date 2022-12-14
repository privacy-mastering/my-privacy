---
description: How to secure your Internet connection
---

# 🌐 Internet connection

How the internet does work in short review:

1. You enter the `google.com` into your browser's address bar
2. Your browser sends a request to a DNS server by unprotected protocol
   1. request: `what the IP address for google.com?`
3. And your browser starts a conversation with this IP by unsecured protocol again to exchange security keys
4. After all manipulations your web requests are secured, but.. a person in the middle could simulate a DNS, or you may be worried about your privacy

**How to**

1.  Just use a good VPN service (not free, with a good rating, my choice is ProtonVPN) - it will fully hide all your internet traffic from an observer person;

    For example, I never connect to the Internet in hotels or cafes without a good secure tunnel

    As a good way - use something like [https://www.gl-inet.com/products/gl-usb150/](https://www.gl-inet.com/products/gl-usb150/)
2. If you wanna hide your DNS requests from your provider without VPN - [use DNS over HTTPS](https://developers.cloudflare.com/1.1.1.1/encryption/dns-over-https/encrypted-dns-browsers/)
3. Deny access to your computer via the net, or setup autolocking an account if many unsuccessful tries detected

<mark style="color:red;">**TODO: add manuals here**</mark>
