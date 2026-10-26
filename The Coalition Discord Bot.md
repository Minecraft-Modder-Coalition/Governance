The Discord bot for the Minecraft Modder Coalition has a defined scope of its capabilities. Its purpose is to collect votes for measures in a way that is transparent and fair. To that end, this document outlines the way that this bot should operate, with the details being left to coalition members to implement via contributions to a separate public repository hosted by The Minecraft Modder Coalition. The bot should be hosted on a server owned by The Minecraft Modder Coalition

The Discord Bot should:
- Allow any member to call a vote of the entire coalition
	- A vote should allow for 2 different kinds of measures:
		- Coalition leadership elections
			- Members must be able to vote for, at most, the total number of available seats for a leadership position. Members may vote for 0 members to signal a present vote for no members.
		- Coalition action proposals
			- Members must be able to vote in the affirmative, in the negative, or present.
	- Votes may contain more than 1 measure if multiple proposals have concluded debate, or if an election happens around the time debate concludes.
	- A snapshot of the current, eligible, members should be taken at the time the vote is created should be made. The "total number of members" should be taken from this snapshot amount
	- A vote can only pass if a quorum of 50% of the total number of members is met. If a quorum is not met 1 week after the vote is called, an automatic extension to the vote by the bot occurs.
	- If after 4 weeks a quorum is not met, the vote fails.
	- If after a quorum is met and at least 50% of the non-present votes are in the affirmative, the vote passes.
	- The results of how many members voted should be public at the conclusion of the vote, but how people voted should be private.
	- The bot should be developed in a way to maintain the secrecy of how people voted