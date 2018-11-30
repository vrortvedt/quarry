# QUARRY
Blockchain-based social networking game to be played at conferences

## Overview
Quarry is a game/dapp hybrid meant to be played with a large group of participants located in the same physical space over several days.  Initial use cases are Devcon V in late 2019 or college orientations.  It will run on either an Ethereum testnet or on a Plasma/L2 chain. 

The basic premise is that participating conference attendees are randomly assigned the name of another attendee to try to find ("the quarry") within each game session (default session length is ~ 3 hours).  When a player finds his or her quarry and scans a game-specific QR code on that person's attendee badge, the quarry is eliminated from the game.  However, in this event both players are encouraged to strike up a conversation about what brought them to the conference, as their meeting has been serendipitously orchestrated by the dapp to develop and strengthen connections within the community. 

Every player seeking a quarry is also assigned as another player's quarry ("the pursuer" from the original player's perspective).  Players do not know who their pursuers are, but they are provided the name of their pursuer's pursuer ("the ally" from the original player's perspective).  Allies allow for defensive strategies to help identify or eliminate the threat to the player, because if the pursuer is eliminated before reaching his or her quarry, the quarry stays in the game.  This second piece of information allows for a new potential serendipitous contact, and another community connection.  

Provided only with the names of their quarries and allies, players may conduct internet searches to try to learn more about what those two players look like, who the work with and whether they share common connections in the community that might be worth finding to gather intel or make connections.  

## Outcomes
At the conclusion of each session, a player will fall into one of the following outcome categories:
* Quarry found, Pursuer did not find quarry -> ADVANCE
* Quarry found, Pursuer found quarry -> ELIMINATED
* Quarry not found, pursuer did not find quarry -> ELIMINATED?
* Withdrew -> ELIMINATED

Players can withdraw from a game of Quarry at any point for any reason, which has the same effect as being found by a pursuer within the game.  Upon withdrawal, the pursuer will be notified.

### Session Advancement
Only players who behaved in certain ways during a session advance to the next session.  The specific advancement rules can be customized, but a default game might require that a player both avoid being eliminated and also eliminate their quarry in order to advance.  This second requirement would deter hiding as a stratagem.  Players are quickly notified if their pursuer is eliminated during a session.  If a player has found his or her quarry and his or her pursuer is eliminated midway through a session, that player is done for the remainder of the session.

### Final Session
Rules are distinct for the final timed session in order to determine a single winner.  Each remaining player receives the name of two quarries at the start of the final session, but does not receive any ally information.  Found quarries are replenished with new quarries so that a player always has two quarries.  At the conclusion of the final session, assuming more than one player remains in the game, the player with the highest numebr of found quarries is the winner.  Ties are broken by the shortest total time spent seeking quarries during the first three sessions. 

### Example of Devcon V Quarry Game
When registering, Devcon V attendees would indicate whether they wished to play Quarry at the conference, with a link to an explanatory website and/or video.  Those attendees who opted to play would be added to the participant pool and would have a special Quarry QR code printed on both sides of their printed ID badge.

Assuming that Devcon V runs at least 3 days, there would be two standard Quarry sessions that would run from noon to 3:00pm on the first two days of the conference, and a final session on day three that would run from noon until 2:00 PM or until there are only three players remaining (who would each have the names of the other two as quarries).  Players that make it to the final session would have to check in at the conference before the start time in order to be eligible to play.

Assuming 1,000 attendees register to play, we estimate that only 100 or so would advance to the second session, and that 25-30 would participate in the final session.

## Norms
Players should follow the Golden Rule of Bill & Ted : Always be excellent to each other. In particular:
* Don't behave aggressively (either physically or emotionally) toward anyone during a game of Quarry
* Always be polite and don't interrupt people in the middle of a conversation
* Don't hide - winning the game is not worth missing the opportunity to interact with the community
* If you are found by your pursuer, don't be a jerk and try to block your QR code.  See it as an opportunity to grow your community.  Imagine being the person who answers a panel question about how a successful partnership was formed by beginning "We actually met when Alice found me as her quarry at Devcon V and we starting talking about ..."
* Only play Quarry in the hallways and common areas - sessions are long enough to give everyone a fair shot
* Talks and workshops are out of bounds. So are bathrooms.  Don't disrupt these environments for a silly game.

## Proposed Implementation
Each Quarry game requires an administrator, who is responsible for 1) setting the participant pool, 2) setting and communicating the dates and times of the Quarry sessions, 3) communicating how the game works to the participants, explaining the behavioral norms expected to make it a fun and productive experience, 4) monitoring the sessions and resolving issues as they arise, including disputes among players and technical issues with on-chain game transactions, and 5) announcing the winner.

