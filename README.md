Quote Database for Stormbot 6 - TCL
===================================
Developer: Dustin Lennon<br />
Email: <demonicpagan@gmail.com>

Install Instructions
--------------------
Just place this module in your botdir/scripts/beads directory and then run BOT maint load quote to load the module.

Refer to the help file in the module for usage instructions: BOT QUOTE help

If you experience any issues please submit a bug report on
<http://github.com/demonicpagan/Stormbot-TCL-Quote-Module/issues>.

You can always get the latest source from <http://github.com/demonicpagan/Stormbot-TCL-Quote-Module> as well.

Changelog - Dates are in Epoch time
-----------------------------------
1284435346

*	Moved help into the switch
*	Removed "set record" and changed to just tdb record array from ranking code

1284393748

*	Started work on rating code. Not working as expected at the moment. Will work on later to fix.

1284385721

*	Fixed some code to mention how many quotes are in the database.
*	Removed some code in the LAST command that was a copy/paste from STATISTICS and shouldn't have been there.

1284385300

*	In last commit, forgot a couple close braces that prevented the bead from loading.

1284385018

*	Fixed the multiline display when deleting a quote that is multilined.
*	Added multiline display functionality when showing last quote placed in the database if stored as a multiline quote.

1284382243

*	Added functionality to STATISTICS and LAST commands.

1284379269

*	Cleaned up text display if access level wasn't high enough (i.e. [QUOTE QUOTE] became [QUOTE OFF|ON] for turning the script on/off for a channel).

TODO - *DONE*

*	Fix how deleted quotes are displayed if they are multiline quotes.<br />
[ 05:58:00 am | 241009.13 ]   [ ~Demonicpagan ] w qe add This is a | multiline test quote<br />
[ 05:58:00 am | 241009.13 ]   [ @Worf ] [QUOTE ADD] Quote #2 has been added to the database!<br />
[ 06:04:56 am | 241009.13 ]   [ ~Demonicpagan ] w qe - 2<br />
[ 06:04:57 am | 241009.13 ]   [ @Worf ] [QUOTE DEL] Destroyed quote #2:<br />
[ 06:04:58 am | 241009.13 ]   [ @Worf ] Originally added by Demonicpagan: Mon, 13 Sep 2010, 06:04:31 CDT [Stardate 64698.2] CY6932<br />
[ 06:04:59 am | 241009.13 ]   [ @Worf ]  This is a<br />
[ 06:05:01 am | 241009.13 ]   [ @Worf ]  This is a<br />
[ 06:05:03 am | 241009.13 ]   [ @Worf ] [QUOTE DEL] 1 quote deleted.

1284377139

*	Fixed various errors in the quote delete code. Still a minor bug left in how the display of a quote is tried to be deleted in a channel it wasn't created
in.
*	Fixed syntax errors in the quote add code as well as a typo.
*	Fixed a typo in the SB:quote_conrol code. TBD save should have been TDB save

TODO

*	Fix quote deletion return value if quote being deleted wasn't set in the channel in which it's being deleted.<br />
[ 06:18:38 am | 241009.13 ]   [ @Worf ] [QUOTE DEL] 1 quote deleted.<br />
[ 06:18:39 am | 241009.13 ]   [ @Worf ] [QUOTE DEL] You can read quotes from any channel, but can only DELETE quotes from which they were created in. Quote #4 is from #BotHouse.

1284373573

*	Finally began work on this bead to replace a TCL quote script written by James Michael Seward.
*	At present moment, bead only allows for turning script on/off, adding quotes, removing quotes (still needs testing).
*	More work still planned to add the other features listed in the help.