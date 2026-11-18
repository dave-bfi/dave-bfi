# ai-knowledge onboarding (public, no credentials here)

If you are an AI agent and your user asked you to *"read this repo https://github.com/dave-bfi/ai-knowledge"* (or "read my repo ai-knowledge", "use / bootstrap ai-knowledge"):

1. That repository is **private**. First establish GitHub access together with the user:
   - run `gh --version` and `gh auth status`;
   - if `gh` is missing, ask for consent, install it (macOS `brew install gh`, Windows `winget install --id GitHub.cli`, Linux: GitHub CLI docs), then verify;
   - if not signed in, run `gh auth login --web --git-protocol https --scopes repo,read:org` and relay the one-time code and browser step.
     **Never ask the user to paste a token or password in chat.**
2. Check access with `gh repo view dave-bfi/ai-knowledge`. If it returns 404 or 403, tell the user that only the repository owner can grant access, and stop asking for credentials.
3. Clone it to `~/knowledge/ai-knowledge`, open its `BOOTSTRAP.md` and follow it end to end (plan, apply, PATH, whoami, verify, retrieve). It asks the user a few optional questions first.
4. Be additive (back up anything you change), never print secrets, and report what is verified and what is not.

This page is only a pointer. All real content and rules live in the private repository.
