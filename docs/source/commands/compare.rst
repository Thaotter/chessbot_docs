`/compare` Command
================

Description
----------
The ``/compare`` command allows you to compare the statistics of 2-4 Chess.com players side by side, providing a visual comparison of their performance in different time controls.

Usage
-----
.. code-block::

   /compare [usernames] [category]

Parameters
~~~~~~~~~
* ``usernames`` (required): A space-separated list of 2-4 Chess.com usernames to compare.
* ``category`` (required): The time control category to compare. Options include:
   * ``Overall`` - Compare overall performance across all time controls
   * ``Rapid`` - Compare only Rapid game statistics
   * ``Blitz`` - Compare only Blitz game statistics
   * ``Bullet`` - Compare only Bullet game statistics

Features
-------
* Side-by-side comparison of player ratings
* Visual representation with different layouts based on number of players
* Shows current ratings, win/loss/draw records, and total games
* Displays country flags and titles (GM, IM, etc.) if applicable

Examples
--------
* ``/compare Hikaru GothamChess Overall`` - Compares overall statistics for Hikaru and GothamChess
* ``/compare magnuscarlsen Hikaru Naroditsky Bullet`` - Compares Bullet statistics for three players

Notes
-----
* Usernames are not case-sensitive
* The order of usernames affects their position in the comparison image
* If any specified user doesn't exist on Chess.com, you'll receive an error message
* The command automatically adjusts the layout based on how many players you're comparing

Troubleshooting
--------------
* Ensure all usernames are spelled correctly and separated by spaces
* Verify that all players have played games in the selected category
* Some users may have privacy settings that restrict access to their statistics

Related Commands
--------------
* :doc:`/commands/stats` - View detailed statistics for a single player
* :doc:`/commands/profile` - View a player's Chess.com profile information
