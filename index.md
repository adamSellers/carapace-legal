# Carapace Privacy Policy

**Effective date:** February 21, 2026  
**Last updated:** February 21, 2026

Carapace is a local companion app for securely preparing encrypted payloads for use with Open Claw hosts.

## 1. Summary

Carapace is designed to process sensitive values on your device.

- No account required
- No backend service operated by Carapace
- No cloud sync operated by Carapace
- No Firebase
- No in-app analytics or ad tracking SDKs

## 2. Information We Process

Carapace may process the following data you provide:

- Open Claw public key (entered manually, scanned from QR, or imported from a photo)
- Secret value (for example: API keys, tokens, passwords, or other sensitive strings)

This processing is used only to generate an encrypted payload on-device.

## 3. How Your Data Is Used

Carapace uses your inputs to:

1. Parse and validate the Open Claw public key
2. Encrypt your secret locally using Libsodium sealed-box cryptography
3. Copy the encrypted payload to your clipboard for you to send through your chosen channel

Carapace does **not** send these values to a Carapace server because Carapace does not operate one for this workflow.

## 4. Permissions

Carapace may request:

- **Camera** permission: to scan QR codes containing an Open Claw public key
- **Photo Library** permission: to import QR code screenshots/photos

You can deny or revoke these permissions in iOS Settings.

## 5. Network Activity

For the core encryption flow, Carapace performs local processing and does not require a backend service.

If your device, OS, or third-party infrastructure performs independent network behavior outside Carapace (for example, app store, OS services, or user actions in other apps), that is not controlled by Carapace.

## 6. Data Storage and Retention

Carapace is intended to be minimal and local-first.

- Secret values are processed in-memory for encryption
- Encrypted output is copied to clipboard on your request
- Carapace does not intentionally store your plaintext secrets in a remote service

You are responsible for handling copied payloads and clipboard contents according to your own security requirements.

## 7. Third-Party Components

Carapace uses open-source libraries for local cryptography and QR processing (for example, Libsodium bindings and QR scanning/image parsing libraries). These components are used for on-device functionality.

## 8. Open Claw Host Responsibility

Decryption and secret storage happen on your Open Claw host environment, not in Carapace. The privacy and security posture of that host, its runtime, and any messaging channel you use are your responsibility.

## 9. Children’s Privacy

Carapace is not directed to children under 13, and we do not knowingly collect personal data from children.

## 10. Changes to This Policy

We may update this policy from time to time. Updates will be reflected by revising the “Last updated” date.

## 11. Contact

If you have privacy questions, contact: **carapace@sellers.life**
