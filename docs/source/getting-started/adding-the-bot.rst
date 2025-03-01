Adding ChessBot to Your Server
===========================

This guide will walk you through the process of adding ChessBot to your Discord server.

Prerequisites
------------

Before adding ChessBot, ensure you have:

* A Discord server where you have the **Manage Server** permission
* A web browser to complete the authorization process

Invitation Process
----------------

1. **Visit the ChessBot Invitation Page**
   
   * Click on the `official invitation link <https://discord.com/api/oauth2/authorize?client_id=1076621730442924197&permissions=545394781431&scope=bot>`_ 
   * You may need to log in to Discord if you haven't already

2. **Select Your Server**
   
   * From the dropdown menu, select the server you want to add ChessBot to
   * Make sure you have the necessary permissions on the selected server

3. **Authorize Permissions**
   
   * ChessBot requires the following permissions:
     
     * **Read Messages/View Channels** - To see and respond to commands
     * **Send Messages** - To reply to users
     * **Embed Links** - To display rich embeds with chess statistics
     * **Attach Files** - To send images with chess statistics and comparisons
     * **Use Slash Commands** - To register and respond to slash commands
     * **Manage Roles** (optional) - Required only if you want to use the ELO role features

4. **Complete Authorization**
   
   * If you agree with the requested permissions, click "Authorize"
   * You may need to complete a CAPTCHA to verify you're human
   * Once authorized, ChessBot will join your server

Initial Setup
-----------

After adding ChessBot to your server:

1. **Check Bot Permissions**
   
   * Ensure ChessBot has access to the channels where you want it to work
   * If using ELO roles, ensure ChessBot's role is positioned higher than the roles it will manage

2. **Test Basic Commands**
   
   * Try using the ``/help`` command to verify the bot is working correctly
   * Test a basic command like ``/stats Hikaru`` to ensure API connectivity

3. **Optional: Set Up ELO Roles**
   
   * If you want to use ELO roles, use the ``/elo-setup`` command
   * See :doc:`/commands/elo-setup` for detailed instructions

Troubleshooting
-------------

If you encounter issues when adding ChessBot:

* **"Bot couldn't be added to the server"** - Verify you have the Manage Server permission
* **Commands not appearing** - It may take up to an hour for slash commands to register; try rejoining the server
* **Can't see bot in member list** - Check your server's integration settings and ensure the bot isn't hidden
* **Permission errors** - Make sure the bot has all the necessary permissions listed above

For further assistance, join the `ChessBot Support Server <https://discord.gg/tAEBJPYd3a>`_ 
