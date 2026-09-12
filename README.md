# Kriens macOS interactive testing

This public repository launches a disposable GitHub-hosted Mac, builds Kriens
Connect & Work from its private source repository, and provides a temporary
noVNC link for browser-based mouse and keyboard testing.

## One-time setup

Add these repository Actions secrets under **Settings → Secrets and variables
→ Actions**:

- `KRIENS_SOURCE_TOKEN`: a fine-grained, read-only GitHub token restricted to
  `turjotree/turya-mukherjee-portfolio` with **Contents: Read-only**.
- `NOVNC_PASSWORD`: a temporary password of at least 10 characters that you
  will type into noVNC. It is never printed to the public workflow logs.

## Start a test

1. Open **Actions → macOS Public noVNC Test → Run workflow**.
2. Choose 15, 30, 45, or 60 minutes and start the run.
3. Open the active run and select **Summary**.
4. Open the generated noVNC link.
5. Sign in with username `kriensvnc` and your `NOVNC_PASSWORD` value.
6. Cancel the workflow as soon as testing is finished.

The public repository contains only the runner definition. The Kriens source,
credentials, and customer data remain private. Standard GitHub-hosted runners
for public repositories do not consume the account's included private-repo
minutes, but GitHub's job-duration, concurrency, and acceptable-use limits
still apply.
