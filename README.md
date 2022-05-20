## Instructions
1. Make sure your old esoTalk installation is fully upgraded to beta 2.
2. Create a new MySQL database.
3. Install a new copy of [1.0.0g2](https://github.com/aokod/esoTalk-1.0.0b3/commit/f05dc997c927bc8dee250aa0960950eee1e7b6ec) in a different folder. Go through the installation process so your forum is all set up. Install into the fresh MySQL database you just created.
4. Download the upgrade script.
5. Upload the upgrade script to a new folder on your server. Open up index.php in a text editor and edit the config variables for your MySQL connection and the old/new databases and table prefixes.
6. Load the upgrade script index.php in your browser. The upgrade script will run. It may take a while, depending on how much data is in your forum.
7. Copy avatars from your beta folder (avatars/) to your gamma folder (uploads/avatars/).
8. Load up your gamma installation in your browser. Hopefully all the data should have transferred over!

## Limitations/Known Issues
1. All users will have to reset their password using the Forgot Password process. This is because the password encryption method changed between beta/gamma.
2. Some complex formatting (nested quotes/lists) may not be converted correctly.

Credit to @tobyzerner for writing the upgrade script.
