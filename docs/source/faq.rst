Frequently Asked Questions (FAQ)
=============================

General Questions
---------------

What is ChessBot?
^^^^^^^^^^^^^^^^
ChessBot is a Discord bot that integrates with Chess.com to provide player statistics, profile information, and comparison features directly in your Discord server.

Is ChessBot free to use?
^^^^^^^^^^^^^^^^^^^^^^
Yes, ChessBot is completely free to use with all of its features.

How do I add ChessBot to my server?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
See our :doc:`/getting-started/adding-the-bot` guide for detailed instructions.

Does ChessBot work with other chess platforms like Lichess?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Currently, ChessBot only supports Chess.com. Support for other platforms may be added in the future.

Command Usage
-----------

Why do I need to link my Chess.com account?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Linking your account makes it easier to use ChessBot commands without having to type your username each time. It's also required for ELO role assignment in servers that use this feature.

How do I link my Chess.com account?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Use the ``/link username`` command where "username" is your Chess.com username.

Can I check stats for any Chess.com user?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Yes, you can check stats for any public Chess.com profile using the ``/stats username`` command.

Why do some commands show an error message?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
This typically happens when:

* The specified Chess.com user doesn't exist
* The user has privacy settings that restrict access to their data
* Chess.com's API is temporarily unavailable
* The username contains special characters or formatting that ChessBot can't process

How many players can I compare at once?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
You can compare 2-4 players at once using the ``/compare`` command.

ELO Roles
--------

What are ELO roles?
^^^^^^^^^^^^^^^^^
ELO roles are Discord roles created by ChessBot based on Chess.com ratings. Server admins can set these up to automatically assign roles to members based on their chess rating.

How do ELO roles work?
^^^^^^^^^^^^^^^^^^^
Once set up by a server admin, ChessBot assigns roles to members who have linked their Chess.com accounts. The roles are based on the member's highest rating across all time controls.

Why didn't I receive an ELO role?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
You may not have received an ELO role because:

* You haven't linked your Chess.com account with ``/link``
* The server hasn't set up ELO roles with ``/elo-setup``
* Your Chess.com profile has privacy settings that restrict access to your ratings
* Your rating doesn't fall within the ranges set by the server administrator
* The bot doesn't have permission to assign the role to you

How often are ELO roles updated?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
ELO roles are updated when:

* You use any ChessBot command that checks your statistics
* A server admin uses the ``/update-elo-roles`` command
* They don't update automatically on a schedule

Technical Questions
-----------------

Is my Chess.com account information secure?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
ChessBot only stores your Discord ID and Chess.com username in its database. It doesn't access or store any sensitive information from your Chess.com account.

Why are some images slow to generate?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Generating comparison images for multiple players or complex stats visualizations can take a few seconds, especially during high usage periods.

Why are the bot's responses sometimes delayed?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Delays can occur due to:

* High traffic on Chess.com's API
* Discord API rate limits
* Server load during peak usage times

Who can I contact for support?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
For additional help or to report issues, join the `ChessBot Support Server <https://discord.gg/chessbot>`_ (replace with actual link).

Server Administration
------------------

Can I customize which ELO ranges get roles?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Yes, server admins can use the ``/elo-setup`` command with custom parameters to define the ELO ranges for roles.

How do I remove all ELO roles?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Use the ``/erase-elo-roles`` command to remove all ELO roles created by ChessBot.

Can ChessBot assign roles based on Puzzle rating?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Currently, ELO roles are based only on standard game ratings (Bullet, Blitz, Rapid), not Puzzle ratings.