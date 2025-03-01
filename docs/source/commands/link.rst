`/link` Command
=============

Description
----------
The ``/link`` command allows you to link your Discord account with your Chess.com account, enabling you to use ChessBot commands without specifying your username each time.

Usage
-----
.. code-block::

   /link [username]

Parameters
~~~~~~~~~
* ``username`` (optional): The Chess.com username you want to link to your Discord account.
   * If not provided, displays your currently linked Chess.com account (if any).

Features
-------
* Links your Discord ID to your Chess.com username in the bot's database
* Allows you to use other commands without specifying a username
* Verifies that the Chess.com account exists before linking
* Provides a simple way to check which Chess.com account you're currently linked to

Examples
--------
* ``/link Hikaru`` - Links your Discord account to the Chess.com user "Hikaru"
* ``/link`` - Shows which Chess.com account (if any) is linked to your Discord account

Notes
-----
* You can change your linked account at any time by using the ``/link`` command with a different username
* Username is not case-sensitive
* Only one Chess.com account can be linked to your Discord account at a time
* When linked, commands like ``/stats`` and ``/profile`` will use your linked account by default if no username is specified

Troubleshooting
--------------
* If you receive an error when linking, verify that the Chess.com username exists
* If the link command isn't working, the bot may be experiencing database connectivity issues
* Your linked account information is stored securely in the bot's database

Related Commands
--------------
* :doc:`/commands/stats` - View your own stats (when linked) or another player's stats
* :doc:`/commands/profile` - View your own profile (when linked) or another player's profile