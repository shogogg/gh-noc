# gh-noc
A [gh](https://github.com/cli/cli) extension to check the pull request checks, and notify if the checks are passed or not.

## NOC means
Notify On Check status

## Requirements
- [terminal-notifier](https://github.com/julienXX/terminal-notifier)

## Install
```bash
gh ext install shogogg/gh-noc
```

## Usage
This extension is designed to run in background.
So we recommend to run this command with `&` and `disown` to run in background.

### For current branch
```bash
gh noc &; disown
```

### For specific branch
```bash
gh noc <branch> &; disown
```

### For specific pull request
```bash
gh noc <pull-request-number> &; disown
```

## Configuration
Customize the notification message and sound by setting the environment variables below.

### `GH_NOC_MESSAGE_ON_SUCCESS`
Message to notify when the checks are passed.

Default: `GitHub Actions checks are passed.`

### `GH_NOC_MESSAGE_ON_FAILURE`
Message to notify when the checks are failed.

Default: `GitHub Actions checks are failed.`

### `GH_NOC_SOUND_ON_SUCCESS`
Notification sound to play when the checks are passed.

Default: `default`

### `GH_NOC_SOUND_ON_FAILURE`
Notification sound to play when the checks are failed.

Default: `default`
