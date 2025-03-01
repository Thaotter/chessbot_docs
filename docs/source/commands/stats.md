# `/stats` Command

## Description
The `/stats` command allows you to view detailed statistics for any Chess.com account, displaying their performance across different time controls.

## Usage
```
/stats [username]
```

### Parameters
- `username` (required): The Chess.com username you want to check statistics for.

## Features
- Shows current and peak ratings for each time format (Bullet, Blitz, Rapid)
- Displays win/loss/draw record
- Includes visual representation of statistics
- Shows country flag based on player's location
- Displays player titles (GM, IM, etc.) if applicable

## Examples
- `/stats Hikaru` - Shows statistics for the Chess.com user "Hikaru"
- `/stats magnuscarlsen` - Shows statistics for the Chess.com user "magnuscarlsen"

## Notes
- Username is not case-sensitive
- If the specified user doesn't exist on Chess.com, you'll receive an error message
- Statistics are updated based on the most recent data from Chess.com's API

## Troubleshooting
- If you receive an error message, verify that the username is spelled correctly
- Some users may have privacy settings that restrict access to their statistics
- If Chess.com's API is experiencing issues, the command may not work temporarily

## Related Commands
- [`/profile`](profile.md) - View a player's Chess.com profile information
- [`/compare`](compare.md) - Compare statistics between 2-4 players