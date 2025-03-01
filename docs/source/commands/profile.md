# `/profile` Command

## Description
The `/profile` command provides detailed information about a Chess.com player's account, including their profile information, membership status, and social statistics.

## Usage
```
/profile [username]
```

### Parameters
- `username` (required): The Chess.com username you want to check the profile for.

## Features
- Displays player's account information
- Shows profile picture from Chess.com
- Includes join date and membership status
- Provides social statistics (followers, friends)
- Shows player location and country flag
- Displays titles (GM, IM, etc.) if applicable
- Shows streamer status and Twitch info if available

## Examples
- `/profile Hikaru` - Shows profile information for the Chess.com user "Hikaru"
- `/profile magnuscarlsen` - Shows profile information for the Chess.com user "magnuscarlsen"

## Notes
- Username is not case-sensitive
- Information displayed is based on what the player has made public on their Chess.com profile
- The profile image is generated based on the most recent data from Chess.com's API

## Troubleshooting
- If you receive an error message, verify that the username is spelled correctly
- Some users may have privacy settings that restrict access to their profile information
- If Chess.com's API is experiencing issues, the command may not work temporarily

## Related Commands
- [`/stats`](stats.md) - View detailed game statistics for a player
- [`/link`](link.md) - Link your Discord account to your Chess.com account