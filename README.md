# get-toolkit-action

This GitHub action will lint and test project's image with Dockle and also send notifications to slack depending on the configuration.

## Config

- `registry`:
  - description: `Registry's host`
  - required: `false`
  - default: `"ghcr.io"`
- `user`:
  - description: `Registry's user`
  - required: `false`
  - default: `${{ github.actor }}`
- `password`:
  - description: `Registry user's password or token`
  - required: `true`
- `image`:
  - description: `Docker image name with tag`
  - required: `true`
- `slack-webhook`:
  - description: `Slack Webhook for notifications`
  - required: `true`