---
tags: [basics, security, passwords, 2fa]
aliases: [Password Security, Account Safety]
difficulty: 1
---

# Password Security

## The Golden Rules
1. **Never reuse passwords**. If one site is hacked, all your accounts are compromised.
2. **Length beats complexity**. `correct-horse-battery-staple` is better than `Tr0ub4dor&3`.
3. **Use a Password Manager**. Humans cannot remember 50 unique passwords.

## Recommended Password Managers
These tools generate and store complex passwords for you. You only need to remember ONE master password.

- **Bitwarden**: Free, open-source, works on all devices. (Recommended)
- **1Password**: Paid, excellent user experience.
- **KeePassXC**: Free, stores passwords locally on your computer (advanced).

## Two-Factor Authentication (2FA)
Even with a strong password, hackers can steal it. 2FA adds a second lock.
- **SMS Codes**: Better than nothing, but can be intercepted.
- **Authenticator Apps**: Google Authenticator, Authy, or 2FAS. (Recommended)
- **Hardware Keys**: YubiKey. (Most secure, expensive)

> [!WARNING] Phishing Attacks
> Never enter your password or 2FA code on a site you reached via an email link. Always type the website address yourself.

## Micro-Challenge
1. Download **Bitwarden**.
2. Create an account with a strong Master Password (write it down on paper and hide it).
3. Install the browser extension.
4. Enable 2FA on your primary email account using an Authenticator App.

Once done, proceed to [[06-Basic-Troubleshooting|Troubleshooting]].
