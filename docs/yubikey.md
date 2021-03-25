# Using your YubiKey

The YubiKey that the company provides employees with is known as a **hardware security token**.
It functions as a portable security processor and is able to handle storage of cryptographic secrets.

# What can the YubiKey be used for?

## Two Factor Authentication

There are two main mechanisms that the Yubikey offers to support 2FA.

- OTP - One Time Password
- U2F - Universal 2 Factor

U2F is the recommended two factor method. It is phishing resistant unlike
TOTP/Google Authenticator. It is much harder to compromise than SMS/Voice call
methods.

The instructions below are specific to provider, but they are all similar
enough.

### GitHub

1. Go to your [GitHub Security Settings](https://github.com/settings/security)
2. Turn on `Two-factor Authentication` if it's not already enabled. You will
   need to set up either an SMS or TOTP (Google Authenticator) if it's not.
3. Under `Security keys, choose `Register new device`
4. Type in a name: `yourname-yubikey-nano4` or something else that will help
   you remember the key
5. Click `Add`
6. Follow the instructions on screen - you'll probably need to tap the YubiKey
   for it to register.

Yubico has more [detailed instructions](https://www.yubico.com/support/knowledge-base/categories/articles/use-yubikey-github/).

### Google

1. Go to your [Google Sign-in & Security page](https://myaccount.google.com/security)
2. Click `Two-step verification` and you may be prompted for your password.
3. Click `Add Security Key` and follow the on-screen instructions. You may
   need to tap or touch your YubiKey.

Yubico has a [video](https://www.yubico.com/why-yubico/for-individuals/gmail-for-individuals/)

### LastPass

LastPass supports OTP and TOTP as a two factor method and does not
support U2F.

1. Go to your [LastPass account details](https://)
2. Click `Two-step verification` and you may be prompted for your password.
3. Click `Enable MFA` and follow the on-screen instructions. When prompted, touch the Yubikey to generate a one-time password.

Yubico has a [video](https://www.yubico.com/gb/works-with-yubikey/catalog/lastpass-premium-and-families/).

## Securely exchanging secrets

