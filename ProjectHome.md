This QVM is based on Lakitu7's latest QVM SVN.
The following are in addition to what is already provided.

**Variables**
  * **g\_adminTempMute** (seconds to mute a player by vote)
  * **g\_adminTempSpec** (seconds to spectate a player)
  * **g\_allStats** (enable or disable /allstats)
  * **g\_allStatsTime** (minimum seconds between use of /allstats per player)
  * **g\_autoGhost** (enable or disable the automatic dropping of duplicate GUID's)
  * **g\_defeatVotes** (enable or disable admit defeat votes)
  * **g\_extendVotesCount** (amount of times an extend vote can be called)
  * **g\_extendVotesPercent** (percentage required to pass an extend vote)
  * **g\_extendVotesTime** (minutes to extend game by)
  * **g\_feedingSpree** (deaths before declaring a feeding spree)
  * **g\_killerHp** (enable or disable the showing of a killer's hit points to their victim)
  * **g\_killingSpree** (kills before declaring a killing spree)
  * **g\_mapRotationVote** (seconds that a map vote menu appears for)
  * **g\_teamStatus** (enable or disable /teamstatus)
  * **g\_teamStatusTime** (minimum seconds between use of /teamstatus per player)

**Commands**
  * !adminlog
  * !drop
  * !nobuild
  * !seen
  * /allstats
  * /mark
  * /teamstatus

**Flags**
  * adminlog
  * ALWAYSVOTE - Player can vote even when voting is disabled (still requires CANVOTE).
  * CANDECON - Player can deconstruct.
  * CANVOTE - Player can vote.
  * drop
  * nobuild
  * seen

**Feature Enhancements**
  * !mute supports optional durations
  * !rotation supports g\_nextmap and map vote menus
  * Aliens can always evolve at the Overmind, even with Human presence
  * Cleaner ban and kick messages
  * Cleaner help output
  * Humans killed by Marauders get a new obituary message (X bit off Y's face)
  * Map vote menus
  * Multiple private message recipients
  * Sudden Death messages are printed to console
  * Team prefix colours
  * Unpowered Jet Pack messages

**Security Enhancements**
  * Players can't be voted against until after they enter the game.
  * GUID Verification (Make sure a client reports a valid GUID, if at all).
  * IP Verification (Make sure a client reports an IP address).
  * States are restored upon reconnection (!mute, !denybuild, !putteam spectate, vote count)

**Bug Fixes**
  * Escaped colours in votes.
  * Multiple hovels glitch.
  * Players can build over corpses.
  * Prevent team stacking through ptrcrestore.
  * Reverting an occupied Hovel doesn't create an invisible Granger.