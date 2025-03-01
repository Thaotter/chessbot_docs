# `/elo-setup` Command

## Description
The `/elo-setup` command allows server administrators to create a series of ELO rating roles that will automatically be assigned to members based on their linked Chess.com accounts.

## Usage
```
/elo-setup [minelo] [maxelo] [increment] [include_titles]
```

### Parameters
- `minelo` (optional, default: 0): The minimum ELO rating for the role range.
- `maxelo` (optional, default: 3000): The maximum ELO rating for the role range.
- `increment` (optional, default: 200): The increment between each ELO role.
- `include_titles` (optional, default: true): Whether to create roles for chess titles (GM, IM, FM, etc.)

## Features
- Creates a series of roles based on ELO ranges (e.g., "ELO 1000-1200", "ELO 1200-1400", etc.)
- Optionally creates roles for chess titles (GM, IM, FM, WGM, WIM, WFM, etc.)
- Automatically assigns roles to members who have linked their Chess.com accounts
- Updates roles when members use ChessBot commands or when forced with `/update-elo-roles`

## Examples
- `/elo-setup` - Creates roles with default settings (0-3000 ELO, 200 increments, with titles)
- `/elo-setup 800 2600 100 true` - Creates roles from 800-2600 ELO with 100 point increments, including title roles
- `/elo-setup 1000 2000 250 false` - Creates roles from 1000-2000 ELO with 250 point increments, without title roles

## Permissions Required
- `Manage Server` permission is required to use this command
- The bot must have the `Manage Roles` permission
- The bot's highest role must be positioned above the ELO roles it will create

## Notes
- ELO roles are based on a player's highest rating across all time controls
- Role colors are automatically assigned based on the ELO range
- Existing ELO roles will be removed and recreated if the command is run again
- Members will only receive ELO roles if they have linked their Chess.com account with `/link`

## Troubleshooting
- If roles aren't being created, check that the bot has the `Manage Roles` permission
- If the bot isn't assigning roles to members, ensure its highest role is positioned above the ELO roles
- If you want to remove all ELO roles, use the `/erase-elo-roles` command

## Related Commands
- [`/erase-elo-roles`](erase-elo-roles.md) - Remove all ELO rating roles created by the bot
- [`/update-elo-roles`](update-elo-roles.md) - Force update ELO roles for all server members
- [`/link`](link.md) - Link Discord accounts to Chess.com accounts (required for role assignment)