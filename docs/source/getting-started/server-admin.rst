Server Administration Guide
========================

This guide is for Discord server administrators who want to use ChessBot's advanced features to enhance their chess community.

ELO Rating Roles System
---------------------

One of ChessBot's most powerful features is the ability to automatically assign roles based on members' Chess.com ratings.

Setting Up ELO Roles
^^^^^^^^^^^^^^^^^^^^

1. **Prerequisites**:
   
   * You must have the ``Manage Server`` permission
   * ChessBot must have the ``Manage Roles`` permission
   * ChessBot's highest role must be positioned above where the ELO roles will be in your role hierarchy

2. **Basic Setup**:
   
   * Use ``/elo-setup`` with no parameters for default settings:
     
     * Creates roles from 0-3000 ELO in 200-point increments
     * Includes chess title roles (GM, IM, FM, etc.)

3. **Customized Setup**:
   
   * Use ``/elo-setup minelo maxelo increment include_titles`` with your preferred values
   * Example: ``/elo-setup 800 2600 100 true``
   * This creates roles from 800-2600 ELO with 100-point increments and includes title roles

4. **Role Assignment**:
   
   * Members must link their Chess.com accounts using ``/link username``
   * Roles are assigned based on highest rating across all time controls
   * Title roles are assigned if the player has an official chess title

Managing ELO Roles
^^^^^^^^^^^^^^^^^

1. **Updating Roles**:
   
   * Use ``/update-elo-roles`` to force an update of all members' roles
   * This is useful after setting up ELO roles or after a Chess.com rating update period

2. **Removing ELO Roles**:
   
   * Use ``/erase-elo-roles`` to remove all ELO rating roles created by ChessBot
   * This completely removes the ELO role system from your server

3. **Modifying ELO Roles**:
   
   * To change your ELO role configuration, first use ``/erase-elo-roles``
   * Then set up a new configuration with ``/elo-setup``

Best Practices for Server Administrators
--------------------------------------

1. **Role Hierarchy**:
   
   * Keep ChessBot's role above the ELO roles it manages
   * Consider where ELO roles should appear in your overall role hierarchy

2. **Channel Permissions**:
   
   * Consider creating chess discussion channels with special access for higher-rated players
   * You might create exclusive channels for titled players

3. **Member Onboarding**:
   
   * Encourage new members to link their Chess.com accounts using ``/link``
   * Consider creating a dedicated #chess-bot channel for commands

4. **Regular Updates**:
   
   * Run ``/update-elo-roles`` periodically (monthly is recommended) to keep roles current
   * This ensures roles reflect members' current Chess.com ratings

5. **Communication**:
   
   * Inform your members about the ELO role system and what each role represents
   * Explain how to link accounts to receive appropriate roles

Troubleshooting
-------------

Common Issues
^^^^^^^^^^^^

1. **Roles Not Being Created**:
   
   * Verify ChessBot has the ``Manage Roles`` permission
   * Check that there are no conflicting roles with the same names

2. **Roles Not Being Assigned**:
   
   * Ensure ChessBot's role is positioned higher than the ELO roles
   * Verify members have linked their Chess.com accounts
   * Check that members' account privacy settings allow access to their ratings

3. **Permission Errors**:
   
   * If you see permission errors, review your server's role hierarchy
   * Make sure ChessBot has all necessary permissions

For additional help with server administration, join the `ChessBot Support Server <https://discord.gg/tAEBJPYd3a>`_ 
