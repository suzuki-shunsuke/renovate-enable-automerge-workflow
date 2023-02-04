# renovate-enable-automerge-workflow

GitHub Actions Reusable Workflow to enable automerge of a pull request from Renovate

## How to use

```yaml
---
name: test
on:
  pull_request: {}
permissions: {}
jobs:
  enable-automerge:
    uses: suzuki-shunsuke/renovate-enable-automerge-workflow/.github/workflows/enable_automerge.yaml@main
    secrets:
      github_app_id: ${{secrets.GH_APP_ID}}
      github_app_private_key: ${{secrets.GH_APP_PRIVATE_KEY}}
    permissions: {}
```

## Requirements

- GitHub CLI

GitHub Personal Access Token or GitHub App

permissions

- contents: write
- pull-requests: write

## LICENSE

[MIT](LICENSE)
