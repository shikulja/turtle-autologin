# Vanilla AutoLogin

Patch from 1.12.1 vanilla WoW client that adds auto login and account info saving features.

> This patch saves your login info into `\WTF\Config.wtf` so keep in mind that it will **contain your passwords** and thus you should think before sharing this file with someone else.

## Features

- Adds an Accounts select panel to the login screen
- Automatically adds accounts with saved login info to the list
- Select accounts to log in (double-click to login directly)
- Check "Auto-login this character" in character select screen to always automatically load into game with this character selected in future logins
- Remove saved character and accounts with controls at the bottom

## Installation

### [Patch-Y.MPQ download link](https://github.com/Haaxor1689/vanilla-autologin/releases/download/release/Patch-Y.mpq)

Download the `Patch-Y.MPQ` and place the file inside `\Data` folder of your client.

## Advanced usage

Account information is saved under `accountName` in your `\WTF\Config.wtf` file. Unlike vanilla behavior, where it contains only the account name. When using this patch it will contain data in following format:

```
<name> <password> <character>;
```

Each entry ends with a `;` symbol. To disable character auto login, third value should be `-`.
