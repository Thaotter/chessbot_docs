ChessBot Documentation
======================

Welcome to the official documentation for ChessBot, a Discord bot that integrates with Chess.com to provide statistics, profiles, and comparison features for chess players.

Overview
--------

ChessBot allows Discord users to:

* View Chess.com player statistics
* Compare multiple players' performance
* Link their Discord account with their Chess.com account
* View detailed Chess.com profiles
* Set up ELO rating roles for server members (admin only)

Command List
-----------

.. list-table::
   :widths: 20 50 30
   :header-rows: 1

   * - Command
     - Description
     - User Type
   * - `/stats <username>`_
     - View Chess.com player statistics
     - All users
   * - `/compare <usernames> <category>`_
     - Compare 2-4 Chess.com players
     - All users
   * - `/profile <username>`_
     - View Chess.com player profile
     - All users
   * - `/link <username>`_
     - Link Discord to Chess.com account
     - All users
   * - `/help`_
     - Get help with ChessBot
     - All users
   * - `/elo-setup`_
     - Set up ELO rating roles
     - Server admins
   * - `/erase-elo-roles`_
     - Remove all ELO roles
     - Server admins
   * - `/update-elo-roles`_
     - Force update ELO roles
     - Server admins

.. _`/stats <username>`: commands/stats.html
.. _`/compare <usernames> <category>`: commands/compare.html
.. _`/profile <username>`: commands/profile.html
.. _`/link <username>`: commands/link.html
.. _`/help`: commands/help.html
.. _`/elo-setup`: commands/elo-setup.html
.. _`/erase-elo-roles`: commands/erase-elo-roles.html
.. _`/update-elo-roles`: commands/update-elo-roles.html

Getting Started
--------------

* `Adding ChessBot to Your Server <getting-started/adding-the-bot.html>`_
* `Basic Usage Guide <getting-started/basic-usage.html>`_
* `Server Administration <getting-started/server-admin.html>`_

FAQs
----

For answers to frequently asked questions, see the `FAQ page <faq.html>`_