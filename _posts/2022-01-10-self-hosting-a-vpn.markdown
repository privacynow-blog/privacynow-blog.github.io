---
title: Self-hosting a VPN
date: 2022-01-10 06:32:00 Z
categories:
- privacy
---

Choosing a VPN provider can be difficult at times, especially if you are on a budget or are still concerned about whether or not the VPN logs your activity or not. Fortunately, open source software allows you to host your own VPN server on a machine. Please only follow this simple guide if you have a decent amount of Linux knowledge and know what you’re doing, otherwise very bad things could happen and you’d be better off using a 3rd party privacy-respecting VPN provider like Mullvad.

We will be using the WireGuard software for this demonstration. WireGuard® is an extremely simple yet fast and modern VPN that utilizes state-of-the-art cryptography. It aims to be faster, simpler, leaner, and more useful than IPsec, while avoiding the massive headache. It intends to be considerably more performant than OpenVPN. WireGuard is designed as a general purpose VPN for running on embedded interfaces and super computers alike, fit for many different circumstances. Initially released for the Linux kernel, it is now cross-platform (Windows, macOS, BSD, iOS, Android) and widely deployable. It is currently under heavy development, but already it might be regarded as the most secure, easiest to use, and simplest VPN solution in the industry. (credit: wireguard.com)

WireGuard supports Ubuntu, Debian, Fedora, and more, but we’ll be using Ubuntu for the WireGuard VPN Server. First, you will need to choose a trustworthy, secure, and privacy-respecting VPS provider to host this VPN on. We’ll save you some time so you don’t need to go looking for one of those, we have multiple privacy-respecting, secure, and trustworthy VPS providers listed here -> [https://swivro.net/hosting-providers.html](https://swivro.net/hosting-providers.html)

Once you purchase your VPS, you’ll want to select Ubuntu 20.04 LTS (or Debian >= 10) as the Operating System. After the Operating System has been installed, you should be provided with SSH credentials so you can access your server. We suggest using PuTTY as an SSH Client as it is free and open source. Now that you’re logged in to SSH, if you’re not logged in as root, you should type `sudo su` and click enter. To easily install WireGuard, we’ll be using a 3rd party script called wire-guard install which is open source and is available on GitHub. Begin the installation process by copy and pasting the following 3 commands.

    curl -O https://raw.githubusercontent.com/angristan/wireguard-install/master/wireguard-install.sh
    chmod +x wireguard-install.sh
    ./wireguard-install.sh

After entering that last command, you will be prompted with some questions. Click enter on all of them (unless you want to change something) to select all of the default options.

A private key file should have now been saved, and a QR code should be displayed. Take that private key and import it to your WireGuard client and voilà. If you have WireGuard on mobile (Android/iOS), you can scan the QR code that is displayed in your SSH session, using your WireGuard app and your phone camera. You now have your own self-hosted VPN.

Thanks for reading!