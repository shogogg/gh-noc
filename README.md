# gh-noc
A [gh](https://github.com/cli/cli) extension to check the pull request checks, and notify if the checks are passed or not.

## NOC means
Notify On Check status

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
