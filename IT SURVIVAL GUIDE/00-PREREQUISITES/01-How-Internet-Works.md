---
tags: [prerequisite, networking, internet]
aliases: [Internet Basics, Networking Fundamentals]
difficulty: 2
---

# How the Internet Works

## The Big Picture
The internet is simply a network of computers talking to each other. That is it. No magic.

## Key Concepts

### IP Address
Every device connected to the internet has a unique number called an **IP Address** (e.g., `192.168.1.1` or `2001:db8::1`).
- Think of it like your home address. Mail cannot be delivered without it.
- **IPv4**: Older format (running out of numbers).
- **IPv6**: Newer format (almost infinite numbers).

### DNS (Domain Name System)
Humans are bad at remembering numbers like `142.250.190.46`. We prefer names like `google.com`.
- **DNS** is the phonebook of the internet. It translates `google.com` to `142.250.190.46`.
- When you type a URL, your computer asks a DNS server: "What is the IP for this name?"

### HTTP/HTTPS
This is the language browsers and servers use to talk.
- **HTTP**: Hypertext Transfer Protocol. Unencrypted.
- **HTTPS**: Secure version. Encrypted. Always look for the lock icon in your browser.

### Client vs Server
- **Client**: Your computer/phone asking for data (e.g., "Show me this webpage").
- **Server**: A powerful computer always connected to the internet that sends data back.

### Packets
Data is not sent as one big file. It is chopped into tiny pieces called **packets**.
- Each packet travels independently.
- They reassemble at the destination.
- If one gets lost, only that small piece is resent.

## Visual Analogy

```text
[YOU] --(Request)--> [DNS Server] --(IP Address)--> [YOU]
  |
  +--(Request Packet)--> [Router] --> [Internet] --> [Server]
                                                          |
[YOU] <--(Response Packet) <-- [Router] <-- [Internet] <--+
```

## Micro-Challenge
1. Open your terminal (Command Prompt on Windows, Terminal on Mac/Linux).
2. Type `ping google.com`.
3. Watch your computer send packets to Google's server and get a reply.
4. Type `nslookup google.com` to see its IP address.

> [!TIP] Understanding Errors
> - "DNS_PROBE_FINISHED_NXDOMAIN": The phonebook couldn't find the name.
> - "Connection Timed Out": The server didn't answer.
> - "404 Not Found": The server answered, but the specific page doesn't exist.
