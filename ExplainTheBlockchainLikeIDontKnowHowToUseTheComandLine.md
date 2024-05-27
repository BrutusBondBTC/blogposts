Definitions:

**Blockchain**- A word used to confuse people into buying scams instead of store their wealth on the bitcoin time chain.

**Nonce**- A number used only once.

**mempool** - each bitcoin node has a pool of transactions in memory. These transactions are waiting to be included in the limited space(2mb) of a bitcoin block. Miners are incentivized to include transactions that pay the highest fees before including transactions that pay lower fees.

**coinbase transaction** - The name given to the block reward which is the block subsidy, plus the fees. After the last sat is mined the coinbase transaction will be fees only.

**hashcash** -- an anti-spam tool discovered by Adam Back that  Satoshi Nakamoto cited in the white paper. 

**hexadecimal**  a number system where:

0 = 0
1 = 1
2 = 2
3 = 3
4 = 4
5 = 5
6 = 6
7 = 7
8 = 8
9 = 9
a = 10
b = 11
c = 12
d = 13
e =14
f = 16


## What Is The Bitcoin Time Chain?




The time chain describes the chain of blocks of the bitcoin network. At the time of this writing, there are 793,474 blocks on the bitcoin timechain. You may have heard a new block is created every ten minutes.  This is because the software is programed to create a new block every ten minutes on average. This will be my starting point, because it is necessary to understand this to understand how we know why the last sat will be mined sometime around the year 2139.

![Difficulty Adjustment](https://nostr.build/p/nb10615.jpg)

In [Bitcoin Clarity](https://getbitcoinclarity.com/), Kiara bickers compares the difficulty adjustment to rolling dice. Imagine if you rolled a single die 6 times per hour.  Each time you rolled a 1, you earn 50 cents.  You would expect to roll a 1 once every 6 times or 16.6% of the time.  Maybe you roll a 1 in the first 20 minutes the first time, but in an hour and 40 minutes the second time, but over a large number of trials you would expect to earn 50 cents every hour on average.  

Say Alice joins your game. You both roll the die the same amount of times per hour and every time she or you roll a 1, one of you earns the reward. Now the game rewards $1.00 every hour on average.  Now the Pit boss says, Wait a minute, We need to change the odds of our game. Now the second person who rolls a 1 gets the $0.50 reward. This is a difficulty adjustment and the Pit Boss goes back to paying fifty cents per hour.

I love this explanation because it's a simplified version of a complex concept. I played a lot of poker before bitcoin and read a lot of poker books. One of my favorite books was the Mathematics of Poker, by Bill Chen and Jerrod Ankerman. This book used toy games to simplify the game theory of poker. I view Bicker's dice example as a similar toy game that describes the difficulty adjustment in succinct terms. My goal is this blogpost is to explain the game theory and chain of blocks using hashcash as an example because it is easier than describing the double SHA256 hash the actual bitcoin network uses.



### How Does The Bitcoin Time Chain Work?
We have all heard Satoshi put "Chancellor on the brink of second bailout for banks." I love that quote, but we will ignore this in this blog.  Instead, we will focus on the header of the genesis block.  this is what it looks like on  [Blockstream's node](https://blockstream.info/block/000000000019d6689c085ae165831e934ff763ae46a2a6c172b3f1b60a8ce26f)  


![genesisblock](https://nostr.build/p/nb10470.png)

I will ignore most of the information you see here like the timestamp virtual size, merkle root etc. If you want to learn about these things, read [Programing Bitcoin ](https://programmingbitcoin.com/) by Jimmy Song.  Instead, I'm going to focus on just the block headers using SHAmory cards.

![genesis block](https://nostr.build/p/nb10624.jpg)

I like these cards because they abstract all the complexity away while still leaving the important stuff in a fun, way that's simple enough for a child to see.  Take note of the leading hex zeros in the genesis block. Finding a hash with the key amount of leading hex zeros is key to unlocking miner rewards.  


Let's look at SHA256 in action.  It's simpler than you think. 

Copy and paste the word bitcoin into the unpopular search engine, https://www.duckduckgo.com.   You can type it out yourself or copy and paste it below.

`sha256 bitcoin`

You'll see this SHA-256 hex hash:

6b88c087247aa2f07ee1c5956b8e1a9f4c7f892a70e324f1bb3d161e05ca107b

This is the hash of bitcoin. According to the computer, each character you type represents a number. SHA-256 does some math and creates a new number.  These numbers are not base 10 or binary. They are **hexadecimals**.   We can't do this calculation in reverse. Each output in SHA256 results in 64 hexadecimals weather you hash the letter "a" or War and Peace.

Now let's do the hash of bitcoin1.

`sha256 bitcoin1`

dbdbac0b3072d7677fc94eebaf8eba9e81e5c3b7de6899dae12c98d6799b065a

We only added one more digit, but have a completely different output.

In a way,  each possible combination of letters, characters, and numbers have a separate identity based on this math. I is always 64 characters, but never the same as any other combination of characters.(for all intents and purposes).

* a = ca978112ca1bbdcafac231b39a23dc4da786eff8147c4e72b9807785afee48bb
* b = 3e23e8160039594a33894f6564e1b1348bbd7a0088d42c4acb73eeaed59c009d
* the bitcoin genesis block =

![gen block](https://nostr.build/p/nb10624.jpg)

The genesis block is chained to the identity of block 1  because block one is a hash of all the transactions and this header with 10 leading hex zeros.

When the next number that produces a certain number of leading hex zeros, the two blocks are chained together forever.


![](https://nostr.build/p/nb10662.png)

 <video width="320" height="240" controls>
  <source src="https://nostr.build/p/nb10627.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video> 

  This happens about every ten minutes. At any given time, it goes faster or slower, but it adjusts back to ten minutes every 2,016 blocks.(two weeks)The reward is cut in half every 210,000 ten minute blocks(almost exactly every 4 years) It's beautiful. I almost feel like it's akin to a monument like the Washington Monument or Lincoln Memorial, but built with computers instead of concrete and getting higher and higher every ten minutes.  The news talks about rock jpegs worth millions of dollars, but they never notice what a mathematical work of art bitcoin is.

![supply](https://nostr.build/p/nb8729.png)



#### How Mining Works.

To show you how mining works, it is impracticable to do a double SHA-256 hash of the genesis block. Since mining was based on Adam Back's hashcash, we can use hashcash to illustrate how it worked. 

Hashcash uses SHA1 and has a 40 character hex hash, but it is similar enough to demonstrate what happens in the bitcoin mining process.

Hashcash worked by hashing emails. some other data, and a nonce.  

For example, copy and paste the following into duck duck go.


`sha1 0:030626:adam@cypherspace.org:6470e06d773e05a7`



* Let "0:030626:" represent the previous bitcoin block hash.

* Let "adam@cypherspace.org:" represent our transactions. 

* Let "6470e06d773e05a7" represent our nonce.

Real bitcoin miners are hashing gazillions of times per second, but our toy game model is meant to simulate how this works in two hashes.

The first hash gives us.

73f88e0645f8ca92ef3a0bc02ef4b7edf85fadbd

That sucks because we are looking for 8 leading hex zeros. Like the pit boss required two 1's to win..  Instead of dice, however, the difficulty is adjusted by adding or removing  leading hex zeros. This is a little inaccurate, but gives us the basic idea of what is adjusted in the difficulty. When you hear the difficulty adjustment has gone up, this means there are more zeros required. If the difficulty adjustment goes down, there are less zeros. Again, this is a bit oversimplified, but gives us the basic idea.

Next we will try hashing this by typing it into duck duck go. Notice how we only changed the last digit of our nonce by adding one.

`sha1 0:030626:adam@cypherspace.org:6470e06d773e05a8`

Now we have the eight leading zeros we we searched for and our rewarded the block subisdy and any fees that were in this block we mined.

00000000c70db7389f241b8f441fcf068aead3f0

#### Why It Matters?

I hope this is obvious, but I didn't actually figure this out myself.  I used Adam Back's documentation which can be found here:

http://hashcash.org/docs/sha1-hashcash.txt

He's a real cryptographer, like a mathematical graffiti artist.  I'm just a fan boy. Hashcash is an interesting rabbit hole in and of itself and I think this math is essential to understanding the bitcoin base layer, but it's not like you need to do this math with a pen and paper, It can be done with a search engine available to anyone with an internet connection. 

I wrote this to teach non-technical people how the math of the bitcoin timechain works as simple as possible, but this is a work in progress. If you think I can make it even simpler, let me know. If you are a real cryptographer and notice any mistakes I made, also let me know. I want to keep iterating at this and make it as easy to understand as possible.

This is math, Some people say it is pointless math. Some say it's a waste of energy.  Some want to tax people for doing this math and broadcasting the results of those math problems to other people checking those math problems. This matters because we the people deserve to have freedom of speech. We have the right to perform calculations. We have the right to tell others of our results. Taxing math is an abhorrent idea, much worse than the idea of taxing pysical goods like tea.  A tax on the energy used to do math, no matter the source,  is a tax on reason itself. This math is not taught in public school.


![the Problem](https://nostr.build/p/nb10670.png)

**The math of bitcoin is important because the math of fiat does not work.**  Can you retire on social security  or do you think your pension will be there for you when it's time to collect?  Do you think your children can save a decent down payment for a house in a savings account that pays 0.01% per year? Do you think the FDIC has enough money to cover many more bank failures with the1% in fees they collect? Are micropayments possible?  Are identity thieves and retail bandits considered employed or unemployed? Do you know what happened in 1971? 

**Run the numbers or the numbers will run you.**




The post where satoshi describes the problem with digital money can be found here:  http://p2pfoundation.ning.com/forum/topics/bitcoin-open-source


Thanks for reading.

Also shot out to Scott from [SHAmory](https://shamory.com/) I asked him if I could use pictures of his card game and he graciously agreed. Have you ever seen a blogger say, I recommend product x because I use it and I would recommend it even if they didn't pay me?  That's what this is. It is not an ad, he did not pay me to shill his card game, but I recommend it anyway.  It's meant to teach kids how bitcoin works and I think that's an excellent idea. The kids our the future. Teach them well.




Blogging Bitcoin

npub1wkljx5c6a8uccc5etws8ry0y3r4dgavh2dcav0tal4rtmcdl4z2sfu5u0t

----


Block Height: 793,610

To pledge your support, please visit my [Value 4 Value Page](https://bloggingbitcoin.store/apps/cd4EUVkfhWbTg5UZsbCJPi5ghxZ/pos), send a zap, or scan this QR Code with lnurl compatible lightning wallet.


![lnurl](https://nostr.build/p/nb8272.png)

[Other ways to support the blog](nostr:note1a0av06dvr3hrvjjlz5ezqnpd3m4w6tf8scp6rw9edcgct7pu57yq96m4qx)



**[Subscribe on Substack](https://bloggingbitcoin.substack.com/p/subscribe).** I don't have a paid subscription. It just sends you an email when I write a new blog.  You can also just look at my profile on [habla.news](nostr:nprofile1qqs8t0er2vdwn7vvv2v4hgr3j8jg36k5wkt4xuwk847l634auxl639gpzfmhxue69uhhqatjwpkx2urpvuhx2ucpp4mhxue69uhkummn9ekx7mqpremhxue69uhkummnw3ez6un9d3shjtnwda4k7arpwfhjucm0d5q3yamnwvaz7tm0venxx6rpd9hzuur4vgq3gamnwvaz7tmjv4kxz7fwv3sk6atn9e5k7qgswaehxw309ahx7um5wgh8w6twv55veszj)








---------

