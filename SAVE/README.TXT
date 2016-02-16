First off, the new account files are kept in the worldsave folder.
SPHEREacct.scp and SPHEREaccu.scp

To make changes to or add new entries to accounts, you no longer have to edit the existing account file (SPHEREaccu.scp), simply make a new SPHEREacct.scp file with all your updates in it following proper format:

For Staff:

[AcctName]
PASSWORD=password
LEVEL=##
PRIV=##

[AcctName]
PASSWORD=password
LEVEL=##
PRIV=##

For Players:

[AcctName]
PASSWORD=password
LEVEL=1

[AcctName]
PASSWORD=password
LEVEL=1

Always have one empty line between account entries. Do not put in remarks  (lines started with //) because they are no longer saved in the file.

If the account already exists, it changes the info to match the ones you made.

when done with additions:
1) save the file as SPHEREacct.scp
2) copy/upload to your server system and THEN copy to your worldsave folder (as defined in SPHERE.INI)
or if local .. save or copy into your worldsave folder
3) In the server console press A then enter; if in-game and an Admin, you may use .ACCOUNT UPDATE
4) In the server console press shift-3 (for #) to save or if in-game and an Admin you may use .SAVE 1 (this is for a current bug which doesn't initiate the accounts immediately on update, but should be fixed soon)

You are done, accounts updated into the proper place and saved.

Account PRIV's and LEVEL's
LEVEL is the recommended option to use, but either is valid

PRIV=0	//player
PRIV=1	//Admin
PRIV=2	//GM
PRIV=4	//Councilor
PRIV=8	//Can listen to Pages
PRIV=10	//Can Broadcast ( !  yell)
PRIV=20	//Can Move all items
PRIV=40	//40=Can get UID number on single-clk (only for debugging)
PRIV=80	//Sets Debug mode (see debug Command)

LEVEL=0	// PLEVEL_Guest	Restricted Guest Account, ie. can't PK
LEVEL=1	// PLEVEL_Player	Player or NPC
LEVEL=2	// PLEVEL_Counsel	Can travel (teleport)
LEVEL=3	// PLEVEL_Seer	Can add items and NPC's but cannot directly affect players
LEVEL=4	// PLEVEL_GM	GM Command Clearance
LEVEL=5	// PLEVEL_Dev	Developement Clearence, not bothered by GM
LEVEL=6	// PLEVEL_Admin	Can Swith into and out of GM mode


FOR MORE INFORMATION SEE THE SUPPORT MENU (ADMIN SECTION) AT WWW.SPHERESERVER.COM

ADDITIONAL NOTES ABOUT WORLDFILES AND ACCOUNT FILES:
This are files needed by the first-time users to get started. These files are not included with the distributed Server to avoid overwriting the customized files of existing shards during an update.

SPHEREaccu.scp -- The actual account file
SPHEREacct.scp -- Where you add your accounts
SPHEREworld.scp -- a BLANK worldfile to avoid a save error on first run.
SPHEREitem2.scp -- Where you place custom-made or edited items
SPHEREchar2.scp -- Where you place custom-made or edited characters

Place SPHEREaccu.scp; SPHEREacct.scp; and SPHEREworld.scp in your save folder
Place SPHEREitem2.scp and SPHEREchar2.scp into your server folder