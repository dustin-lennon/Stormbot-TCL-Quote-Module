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
1284377139

*	Fixed various errors in the quote delete code. Still a minor bug left in how the display of a quote is tried to be deleted in a channel it wasn't created
in.
*	Fixed syntax errors in the quote add code as well as a typo.
*	Fixed a typo in the SB:quote_conrol code. TBD save should have been TDB save

TODO

*	Fix quote deletion return value if quote being deleted wasn't set in the channel in which it's being deleted.
[ 06:18:38 am | 241009.13 ]   [ @Worf ] [QUOTE DEL] 1 quote deleted.
[ 06:18:39 am | 241009.13 ]   [ @Worf ] [QUOTE DEL] You can read quotes from any channel, but can only DELETE quotes from which they were created in. Quote #4 is from #BotHouse.

1284373573

*	Finally began work on this bead to replace a TCL quote script written by James Michael Seward.
*	At present moment, bead only allows for turning script on/off, adding quotes, removing quotes (still needs testing).
*	More work still planned to add the other features listed in the help.