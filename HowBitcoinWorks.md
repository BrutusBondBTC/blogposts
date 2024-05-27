
### What Is Bitcoin

According to [Pablo Xannybar](note1zaypcyvnvczw5lek6ge20vz0am8l8rp9t9ltl0wcyy308feazs6sl4af0n) Bitcoin exists outside the control of nation states, as well as central investment, and commercial banks, or any other single third party[--It is money ruled solely by code, mathematics, and compute power, not a government or any other body of fallible humans."](https://highlighter.com/e/note1zaypcyvnvczw5lek6ge20vz0am8l8rp9t9ltl0wcyy308feazs6sl4af0n) This is important because the peer-to-peer electronic cash system does not have a central point of failuresince bitcoin is a  peer-to-peer electronic cash system; a system built on distributed computer networking instead of a centralized third party. This is different from almost all technology most people use in their day to day lives. Apple is the biggest technology company in the world. It has many servers all around the world.  Your data on the Apple cloud is protected from natural disasters because Apple has backups all over the word.  To be honest, I have assume someone else has seen it.not verified this, but I don't imagine the Apple cloud is just running on a laptop in somebody's closet. If one of Apple's server breaks, your data will surely  survive.  

They say this cloud is secure, yet somehow [naked celebrity pictures get hacked from the iCloud](https://www.cnet.com/tech/mobile/how-nude-photos-leaked-protect-icloud-account-security/) and the [FBI can break the iCloud encryption](https://www.washingtonpost.com/technology/2021/04/14/azimuth-san-bernardino-apple-iphone-fbi/).  To be fair, bitcoin stored on hot wallets can also be hacked. If you type a seed phrase onto an Internet computer, [assume someone else has seen it.](https://en.wikipedia.org/wiki/PRISM)  That's why most Bitcoiners advise to only keep a small amount of your stack on a hot wallet. That's why governments don't like "unhosted wallets." Unhosted wallets are a euphimism for big  random number the government can't guess. Their Internet surveillance doesn't work on a calculator plugged into a 9v battery inside a shed at the middle of nowhere. This is also why we can rest assured that the bitcoin we keep in cold storage can be safer than even data kept on the servers of the biggest companies in the world.

### Bitcoin Full Nodes Keep The Network Decentralized


Imagine if there was only one person running a bitcoin node. This node verified all the transactions on the network. If the power went out or if it got droned,  bitcoin would die. There would be no record of the bitcoin time chain anymore. Nobody would verify transactions. There would be no network to broadcast to.

![singleNode](https://cdn.nostr.build/p/P4L0.png)

What if there are 17,000 bitcion nodes. Let's say my node gets droned. Bitcoin is still alive like Eddie Vedder. There are still 16,999 nodes validating transactions all over the world.  Maybe one bitcoin node dies every now and then, but there are more peers on the network. They are distributed all over the globe. As long as several nodes remain on the network, bitcoin will not die.  

![earth](https://cdn.nostr.build/p/W49k.jpg)

The same is true of miners now that mining bitcoin and running a node are not the same thing.. We only need one bitcoin miner for the network to work. Of course, if that miner gets droned or a government tells it to censor transactions bitcoin would not make it.  Miners mine bitcoin blocks all over the world .  These people maintain the rules of the bitcoin network no matter what the drone pilots do. This means the bitcoin network is not at the mercy of a single government. Governments could shut down exchanges, but they cannot shut down the bitcoin network. 

Bitcoin will be alive as long as many humans run the software on computers. Some will mine, some will run full nodes that validate every transaction since the genesis block. There are  thousands maybve tens of thousands of nodes like this in the world. For bitcoin to die, all of these nodes would need to die. A node is just a computer running the bitcoin software. I won't say this is impossible, but I remain optimistic that even the most evil of nuclear armed, drone wielding governments will not destroy all the bitcoin nodes in the world. 


### What Is A Bitcoin Wallet?

A bitcoin wallet is created using elliptical key cryptography.  I just like to call it a **big ass random number**. The goal of this chapter is not to make you an expert on eliptic curve cryptography. If you want to learn how to do the math like an OG cypherpunk, take some discreet mathematics classes. WAtch the MIT Cryptography course and read Jimmy Song's book, Programing Bitcoin. The purpose of this chapter is to teach you how the math of bitcoin works without learning to program or earning a bachelor's degree in applied cryptography.  I won't teach you how to do SHA256 using a pencil and paper or the command line interface. We will use tools available to anyone with an Internet connection instead. If you are interested in learning a bit more about eliptic curve cryptography, LN Capital has a pretty good thread about it on the [dead bird app](https://twitter.com/LN_Capital/status/1685654004745809920)

To create a bitcoin wallet, we can hash some random data or we can create a 256 bit number using dice rolls. We could also flip a coin 256 times to get 256 bits.  Say heads =0 and tails=1.  We get a 256 bits f 1's and zero's that computers sees as a totally random, almost impossible to guess number. According to [Yan Pritzker,](https://www.inventingbitcoin.com/) in Inventing Bitcoin you have about the same chance of guessing a bitcoin private key as winning the Powerball 9 times in a row. Your bitcoin seed is a tiny needle in the haystack called the all of the atoms in the universe.  If you would like to learn how to make a bitcoin wallet the hard way, check out [armantheparman's article](https://armantheparman.com/dicev1/), but in the next chapter, you will learn how to make a bitcoin wallet using Padawan.  Padawan only uses testnet bitcoin and they give them to you for free. If you F up your Padawan-have no fear. Testnet bitcoin is for practicing and it's not worth anything.

### What Is Mining?

![orangeRubix](https://cdn.nostr.build/p/jAn9.png)



Bitcoin mining is the act of applying the SHA256 algorithm to .  People often compare bitcoin mining to solving a puzzle. This is not wrong. I think of it as  a mathmatical Rubix Cube of sorts, but no analogy does bitcoin mining justice.. During the government mandated lockdowns, my wife became quite adept at solving Rubix Cube.  She watched a YouTube video that taught her how to solve it using an algorithm.  It helps to visualize the SHA256 as a way of twisting a Rubix Cube in a certain pattern. Each twist gives a different result, but you spin and spin until all the colors match on each side. The Secure Hash Algorithms work in a similar way, except with numbers instead of colors. unfortunately, like all analogies, this Rubix Cube analogy doesn't tell you much about how bitcoin mining works.  The best way I can descibe it is like a Rubix Cube with letters and numbers. I dont know how to solve a rubix cube, but my wife says she uses an algorythym. SHA256 is also an algorithym , but instead of creating sides with uniform colors. it searches for a random number with a certain amount of zeros in the front of it.  All the other numbers and letters look random, but the zeros of a block do not look random, do they.

![801416](https://cdn.nostr.build/p/89jz.png)
 
 ### On SHA256

According to Satoshi, "Writing a descreiption for this thing for general audiences is bloody hard, Theres nothing to relate it to." Everyone tries to explain bitcon by analogy like I just did with the rubix cube.  Although this was the best visual representation I cold think of, it's still not perfect. I believe there is something in the world bitcoin can be compared to, back then, you had to be a real cryptographer like Adam Back to see it. Adam Back was cited in the white paper because he discovered a way to prevent spam, hashcash. Hashcash is an electronic stamp of sorts. You can use the command line to see how it works if you want to do it the hard way, but the easy way requires https://www.duckduckgo.com.  To learn  how SHA256 works , we will perform SHA256 on the lowercase letter "a" by entering the following into DuckDuck Go:

`sha256 a`

You will receive this result:

ca978112ca1bbdcafac231b39a23dc4da786eff8147c4e72b9807785afee48bb

Notice how** even though we only did a sha256 hash of one letter, we still get a 64 character hexadecimal number**. If we add the number 0 to the letter a, `sha256 a0` we get the following hash:

4e1195df020de59e0d65a33a4279f1183e7ae4e5d980e309f8b55adff2e61c3e

If we add the numbver 1, `sha256 a1`, we get:

f55ff16f66f43360266b95db6f8fec01d76031054306ae4a4b380598f6cfd114


There is no other output to each of these because each change no matter how large or small gives us a different output.  That's why a number is only used once in the mining process. This is called a nonce. It makes sense. You can almost deduce the meaning by the sound of that word in the same way nobody ever had to explain to you what the word "sharted" means.







We can also has letters and any character on the keyboard. You may have heard computers only understand 1's and 0's. This is true at the base layer of the machine. but the bitcoin blockchain uses hexadecimals and all kinds of text in the transactions. This is because each character on your keyboard is represented by a number so you could do these mathmatical calculations on text like this. 

`sha256 Blogging Bitcoin`

You will see the following SHA-256 hash digest:

965aef3b925ed3d5b5315906e49a4956863528be3bfeaa357a62be6b74def0a0



If we SHA-256 Chapter 8 of George Orwell's 1984 we get:

7d7c0aad69d213e113fbaa53be74f0f88f98791c79fe44f6adb809e0787654e3

If we SHA-256 the book, War And Peace, we get:

8e09cbbbc608d61fb61f012819259987a7399351aaffb1c1790c88f134ec840e

By the way, War And Peace is a big book. it's easier to hash it by using https://xorbin.com/sha256-calculator instead of duck duck go. I copied and pasted evertying from here.  **https://www.gutenberg.org/cache/epub/2600/pg2600-images.html**  The intetresting thing aout SHA256 is that **you always get a 64 character output weather you has a single letter or a huge novel**.   If you change one character, you get an entirely new 64 character output that looks nothing like the previous output.




Notice how **each one of these gives us 64 unique hexadecimal numbers, no matter how small or large the amount of data being hashed is**.

**We would not make a bitcoin wallet out of a novel because anyone with that novel can take our bitcoin** We want to use **random numbers** to make our bitcoin wallet. The purpose of writing this is to show you that anythhing from a single letter to a large book can be hashed into 64 characters.  


The math is a little complicated, but I [highlighted it here](https://highlighter.com/e/note1dn9t3727qnml6fwfvxt4xpzhszelfctt9y2jar98egy4purptjrq4xdeny) in case your interested, but the War And Peace  number is actually this:

92,013,536,190,004,391,427,498,867,800,243,235,304,388,826,599,257,256,328,980,806,975,182,967,533,301

We will make our first bitcoin wallet in the next chapter, but before we do, let's talk more about mining?

### How The F$@$% Does Bitcoin Mining Work?

Just like I can hash War and Peace, bitcoin miners can hash all the data in the bitcoin mempool.  In other words all the transactions sent since the last block. [Here's a good visualization](https://bitfeed.live/) of how it works. All the falling orange squares represent transactions that go into the mempool. These orange squares are really text. Miners hash this text with a nonce.  They are also more likely to hash transactions that pay a higher transaction fee than transactions that pay a lower trasnsaction fee since these transaction fees are part of the reward for solving the puzzl.  All the miners all over the world do this trillions of times until one of these nonces produces a number with a certain number of leading hex zeros. 


 https://cdn.nostr.build/p/nb10627.mp4


Bitcoin actually uses a double SHA256 hash to make it more secure. This also makes it more complex to explain, but we are going to demostrate it using a simpler Secure Hash Algorithym, First, let's look at the the SHA-256 hash of War and Peace again.
 
 8e09cbbbc608d61fb61f012819259987a7399351aaffb1c1790c88f134ec840e
 
 Now we will hash the entire text of war and peace plus a number we will only use once. The number could be anything, but we will use the number 0.  In other words, we append War And Peace by adding a zero to the end of our text
 
 "...This website includes information about Project Gutenberg™, including how to make donations to the Project Gutenberg Literary Archive Foundation, how to help produce our new eBooks, and how to subscribe to our email newsletter to hear about new eBooks.0" 
 
 We get this hash
 
 e5a1d7ce9bb2d1c3450c7149633ddd3738a8f88e93457fb46df32c312361f0b4 Which is much different from:
 8e09cbbbc608d61fb61f012819259987a7399351aaffb1c1790c88f134ec840e 
 
 Yet, we only changed one out of thousands of characters.
 
 Now we will replace the Number Only Used Once, **0** with a new number we will only use once,**1**  and get this result:
 c600f3e297f850a1b5e4620b0719556a4f7b1e3614875bbe083a31ad84c40367
 
 
 
 
** TK video of this using https://xorbin.com/tools/sha256-hash-calculator** 
 
 
 ### How This Works In Bitcoin

I could keep adding new nonces uWell, I can't, but an ASIC miner can. eventually I will get some cool looking result that has **0000000000000000000** in front of it. I can't do this by hand and it would be a waste of energy to hash War and Peace over and over again with a new number until we get a number with a certain number of zeros in front of it, but that's not the easy way of demonstrating things.

Bitcoin mining is just a souped up version of hashcash I mentioned earlier in this chapter Satoshi referenced hashcash in the white paper because the bitcoin blockchain is simmilar to hashcash, with a few differences. Hashcash uses SHA-1.  Bitcoin uses a double SHA-256 hash which means it actually does it twice. The specifics are beyond the scope of this book, but hashcash is a little different.

I previously stated that we can hash any data from a single letter to the novel war and peace.

I have also demonstrated that if we add just one single number to all that data again and again, we will recieve a different result every time.

The zeros I told us are the answer to the puzzle miners are looking for.


For example, the header of the Genesis block, or block 0, is:

000000000019d6689c085ae165831e934ff763ae46a2a6c172b3f1b60a8ce26f

Block height 1:
00000000839a8e6886ab5951d76f411475428afc90947ee320161bbf18eb6048

block 210,000
000000000000048b95347e83192f69cf0366076336c639f9b7228e9ba171342e

Block height 700,000:

0000000000000000000590fc0f3eba193a278534220b2b37e9849e1a770ca959

Like I said before, **the leading hex-zeros are like the colored sides of a Rubix Cube**. The software adjusts so miners find the answer to this puzzle every 2016 blocks.  We say it is two weeks because, on average, there are 6 ten minute blocks in an hour. If blocks come too quickly, more zeros are required. If they come to slow, less zeros are required. This is a little more complicted than this, but this is the easy way of explaining **The Difficulty Adjustment.**

There are 144 ten minute blocks in a day, 1008 blocks in a week and 2016 bloks in two weeks. Pretty neat, huh?

### Hash Cash--The Easy Way

![hashcash](https://cdn.nostr.build/p/89Xg.png)

You can see how this works by using hashcash, a sort of digital stamp discovered by Adam Back. Back used SHA1. I found some interesting things while perusing the the hashcash documentation.  Hash the following in either [duck duck go ](https://duckduckgo.com/)or [xobin calculator.](https://xorbin.com/tools/sha1-hash-calculator)

0:030626:adam@cypherspace.org:6470e06d773e05a7

----

Imagine "**0:030626" is the header of the previous block.**

Imagine** ":adam@cypherspace.org" is all the data in the mempool **we are trying to mine.

Imagine **"6470e06d773e05a7" is the nonce**. Sure the actual bitcoin timechain takes terahashes per second to solve, but the results are easily verifiable. We use a number only once because each number only yields one answer. It would be a waste of energy to use the same number twice. Instead of double hashing the actual mempool, we can use this simpler version of data to see how bitcoin mining works.  Notice how the header of the last block is used in this system. This means that every bitcoin block, except the genesis block, requires information from the previous block.  Becaise of this, we can say these blocks are chained together.  It cannot be undone because eaach new block requires information from the previous block.

----

Let's use duck duck go to find the SHA-1 hex hash of this data by entering the following into the duck duck go browser.

`sha1 0:030626:adam@cypherspace.org:6470e06d773e05a7`

You should get this:
73f88e0645f8ca92ef3a0bc02ef4b7edf85fadbd

Unfortunately, this is like a jumbled up Rubix Cube and will not create a new block, but when we try the next **nonce**, we get this:

`sha1 0:030626:adam@cypherspace.org:6470e06d773e05a8`  This is from the hashcash documentation at https://hashcash.org.

00000000c70db7389f241b8f441fcf068aead3f0

Now we have a required  amount of zeros and we can say the puzzle is complete. It is not that complicated, but requires doing this a gazillion times before we get an answer





### The Halfing

There is a debate. Some people prefer Halvening, others Halfing. I like Halfing because it makes me think of Hal Finney, but that's just this authors personal opinion. My opinion does not matter but the math does.

After 210,000 blocks, the block reward gets cut in half, until the last Satoshi is mined in about the year 2139 or 2140.  Nobody really know for sure, but we can forsee the future of a bitcoin to a certain degree. We are like the Oracle in the Matrix who knew the spoon would drop.   I never took calculus. I never learned what a summation was in college, but the following made perfect sense to me right away. I could see this goofy math thing-a-majig described the halfings.  It made sense because I knew the halving was every four years.  Then I realized this summation really tells the same story Satoshi told, but in the language of mathmatics. The actual story is told in C++, yet another language. Copernicus called "mathematics the language of the universe". In this framing, bitcoin is more than just software. It is a work of art, a monumental mathmatical achievement that can be awed after for hundreds of years to come like the Cistine Chappel..
![hour](https://pbs.twimg.com/media/E-8bBOsVQAMAWfm?format=jpg&name=large) (Anil Patel aka @anilsaidso)


The block reward was 50 for the first epoch. 

In the language of mathmatics, it is divided by two every 210,000 blocks.

We get a new block every ten minutes.

![hour](https://cdn.nostr.build/p/nb5267.png)

144 blocks every day

![day](https://cdn.nostr.build/p/nb5266.png)

The blocks start to get to big to manage when we get into these higher numbers, but you get the idea.

144 x 7 = 1,008 **one week**



144  x 14 = 2016 The difficulty adjustment is every 2016 blocks, but 2016 ten minute blocks are exactly **two weeks**.

144 x 365 = 52,560 **blocks in a year**

4(144 x 365.25) = 210,384 **in 4 years**

That's 4 years and 2.67 days, but we round and say the having happens  every four  years.

We just say we have a halving every 4 years, but the subsidy stops after 32 of them. Then fees incentivize the miners to solve this numeric Rubix Cube 

That's how bitcoin works in a nutshell.

By the year 2032, a solo miner who creates a block will receive a block subsidy of 0.78125.  Unless fees drastically increase, miners will not receive a whole coin for solving this puzzle in just nine years.  You might want to get some before then, but first we need to learn how to create a wallet

[Next Chapter-- Practice Makes Perfect: The Padawan Wallet(#)





