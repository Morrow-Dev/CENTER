# Security policy

## Reporting a security problem

Please report security problems in CENTER privately, never in a public issue or discussion:

- on GitHub: **[Report a vulnerability](https://github.com/Morrow-Dev/CENTER/security/advisories/new)** (this
  repository's **Security** tab, GitHub's private vulnerability reporting), or
- by email: **morrow.devlab@gmail.com**

Please include what you found, the CENTER version, your Windows version, and the steps that show the problem. The fix
ships as a normal CENTER update; please give it time to reach everyone before you talk about the problem publicly.

## Supported versions

Only the newest CENTER release gets fixes. Installed copies keep themselves up to date: CENTER looks for a new version
when it opens and every hour, and starts it the next time it is opened.

## How downloads and updates are protected

- Every update is signed with CENTER's release key. An installed CENTER checks the signature and the exact contents of
  every update before it uses it, and never goes back to an older version.
- Every release lists the SHA-256 of its installer in its notes and in its **SHA256SUMS** file. To check a download,
  run `Get-FileHash .\CENTER-Setup.exe` in PowerShell, in the folder you downloaded it to: the hash it prints must
  be exactly the one on the release's page.
