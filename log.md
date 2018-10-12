# 100 Days Of Code - Log

### Day 0: October 12, 2018


**Today's Progress**: I watched the [youtube series about Mastodon bots by Daniel Shiffman](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6byiVX7_Z1rclitVhMBmNFQ) and built my own [first bot](https://botsin.space/@peotry).

**Thoughts:** It was fun to see the bot tooting its first toots. When I am watching videos from Daniel Shiffman, I usually do not follow them 1 to 1, but tend to take other turns or think a little ahead, sometimes. So this time I found a solution for the problem of versioning the bot, but keeping the access tokens hidden, before it was mentioned in the video. Because of that, I did it different and now I am not sure, which of the solutions I like better.
The Coding Train video show the usage of the [dotenv](https://www.npmjs.com/package/dotenv) library, which seems to be the standard tool for this job. I did not use any library. But the code I wrote is not really more complex than the code to use the library, so why use a library? I just put the tokens in a file called tokens.js, exporting them into one object. This can then be required and used in the project. tokens.js is blocked from versionioning via gitignore and instead there is an empty file, as an example, for people who want to use the bot for their own accounts.

**Link to work:**

* [Sourcecode for the bot](https://github.com/doxanthropos/peotrybot)
* [Robotic Peotry](https://botsin.space/@peotry) My bot in the wild of [Bots in Space](https://botsin.space/)
