# 100 Days Of Code - Log

### Day 0: October 12, 2018


**Today's Progress**: I watched the [youtube series about Mastodon bots by Daniel Shiffman](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6byiVX7_Z1rclitVhMBmNFQ) and built my own [first bot](https://botsin.space/@peotry).

**Thoughts:** It was fun to see the bot tooting its first toots. When I am watching videos from Daniel Shiffman, I usually do not follow them 1 to 1, but tend to take other turns or think a little ahead, sometimes. So this time I found a solution for the problem of versioning the bot, but keeping the access tokens hidden, before it was mentioned in the video. Because of that, I did it different and now I am not sure, which of the solutions I like better.
The Coding Train video show the usage of the [dotenv](https://www.npmjs.com/package/dotenv) library, which seems to be the standard tool for this job. I did not use any library. But the code I wrote is not really more complex than the code to use the library, so why use a library? I just put the tokens in a file called tokens.js, exporting them into one object. This can then be required and used in the project. tokens.js is blocked from versionioning via gitignore and instead there is an empty file, as an example, for people who want to use the bot for their own accounts.

**Link to work:**

* [Sourcecode for the bot](https://github.com/doxanthropos/peotrybot)
* [Robotic Peotry](https://botsin.space/@peotry) My bot in the wild of [Bots in Space](https://botsin.space/)

### Day 1 and 2: October 13 + 14, 2018

**Today's Progress:** I read a lot about generating texts through programming and am not really sure about the way I will choose to take with my mastodon bot (which is still trying to find the answer to life, the universe and the rest, please do not spoil him).
A pure Markov Chain based approach will probably not produce texts that look like poems, there needs to be some predefined structure. Therefore I read the second chapter of [Paradigms of Artificial Intelligence Programming](https://github.com/norvig/paip-lisp) and tried to create a similar sentence generator in JavaScript.
I also tried to fix a missing part of the yarn documentation.

**Thoughts:** There is a saying: "one can write Fortran in any language" and I think here I have experienced something similar with Lisp. While the solution to building sentences from Peter Norvig looks objective and only driven by the rules of the english language, but still it is written in Lisp. In trying to do something similar in JavaScript, I ended up using a lot of lists in many places.

**Link to work:**

* [Sentence generator](https://gist.github.com/doxanthropos/9c0fdfe42fe1ef664c8690013732d3fb)
* [yarn documentation PR](https://github.com/yarnpkg/website/pull/873)

### Day 3: October 15, 2018

**Today's Progress:** Been away from the computer for a long time today and listend to some episodes of the [Base CS Podcast](https://www.codenewbie.org/basecs) on the train. Back home I tried making something resembling a poem out of my sentence generator, that I built yesterday. Now my generative poet toots two sentence poems.

**Thoughts:** After having a sentence generator that produces purely random sentences, it was quite easy to reduce the randomness in a selected part to give the two sentences of the poem something in common.

**Link to work:**

* [Commit for today](https://github.com/doxanthropos/peotrybot/commit/13815fac4490a9bdb81c5889ad1d002d1e55f190)

### Day 4: October 16, 2018

**Today's Progress:** While I am still not sure how to proceed with the bot, I did some FreeCodeCamp challenges. I started with the API and Microservices part and learned how to use (on a very basic level) express for JavaScript back end programming and how SemVer works.

**Thoughts:** Since these challenges are not really my own project, doing them feels a lot less productive. I learned a lot, but I think I will go onwards with at least some time spent on own projects every day.

### Day 5: October 17, 2018

**Today's Progress:** Like on day zero, I followed a video from Daniel Shiffman and built something on top of that. [He made a nice video about seven segment displays](https://www.youtube.com/watch?v=MlRlgbrAVOs) and I made a clock with that.

**Thoughts:** Had some fun with p5. I think this code could use some refactoring, but I am OK with the existing functionality.

**Link to work:**

* [7-Segment Clock](https://doxanthropos.github.io/sketchbook/2018101701/)

### Day 6: October 18, 2018

**Today's Progress:** Watched [another video of Dan Shiffman](http://thecodingtrain.com/CodingChallenges/085-the-game-of-life.html), this time the one on [Conway's Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life) in [p5.js](http://p5js.org/). As usual, I followed a bit, then did something on my own. It is working, but I will change it a little tomorrow to allow the visitor to change the state of the cells, so one can paint the nice structures that are possible on this.

**Thoughts:** While going for a wraparound before Dan did, I encountered more then one of the famous "off by one" errors that so easily can happen. Getting the wrapping via modulo right was a lot harder for me than for Dan Shiffman in the video, even after I basically had the same idea to do that, that he also used.

**Link to work:**

* [Game of Life v1.0](https://doxanthropos.github.io/sketchbook/2018101801/)
* [Sourcecode](https://github.com/doxanthropos/sketchbook/tree/master/2018101801)

### Day 7: October 19, 2018

**Today's Progress:** I took the Game of Life from yesterday and implemented some ways for the user to interact with it. Now it is possible to pause and resume, to change the state of the cells and to speed up and slow down.

**Thoughts:** Refining was quite an enjoyable process. I was able to think about what would be fun and make the site interesting. 

**Link to work:**

* [Game of Life v2.0](https://doxanthropos.github.io/sketchbook/2018101901/)
* [Sourcecode](https://github.com/doxanthropos/sketchbook/tree/master/2018101901)

### Day 8 and 9: October 20 + 21, 2018

**Today's Progress:** Have been travelling on the weekend without my computer, so was only able to read, to go on with this. Read about c programming and networking.

**Thoughts:** Not sure how to cope with days like these in this challenge. Does reading count? I think I am finally getting things like malloc, free and so on in my head.

### Day 10: October 22, 2018

**Today's Progress and Thoughts:** Making a 3D version of the Game of Life made my old little laptop overheat seriously, at least with p5. so I thought: why not do that in Processing? Compiling before running the code should take some load off the laptop. But I have never done 3D with Processing and no Processing until now on this machine. So I spent some time configuring [Emacs for using Processing](https://www.emacswiki.org/emacs/Processing) and figuring out how to create a sketch that will actually compile. In the end I was able to follow the short video on [Coding Challenge #101 from Daniel Shiffman](http://thecodingtrain.com/CodingChallenges/101-may-the-4th.html) and make that run from inside Emacs.

**Link to work:**

* [Today's commit](https://github.com/doxanthropos/sketchbook/commit/4581ad95432bc68b3f2b312e2e0dd7b8536f4e15)

### Day 11: October 23, 2018

**Today's Progress:** I saw that there was a new [Coding Challenge Video](https://thecodingtrain.com/CodingChallenges/119-binary-decimal-conversion.html) online, so I had to watch it and code along. Based on the code from this video, I built a sketch that converts ascii characters to their binary code and visualizes this binary code.

**Thoughts:** This was fun. I choose to go for the green on black design from the 7-segment clock, because it provides a fitting retro look. I worried that I would have to write a function to convert decimal numbers to a binary number string, but luckily the JS function "toString(2)" with the 2 for the base, does just that, so I only had to pad the zeros on the left. Of course writing it would not have been difficult (that would have been a good use of the modulus operator), but not that much fun.

**Links to work:**

* [Ascii to Binary Visualization](https://doxanthropos.github.io/sketchbook/2018102301/)
* [Source](https://github.com/doxanthropos/sketchbook/tree/master/2018102301)
