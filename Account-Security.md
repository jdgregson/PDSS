# Account Security

A properly secured account MUST:
- have a unique, complex password
- have a hardware key set as the primary 2FA authenticator
- have a TOTP-based app set as the backup 2FA authenticator
  * The phone/device with the TOTP app MUST:
    - utilize full disk encryption
    - be protected by a passcode or biometrics
  * The phone/device with the TOTP app SHOULD:
    - have an additional, unique passcode set on the TOTP app

A properly secured account MAY:
- have "backup codes" saved to a secure location (i.e. locked in a safe, stored in an encrypted file)
- have another email address used for password recovery IF that account is also secured by this same standard*

A properly secured account MUST NOT:
- have SMS or phone calls set as a 2FA method
- share a password with another account
- be configured to have passwords expire arbitrarily

*Using email-based 2FA will not protect against nation-states, since, for example, all of Gmail is already being piped through the NSA's various programs.
