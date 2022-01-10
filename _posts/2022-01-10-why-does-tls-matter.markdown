---
title: Why does TLS matter?
date: 2022-01-10 06:32:00 Z
categories:
- cybersecurity
- privacy
- encryption
---

When browsing the internet or using a website, you should always make sure that your connection to the website is encrypted via TLS, mostly referred to as HTTPS, so no one can see exactly what you’re doing.

TLS stands for Transport Layer Security, but we find that it’s mostly referred to as transport encryption. HTTP stands for Hypertext Transfer Protocol, and is displayed in all website URLs before the domain name. For example, **http**://duckduckgo.com. When transport encryption is being utilized, **https://** is displayed before a website domain name rather than **http://** The **S** simply stands for secure, because your connection to the website is now secure as it is encrypted.

When you’re not utilizing TLS aka HTTPS when connected to a website, all information/data that you send and receive from that website is transmitted in plaintext. This means hackers, an everyday citizen that knows a bit about cybersecurity, your ISP, and more, can all easily see all of the information you are sending and receiving, all in plaintext. This means they can see your username(s), password(s), credit card details (depending on the unencrypted website which you are using), and much more.

When you are utiziling TLS aka HTTPS - your connection to x website, as mentioned, is encrypted. This means hackers and your ISP, when inspecting web traffic, will just see a bunch of random gibberish (random letters, numbers, symbols, etc) rather than your information/data in plaintext. As the name suggests, transport encryption ensures that your data when leaving your network is encrypted and remains encrypted while in transport, and is then decrypted at the destination website or service.

Fortunately nowadays, many browsers attempt to force an encrypted connection to websites when possible, but not all browsers do this, and not all websites support TLS. If a website you are visiting/using does not support TLS (indicated by whether or not the lock icon in your browser is green), you should not be using that website as it is considered to be dangerous. HTTPS Everywhere is a browser addon created by EFF (Electronic Frontier Foundation) that ensures you are always connected to websites using HTTPS aka TLS, if your browser does not enforce HTTPS connections. Please note that EFF is planning on deprecating the HTTPS Everywhere browser addon some time in 2022 as more and more browsers are beginning to enforce HTTPS connections.