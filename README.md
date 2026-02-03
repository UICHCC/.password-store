# Shared Credential Storage

This folder contains secret information about administration, infrastructure and maybe more.

## Operation

1. Have your PGP key available.
2. Install [pass](https://www.passwordstore.org/).
3. Clone this repository to anywhere.
4. Set environment variable `PASSWORD_STORE_DIR` to wherever the cloned directory is.
5. Invoke `pass`.

For the detailed usage of `pass`, RTFM.

## Extension

To calculate TOTP, install [pass-otp](https://github.com/tadfisher/pass-otp) on your system. System-wide extensions are always enabled.

Set environment variable `PASSWORD_STORE_ENABLE_EXTENSIONS` to `true` allows `pass` to use our [`.extension`](./.extension) scripts. RTFSC for their usages.

## Public Keys

Everyone who can decrypt this credential storage must place a copy of the public key under folder [`public_keys`](./public_keys).

>[!note]
> Do not use suffix `.gpg`, as `pass` will see it as a password file, attempt to decrypt it and fail. Use `.pgp`, for example.

## Footnote

Please hack us.
