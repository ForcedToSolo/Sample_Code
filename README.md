# Sample_Code
Tower Defense &amp; Linux File Uploader for Documentum


# Text2EDMS Program Overview:

Command line program used to take documents from a linux/unix/hpux environment & place them into an Enterprise Document Management System (EDMS, Documentum software) as attachments. The program uses regular expressions (found in the config file) to parse the attachment for information which will be used as metadata in the EDMS environment.

# Note worthies:

This program is self-updating; a bootstrap program logs the user in, validates their software version (via an MD5 checksum), and will auto-update their copy to the proper version. This eliminated the version fracturing that occured with the previous iteration of this program (which was written in Perl).

T2E prompts for user credentials only once & stores them encrypted in the users local directory. This satisfied a business need to log in as little as possible.

The banner criteria is configurable; regular expressions can be added/modified on the fly. This coupled with the banner interface class make it significantly easier to keep up with business requests for banner modifications. The previous Perl version required a significant undertaking (days) just to track & replace the various releases. The update process is now a matter of seconds once the new banner has been developed.

# SketchTD Program Overview:

Tower Defense game for all platforms (mobile - android/iOS, Web) using the ImpactJS engine. Bad guys navigate from the start & move towards the end & the user places towers along the way to defeat them.

This is an unfinished game, more of a barebones skeleton in some areas (score keeping/item upgrades/etc). The ultimate goal is to allow users to design their own tower/bad guy models and maps to share & compete with each other.

# Note worthies:

A* Pathfind is used - dynamic path from A to B, recalculated after each tower is placed (for efficiency).

Towers/units have upgrades (armor, damage, etc.)

