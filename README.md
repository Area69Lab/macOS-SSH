# macOS-SSH

_SSH into macOS Big Sur running in GitHub Actions_

## _Preparation_

1. Fork This Repo
2. Add your ngrok authtoken as `NGROK_TOKEN` in the Repository Secrets
   > You can find this token here: https://dashboard.ngrok.com/auth/your-authtoken
3. Add a shell login password as `SSH_PASSWORD` in the Repository Secrets
4. To get Session Link in Telegram [Optional, but Recommended]
   - Add  your bot token as `TELEGRAM_BOT_TOKEN` and group chat id as `TELEGRAM_CHAT_ID` in the Repository Secrets
5. Go to Actions tab, select the workflow name, and run it through `workflow_dispatch` method

### _That's it!_

> Default username of macOS VM in ngrok mode is `root`. If you want to change to normal user, after login, run `su - runner` and continue work

### _Where To Go Next_

Experiment anything in your own remote _macOS Big Sur_ machine.

What's inside the beast?! Run `system_profiler SPHardwareDataType` inside the session or use `pip3 install bpytop && bpytop`

Good Luck.

### _Credits_

- [rokibhasansagar](https://github.com/rokibhasansagar) - Author
- Team [Area69Lab](https://github.com/Area69Lab) for inspiring me into using macOS
- [P3TERX's ssh2actions](https://github.com/P3TERX/ssh2actions) for SSH-ing into Actions

### _Disclaimer_

```text
Please do not use this repository for 24x7x365 operations on GitHub.
Your account might get flagged or banned if GitHub Authorities want to do so.
Use this for education purposes only.
```
