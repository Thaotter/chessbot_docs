`/erase-elo-roles` Command
=======================

Description
----------
The ``/erase-elo-roles`` command allows server administrators to remove all ELO rating roles that were previously created by the bot using the ``/elo-setup`` command.

Usage
-----
.. code-block::

   /erase-elo-roles

Parameters
~~~~~~~~~
* None

Features
-------
* Removes all ELO rating roles created by the bot
* Removes all chess title roles created by the bot
* Cleans up the server's role list completely of ChessBot-created roles
* Provides confirmation when all roles have been successfully removed

Permissions Required
------------------
* ``Manage Server`` permission is required to use this command
* The bot must have the ``Manage Roles`` permission
* The bot's highest role must be positioned above the ELO roles it will remove

Notes
-----
* This command will remove ALL roles created by the ``/elo-setup`` command
* It's useful when you want to reconfigure your ELO roles or if you no longer want to use the ELO role system
* This action cannot be undone - if you want ELO roles again, you'll need to run ``/elo-setup`` again
* Members who had ELO roles will have them removed

Troubleshooting
--------------
* If roles aren't being removed, check that the bot has the ``Manage Roles`` permission
* If specific roles aren't being removed, ensure the bot's highest role is positioned above those roles
* If you're getting an error, it may be because there are no ELO roles to remove

Related Commands
--------------
* :doc:`/commands/elo-setup` - Set up ELO rating roles for the server
* :doc:`/commands/update-elo-roles` - Force update ELO roles for all server members