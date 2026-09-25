## Overview

This document is an accessible starting point for using Aenigma. It briefly and concisely
describes the problems this project aims to solve. By the end, even users unfamiliar with
technology will have a general picture of how to set up their own encrypted communication
system on their personal devices.

### Something familiar? Or just something from old stories?

Before electronic means of communication, people used letters. A sheet of paper with a
message written on it was then folded into an envelope. For the message to reach its
recipient, the envelope had to have the recipient's address written on it. And let's not
forget that, to receive a reply, we also had to write our own address on the back of the
envelope. We sealed the envelope carefully and then handed it to the nearest post office.
Step by step, passing through multiple post offices and sorting centers, our message
reached its recipient.

### The digital equivalent

Aenigma works like the postal service (or a courier service). It takes an *"envelope"* and
delivers it to an *"address"*. What it can do beyond the national postal service, however,
is move the post office into your personal computer. The message written on paper becomes
a string of bits. The envelope is replaced by encryption. Addresses become internet
addresses. Post offices and sorting centers are replaced by servers.

### Anonymity? Back to the post office.

Let's suppose two friends want to communicate while keeping their identities unknown. In
the original postal example, this is impossible. Both addresses are in plain sight. There
is, however, a small trick that can be used to mislead the postal service. Let's suppose
these two enthusiasts have three other friends willing to help. That makes five in total.
The message has to get from friend 1 to friend 5.

Friend 1 writes the message, puts it in an envelope, and writes friend 5's address on it.
Then they put that envelope inside a second envelope addressed to friend 4, which goes
inside another envelope addressed to friend 3, which goes inside yet another envelope
addressed to friend 2. This last envelope is delivered by mail to friend 2, who opens it.
Inside is the envelope addressed to friend 3. Friend 3 receives it, opens it, and finds
the envelope addressed to friend 4. Friend 4, upon receiving it, opens it and finds the
original envelope addressed to friend 5, the final destination.

The exception that immediately stands out is that the friends no longer write their own
address on the envelopes. The message can no longer be returned if one of the addresses
cannot be found. However, friend 1, who wrote the original message, will make sure to
mention in the letter to friend 5:

> *"...please reply to me at address X.*
>
> *Warmly,*
>
> *Friend 1."*

Friend 5 will do the same, in reverse, to communicate with friend 1.

Aenigma is the digital equivalent of this trick. Each friend has a personal computer
connected to the others. The message is protected by successive layers of encryption that
are removed one by one as the message travels, step by step, toward its final recipient.
Note that in this arrangement, nobody knows who wrote the message or who read it, except
for the friends who agreed to pull off this trick together.

### The goal?

The immediate goal of this project is to offer an independent alternative for private
communication. There are certainly other alternatives, at least as ambitious and
trustworthy. What Aenigma aims to achieve, however, is a democratization of
communication: putting into the hands of those with limited resources the ability to
communicate without restrictions, uncensored, and free from commercial imperatives.

### How does it work?

Aenigma is available on
[Google Play](https://play.google.com/store/apps/details?id=ro.aenigma).
For devices without Google Services, you can use this
[link](https://github.com/m3sserschmitt/aenigma-android/releases/latest/download/aenigma.apk).
The app comes with a public server (or several, depending on available resources) that it
connects to initially. *"Public"* does not imply any compromise in terms of security. It
simply means it is freely available to everyone. You can also host your own Aenigma
server using your own equipment at home: a regular personal computer and an internet
connection that is as stable as possible will be enough. Various action groups may find
this second option more convenient.

<a href="https://play.google.com/store/apps/details?id=ro.aenigma">
<img alt="Get it on Google Play"
src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png"
width="150">
</a>

Next, follow the series of quick guides to get familiar with the app:

1. [Aenigma Mobile App User Guide](https://web.aenigma.ro/#/blog/article?url=https%3A%2F%2Farticles.aenigma.ro%2Fuser-guide%2Fquick-start-mobile-app-ro.md)
2. [Host Your Own Aenigma Server](https://web.aenigma.ro/#/blog/article?url=https%3A%2F%2Farticles.aenigma.ro%2Fuser-guide%2Fhost-server-ro.md)

### Contact

You can report bugs or suggest improvements at
[contact@aenigma.ro](mailto:contact@aenigma.ro)

---

*This document is licensed under
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).*
