# Kriens macOS Actions Public Runner

Public GitHub Actions harness for manual macOS GUI/noVNC testing.

## Important

- This repository is **public**. Do not commit private Kriens source code, credentials, tokens, customer data, or other confidential material here.
- Standard GitHub-hosted runners in public repositories are currently free to use, but GitHub Actions still has workflow, concurrency, acceptable-use, and per-job runtime limits.
- This repository is intended for development/testing of the software and test harness associated with this repository, not as a generic compute service.

## Run a macOS GUI session

1. Open **Actions**.
2. Select **macOS Public noVNC Test**.
3. Click **Run workflow**.
4. Choose a session duration.
5. Open the generated noVNC URL shown in the workflow summary.
6. Sign in with the temporary username/password shown in the summary.
7. Cancel the workflow when finished.

The session also stops automatically at the selected limit.

## Kriens app source

The workflow does not publish or copy the private Kriens codebase. If you want the actual Kriens app to be built here, first decide what source is safe to make public. A public mirror can then be added to this repository or referenced by the workflow.
