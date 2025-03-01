# ChessBot Basic Usage Guide

This guide covers the fundamental commands and features of ChessBot to help you get started quickly.

## Getting Started with ChessBot

ChessBot uses Discord's slash command system, which means all commands begin with a forward slash (`/`) followed by the command name. When you type `/`, Discord will show a list of available commands from ChessBot.

## Linking Your Chess.com Account

The first thing you should do is link your Chess.com account to your Discord profile:

1. Type `/link username` (replace "username" with your Chess.com username)
2. Example: `/link Hikaru`
3. ChessBot will confirm when your account is successfully linked

Once linked, you can use many commands without specifying a username, as ChessBot will use your linked account by default.

## Core Commands

### Viewing Chess.com Stats

To check your or someone else's Chess.com statistics:
- `/stats` - Shows your own stats (if you've linked your account)
- `/stats username` - Shows stats for the specified Chess.com user
- Example: `/stats magnuscarlsen`

The stats command shows:
- Current and peak ratings for Bullet, Blitz, and Rapid
- Win/loss/draw record
- Graphical representation of performance

### Viewing Player Profiles

To view detailed profile information:
- `/profile` - Shows your own profile (if you've linked your account)
- `/profile username` - Shows profile for the specified user
- Example: `/profile GothamChess`

The profile command displays:
- Account information and join date
- Profile picture
- Location and country
- Membership status
- Social statistics (followers, etc.)

### Comparing Players

To compare multiple Chess.com players:
- `/compare username1 username2 category`
- You can compare 2-4 players at once
- Example: `/compare Hikaru Naroditsky Blitz`

Available categories for comparison:
- `Overall` - Compare overall performance
- `Bullet` - Compare Bullet game statistics
- `Blitz` - Compare Blitz game statistics
- `Rapid` - Compare Rapid game statistics

## Getting Help

If you need assistance with ChessBot:
- `/help` - Shows a list of all available commands with brief descriptions

## Tips for Best Experience

1. **Link Your Account**: This makes using commands faster and more convenient
2. **Check Usernames Carefully**: Ensure Chess.com usernames are spelled correctly
3. **Be Patient**: Image generation and API calls may take a few seconds to complete
4. **Try Different Comparisons**: The compare command has different layouts for 2, 3, or 4 players
5. **Include Category**: Always specify which category (Overall, Rapid, Blitz, Bullet) when using `/compare`

## Next Steps

After mastering the basics, server administrators might want to explore:
- [Setting Up ELO Roles](server-admin.md) - Automatically assign roles based on Chess.com ratings
- [Customizing ELO Role Ranges](../commands/elo-setup.md) - Tailor ELO roles to your server's needs