---
title: "Private internets"
date: 2023-05-23
draft: false
---

I'm not a networking person. I can to grasp the most critical parts on a
conceptual level, and I'm able to copy and paste a CIDR block in some Terraform
code, but it's not an area I've worked a lot in.

But, as a part of [studying](/posts/security-plus/), I needed to refresh some
foundational knowledge. And suddenly I found myself reading [RFC 1918 Address
Allocation for Private Internets](https://www.rfc-editor.org/rfc/rfc1918.html)
with my morning coffee. Just the title is intriguing on its own, I wish we
talked more about internets in plural. Maybe that terminology is on its way
back?

Older internet documents tend to have a nice tone to it:

_The Internet has grown beyond anyone's expectations. Sustained
   exponential growth continues to introduce new challenges._

And in section 3 the private address space is defined:

   The Internet Assigned Numbers Authority (IANA) has reserved the
   following three blocks of the IP address space for private internets:

     10.0.0.0        -   10.255.255.255  (10/8 prefix)
     172.16.0.0      -   172.31.255.255  (172.16/12 prefix)
     192.168.0.0     -   192.168.255.255 (192.168/16 prefix)
