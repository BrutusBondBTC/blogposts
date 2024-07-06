
# The Lightning Network

(1.5 Draft)

["Bitcoin isn't currently practical for very small micropayments. Not for things like pay per search or per page view without an aggregating mechanism, not things needing to pay less than 0.01. The dust spam limit is a first try at intentionally trying to prevent overly small micropayments like that. Bitcoin is practical for smaller transactions than are practical with existing payment methods. Small enough to include what you might call the top of the micropayment range. But it doesn't claim to be practical for arbitrarily small micropayments."]([Flood attack 0.00000001 BC](https://bitcointalk.org/index.php?topic=287.msg7524#msg7524))

The lightning network fixes this, but this is not a magic Internet money bullet. If the goal is to have 8 billion people use the ligntning network on their own computer, with their own [UTXO's]([UTXO Model: Definition, How It Works, and Goals](https://www.investopedia.com/terms/u/utxo.asp)) without any [hard forks]([Hard Fork: What It Is in Blockchain, How It Works, and Why It Happens](https://www.investopedia.com/terms/h/hard-fork.asp))--we might not be able to achieve this. If the goal is to make micro-payments possible, then the lightning helps us achieve this goal. How can we reconcile this with our first principle, the first sentence of the bitcoin white paper? 

**"A purely peer-to-peer version of electronic cash would allow online payments to be sent directly from one party to another without going through a financial institution."** 

I don't have the bitcoin because silver sucks bullet. There is no perfect answer. There are trade-offs. Some are not willing to abdicate any self-sovereignty. I respect that, but I have chosen a different security model. I wish I could attribute this idea to the person who I met at a conference who told this to me because it's a brilliant idea. I just don't know this guys name, but he gave me the best answer to this problem. I will do my best to paraphrase this anon's advice. **If you lose your phone, you're out a thousand bucks, but it's not the end of the world.**" Most of us have a phone. Most of us can replace our phone if we lose it. My phone cost $150, so maybe I should keep no more than $150 on a custodial wallet. If yo have a fancy-ass iPhone 3000, maybe you can risk more. It's a little subjective, but a good rule of thumb is: **Make sure the sats on a custodial wallet are not worth more than your phone**. 

When talking about the bitoin, peer-to-peer electronic cash system, our threat model must be super paranoid. Fort Knox does not have the security to prevent double spending. The bitcoin peer-to-peer electronic cash system is 10,000X better than the Fort Knox security model. We might say the current financial system is just a bailout that began in 1971 when Nixon "temporarily" took the US off the gold standard. The bailout Satoshi wrote about in the genesis block was a bailout of the entire fiat financial system. I can't speak for Satoshi, but it appears he intended to solve the double spending problem in response to the systematic threat posed by a credit based fractional reserve system. **There is a big difference in the security needs of a global payment system vs. $100 of paper fiat in your wallet**. There is also a big difference between $150 and your entire life-savings.

## Running Your Own Lightning Node Is Reckless

It is possible to run your own lightning node, but you can still lose sats. I lost sats running my own node. It's a lot of work, some say running one properly is a full time job. It's not worth spending 40 hours a week on running a ligntning node unless you are making a living doing it. 

Running a Lightning node is feasible, but you need to be careful and don't expect to make tons of money with routing fees. You also need to back it up regularly. This process is beyond the scope of this guide, but there are some wallets like Phoenix, Zuess, and Mutiny that allow you to run a node in the cloud. It involves some trade-offs, but these tend to be easier. Phoenix is great, but requires a VPN to download from normie stores. You can still use it if you know how to install apk files on Android.

### Trusting Financial Institutions Works For Most Transactions

"Commerce on the Internet has come to rely almost exclusively on financial institutions serving as trusted third parties to process electronic payments. **_*While the system works well enough for most transactions, it still suffers from the inherent weaknesses of the trust based model_**.""

Emphasis added my the author. A custodial model works for most transactions. There is some risk of rug-pull with custodial lightning addresses, but these risks can be mitigated by limiting the amount of sats you keep on them. If this is something that you are more concerned with, you can always run your one node. Consider your goals, however. Are you concerned with getting rug-pulled? What are the odds that you will rug-pull yourself. I lost 800k sats running my own node. 

Since custodial solutions work fine most of the time, I am willing to risk a small percentage of my net worth by using them. This is no trustless, but it is trust minimized. From there, we can choose our lightning wallet based on our needs. When I started writing this guide, my bias got the best of me. We must earn KYC free sats under all circumstances. That's the way bitcoin should be, FTW. The more I thought about it, however, the more my position evolved. The main issue with not trusting anyone is you need to trust yourself. If you do not trust yourself with runnign a lightning node, I see nothing wrong with trusting someone else with a couple hundred bucks worth of sats. Could you get rug-pulled? Of course, but you can also rug-pull yourself.

If you're just shitposting on nostr and earn a few thousand sats per month, minibits.cash is a custodial wallet that integrates chaumian e cash and the lightning network. The CEO of Coinkite, NVK, calls chumian eCash an honest shitcoin. This is a good way to look at it. Keeping my life savings on minibits is a dumb-ass idea, but it's not worth spending the time learning how to run your own lightning node to protect 5,000 sats. For one thing, you spend 50x the price of 5,000 sats on the cheapest refurbished Dell computer Amazon has to offer. On top of that, you can just as easily rug-pull yourself in a trustless manner. Don't Trust, Verify is important, but the lightnibg network os reckless and "Don't trust, oh shit!" is a real risk on the lightning network. Ask me how I know.



## Choosing A Lightning Wallet

![lnaddresses](https://i.nostr.build/romm3.png)

I cannot recommend any one wallet. I have my own preferences. The issue is custodial wallets get taken down or bugs are found, or maybe fee increases make awesome wallets less useful. You should do your own research. I recommend starting your quest for a lightning wallet here: https://lightningaddress.com. In this section I will give my best shot at explaining the advantages and disadvantages of each of these wallets.


### Zebedee

### BTCPay

### LNMArkets

### Bipa

### FastBotcpoms

### Spark Wallet

### Coinos

### Ligntning Tip Bot

### Blink

### GetAlby


### Wallet of Satoshi

### Noah

### Bitnob


### Bookmark

### Satoshi Lightning


### Stacker News



### NiceHash





### < The Cost Of Replacing Your phone.

If I had less than a 1,000 worth of sats, I wouldn't mind using any of the options on [https://lightningaddresses.com](https://lightningaddresses.com) Could the custodial solutions rug-pull you? Yes, but like that dude at the conference said, I could drop my phone in the ocean. I won't be happy about it, but it's not the end of the world. You could also run a fat lightning channel for a thousand bucks. If you want to be self-sovereign and have the time, go for it. Use Bitcoin Core or LND and go to town. Get a ligghtning address with BTCpayServer. The one-click option on Lunanode is the easiest way to do so, but it costs about 4.00 per month.

You can also run your own node. The most popular options are Start9 and Umbrel. At the time of this writing, you can pick up an Umbrel for 400 and Start 9 for 600. You can also use a refurbished computer for about a hundred bucks if you know what you're doing. There are also hybrid models that allow you to hold your own keys using a lightning service provider, but the availability will vary based on your local jurisdiction. For example, many of these companies will now operate in the United States due to draconian regulatory enforcement. The Samourai devs were controversial. They made many enemies. To be honest, they could be dicks at times, but in my opinion they did not deserve to be arrested on conspiracy charges. They allegedly conspired to launder money or some shit. I don't know. I'm not a lawyer, but from my perspective they did one thing that the US government considered to be an illegal act: Write code. This is the one thing each of these wallets have in common. They are all code.

![PGP Book](https://i.thriftbooks.com/api/imagehandler/m/CBFB1A1800D84E0DC62EF565B9EC107D21119457.jpeg)

[Phil Zimmerman wrote code for PGP](http://www.philzimmermann.com/EN/essays/WhyIWrotePGP.html). The US Government thought this was dangerous and they put him on trial. This is one of my favorite stories of regulatory over reach and I've written about it before, but Phil Zimmerman is a smart mother fucker. He knew code was speech. HE also knew the bill of rights had another powerful first sentence. "Congress shall make no law respecting an establishment of religion, or prohibiting the free exercise thereof; or abridging the freedom of speech, or of the press; or the right of the people peaceably to assemble, and to petition the Government for a redress of grievances." I hoped this would be enough to protect people who write code in the United States, but It looks as though I may have been wrong. It's too early to tell and like I said, I'm not a lawyer.

I do not know if the powers that be think using bitcoin on the lightning network is legal or illegal. I do know that privacy is necessary for an open society. If we wish to maintain an open society, we must do our best to preserve it. Lightning is a step in the right direction, but it is not full proof. We should use it anyway, especially in a world so preoccupied with  identity politics. Martin Luther King Jr. once wrote, "I would be the first to advocate obeying just laws. One has not only a legal but a moral responsibility to obey just laws," he wrote. "Conversely, one has a moral responsibility to disobey unjust laws. I would agree with St. Augustine that 'an unjust law is no law at all.'" Martin Luther King Jr. is the quintessential example as to why privacy is necessary in the electronic age. You cannot hide your identity in meatspace. You must reveal yourself. People often think people wearing masks are suspicious. They assume they must be doing something wrong, but the reality is--People judge you based on your appearance. If you don't wear the right clothes, drive the right car, have the right gentalia, the right pigmentation--You could be labeled a persona non-grata--banished from a portion of society. 

"But I didn't do anything wrong so I have nothing to hide."  Martin Luther King Jr. was arrested. What was he arrested for? The powers that be thought he did do something wrong, [leading a Good Friday Demonstration](https://www.history.com/news/kings-letter-from-birmingham-jail-50-years-later).  He wrote a powerful essay in jail. The law is concerned with might, not wrong or right.  This happens again and again. Muslims get put on no-fly lists, black people are sent to the back of the bus, Japanese get sent to internment camps. From time to time, people people are massacred because of their religion. People who are not doing anything wrong can suddenly become suspicious for being nothing more than their identity and the state is not your only problem. Some women get stalked with their geo-location. You can justify using a custodial KYC'd service here and there, but privacy is a human right. We should not expose those who wish to protect that right weather we are doing anything wrong or not.
