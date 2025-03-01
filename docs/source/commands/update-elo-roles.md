# `/update-elo-roles` Command

## Description
The `/update-elo-roles` command allows server administrators to force an update of ELO rating roles for all members who have linked their Chess.com accounts. This is useful after setting up ELO roles or when you want to ensure everyone's roles are up-to-date with their current Chess.com ratings.

## Usage
```
/update-elo-roles
```

### Parameters
- None

## Features
- Updates ELO roles for all members with linked Chess.com accounts
- Assigns appropriate title roles (GM, IM, FM, etc.) if enabled
- Removes outdated ELO roles if a member's rating has changed
- Processes all linked members in the server at once
- Provides a status message upon completion

## Permissions Required
- `Manage Server` permission is required to use this command
- The bot must have the `Manage Roles` permission
- The bot's highest role must be positioned above the ELO roles it will assign

## Notes
- This command will only affect members who have linked their Chess.com accounts with `/link`
- ELO roles must first be created using the `/elo-setup` command
- The process may take some time depending on the number of linked members in your server
- Members' roles are based on their highest Chess.com rating across all time controls
- This command is useful after making changes to your ELO role configuration

## Troubleshooting
- If roles aren't being updated, check that the bot has the `Manage Roles` permission
- If specific members aren't getting roles, ensure they have linked their Chess.com accounts
- If you're getting an error, verify that you've set up ELO roles with `/elo-setup` first

## Related Commands
- [`/elo-setup`](elo-setup.md) - Set up ELO rating roles for the server
- [`/erase-elo-roles`](erase-elo-roles.md) - Remove all ELO rating roles created by the bot
- [`/link`](link.md) - Link Discord accounts to Chess.com accounts (required for role assignment)