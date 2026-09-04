# Security Policy

## Supported version

Only the latest GitHub Release is considered for public-preview security reports. TAIL is early-stage preview software and is not approved for real-money use.

## Do not disclose secrets publicly

Do not include private keys, seed phrases, access tokens, cookies, account identifiers, balances, transaction history, production URLs or exploitable sensitive details in a public Issue.

If the repository Security page offers **Report a vulnerability**, use that private GitHub channel. No separate confidential contact address is currently published. If private reporting is unavailable, open only a minimal non-sensitive Issue asking the maintainer to enable a private channel.

## Scope

Useful reports include:

- the public preview unexpectedly enabling signing, broadcast or order execution;
- loopback API exposure outside the local machine;
- browser policy bypasses to local/private networks or credential-bearing URLs;
- secrets, private paths, wallet addresses or source maps present in a Release asset;
- unsafe handling of imported backgrounds or assistant assets;
- installer or update integrity problems.

## Out of scope

- profitability or investment performance;
- missing live data in the intentionally offline preview;
- private systems or repositories not distributed through this public project;
- social engineering, denial-of-service against third parties or testing with real funds.

TAIL provides no bug bounty at this stage. Do not test against accounts, wallets or infrastructure you do not own or have explicit permission to assess.
