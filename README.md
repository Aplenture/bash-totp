This will be a basic OTP manager in pure bash (no external programs ever)

Put in your secrets, encrypt with a key, and then come back and
generate your OTPs

This script is a fork from Scott Nicholas' bash-totp. For more informations see https://github.com/neutronscott/bash-totp.

## Commands
### help
Lists all possible commands. There are no arguments.

### add
Adds a new token. Arguments:
- issuer (required): name to identify the token
- key (required): secret of token
- hash (optional, default: sha1): used hash algorithm
- step (optional, default: 30): timeframe of valid passwords in seconds
- digits (opitonal, default: 6): number of digits of generated passwords

### get
Returns the current passwords of tokens. When issuer is set, tokens are filterd by it. Arguments:
- issuer (optional): filters tokens by issuer

## Supported Hash algorithm
- sha1
- sha1o
- sha256
- sha512