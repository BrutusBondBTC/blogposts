
# The Lightning Network

(4th Draft)

["Bitcoin isn't currently practical for very small micropayments. Not for things like pay per search or per page view without an aggregating mechanism, not things needing to pay less than 0.01. The dust spam limit is a first try at intentionally trying to prevent overly small micropayments like that. Bitcoin is practical for smaller transactions than are practical with existing payment methods. Small enough to include what you might call the top of the micropayment range. But it doesn't claim to be practical for arbitrarily small micropayments."](https://bitcointalk.org/index.php?topic=287.msg7524#msg7524)


The lightning network fixes this, but this is not a magic Internet money bullet. If the goal is to have 8 billion people use the ligntning network on their own computer, with their own [UTXO's]([UTXO Model: Definition, How It Works, and Goals](https://www.investopedia.com/terms/u/utxo.asp)) without any [hard forks]([Hard Fork: What It Is in Blockchain, How It Works, and Why It Happens](https://www.investopedia.com/terms/h/hard-fork.asp))--we might not be able to achieve this. If the goal is to make micro-payments possible, then the lightning helps us achieve this goal. How can we reconcile this with our first principle, the first sentence of the bitcoin white paper? 

## Semi-Self-Soveriegn Lightning

**"A purely peer-to-peer version of electronic cash would allow online payments to be sent directly from one party to another without going through a financial institution."** 

I don't have the bitcoin(because silver sucks) bullet. There is no perfect answer. There are trade-offs. Some are not willing to abdicate any self-sovereignty. I respect that, but I have chosen a different security model. I wish I could attribute this idea to the person who I met at a conference who told this to me because it's a brilliant idea. I just don't know this guys name, but he gave me the best answer to this problem. I will do my best to paraphrase this anon's advice. **If you lose your phone, you're out a thousand bucks, but it's not the end of the world.**" Most of us have a phone. Most of us can replace our phone if we lose it. My phone cost $150, so maybe I should keep no more than $150 on a custodial wallet. If yo have a fancy-ass iPhone 3000, maybe you can risk more. It's a little subjective, but a good rule of thumb is: **Make sure the sats on a custodial wallet are not worth more than your phone**. 

When talking about the bitoin, peer-to-peer electronic cash system, our threat model must be super paranoid. Fort Knox does not have the security to prevent double spending. The bitcoin peer-to-peer electronic cash system is 10,000X better than the Fort Knox security model. We might say the current financial system is just a bailout that began in 1971 when Nixon "temporarily" took the US off the gold standard. The bailout Satoshi wrote about in the genesis block was a bailout of the entire fiat financial system. I can't speak for Satoshi, but it appears he intended to solve the double spending problem in response to the systematic threat posed by a credit based fractional reserve system. **There is a big difference in the security needs of a global payment system vs. $100 of paper fiat in your wallet**. There is also a big difference between $150 and your entire life-savings.

## Running Your Own Lightning Node Is Reckless

![picture of raspberry pi broken](#)
It is possible to run your own lightning node, but you can still lose sats. I lost sats running my own node. It's a laborious pain in the ass. Some say running one properly is a full time job. It's not worth spending 40 hours a week on running a lignthing node unless you are making a living doing it. 

You can still run a lightning node, but it takes a lot of research. You can also run a BTCpayServer on [lunanode with oneclick](https://docs.btcpayserver.org/Deployment/LunaNode/). This costs about $4.00 per moth(you can pay with sats on the lightning network). I ran one of these for about two years and it worked great. You can use extenstions to do things like host your own lightning address. They have woocommerce plugins and tools that allow you to sell pdf's online, but don't expect to make tons of money with routing fees. It will work well if you have stuff to sale. 

[LNBits](https://my.lnbits.com/login) also has a cloud option to run a node that is even easier to set up.[Voltage](https://www.voltage.cloud/pricing) is another great option. You can choose these based on your own needs. Not everyone needs a $200 per month Voltage plan, but some people do. The goal of this section is to expose you to different options available to orange coin conisoours. 

Some wallets like [Phoenix](https://phoenix.acinq.co/), [Zuess](https://zeusln.com/), and [Mutiny](https://www.mutinywallet.com/), allow you to run a node in the cloud. GetAlby is working on [AlbyHub](https://github.com/getAlby/hub), but it's in Beta.  Thesse options involve some trade-offs, but they tend to be easier to run than your own node. Phoenix still works in the US, but requires a VPN to download from normie stores. You can still use it if you know how to [install the apk file on Android](https://github.com/ACINQ/phoenix/releases/tag/android-v2.3.1).

If you do choose to run your own lightning node, get a real computer like, [start9](https://start9.com/) or [umbrel](https://umbrel.com/). You can also run these on your own hardware. Many sat stackers flash this software onto refurbished computers like Dell OptiPlex for a couple hundred bucks. This worked for me for a while, until the hardware failed. I think it's better to buy machines on the market made to run nodes like Start9 and Umbrel. I have both. Whatever you do, do not use a raspberry pi unless you want to incenerate your sats. Ask me how I know.

I also want to yell at the top of my lungs that THESE NODES DO MORE THAN JUST BITCOIN TRICKS FOR BITCOIN KIDS SILLY RABBIT! I love [Mealie](https://github.com/mealie-recipes/mealie) on my Umbrel and [SearX](https://github.com/searx/searx) on Start9. These have nothing to do with bitcoin, but are awesome tools nonetheless.

### Trusting Financial Institutions Works For Most Transactions

"Commerce on the Internet has come to rely almost exclusively on financial institutions serving as trusted third parties to process electronic payments. **_*While the system works well enough for most transactions, it still suffers from the inherent weaknesses of the trust based model_**.""

Emphasis added my the author. A custodial model works for most transactions. There is some risk of rug-pull with custodial lightning addresses, but these risks can be mitigated by limiting the amount of sats you keep on them. If this is something that you are more concerned with, you can always run your one node. Consider your goals, however. Are you concerned with getting rug-pulled? What are the odds that you will rug-pull yourself. I lost 800k sats running my own node. 

Since custodial solutions work fine most of the time, I am willing to risk a small percentage of my net worth by using them. This is no trustless, but it is trust minimized. From there, we can choose our lightning wallet based on our needs. When I started writing this guide, my bias got the best of me. We must earn KYC free sats under all circumstances. That's the way bitcoin should be, FTW. The more I thought about it, however, the more my position evolved. The main issue with not trusting anyone is you need to trust yourself. If you do not trust yourself with runnign a lightning node, I see nothing wrong with trusting someone else with a couple hundred bucks worth of sats. Could you get rug-pulled? Of course, **but you can also rug-pull yourself**.

If you're just shitposting on nostr and earn a few thousand sats per month, [minibits.cash](https://www.minibits.cash/) is a custodial wallet that integrates [chaumian e cash](https://chaum.com/ecash/) with the lightning network. The CEO of [Coinkite](https://coinkite.com/), NVK, calls chaumian eCash an honest shitcoin. This is a good way to look at it. Keeping my life savings on minibits is a dumb-ass idea, but it's not worth spending the time learning how to run your own lightning node to protect 5,000 sats. For one thing, you spend 50x the price of 5,000 sats on the cheapest refurbished Dell computer Amazon has to offer. On top of that, you can just as easily rug-pull yourself in a trustless manner. Don't Trust, Verify is important, but the lightnibg network os reckless and "Don't trust, oh shit!" is a real risk on the lightning network. Ask me how I know.



## Choosing A Lightning Wallet

![lnaddresses](https://i.nostr.build/romm3.png)

I cannot recommend any one wallet. I have my own preferences. The issue is custodial wallets get taken down or bugs are found, or maybe fee increases make awesome wallets less useful. You should do your own research. I recommend starting your quest for a lightning wallet here: https://lightningaddress.com. In this section I will give my best shot at explaining the advantages and disadvantages of some of these wallets. I have not tried them all. Some of them are geared for other countries, but here are some of the wallets on lightning address.com that I have used.


### BTCPay
Great Fpor Stores Woo Commerce support Create Youw Own Store One Click solution




### Spark Wallet
Ran it on linux



### Ligntning Tip Bot
I loved this wallet. I had it on telegram for years and was able to use the API with [LNBits](https://lnbits.com/)

### Blink
Blink is an interesting wallet designed for circular economies. One thing that is interesting about this wallet is the [stablesats](#) feature. Stablesats are a bitcoin dollar derivative. This can be helpful for those who don't like to stomach the bitcoin/USD price swings, but still don't want to use banks.

### GetAlby
Get Alby has a great custodial wallet that allows you to login to nostr with the click of a button. You also get a neat lightning address and no KYC is required. Unfortunately, you need an invite code. On the birght side, they are working on a self custodial solution that is in bet testing. 


### Wallet of Satoshi
Wallet of Satoshi is the easiest way to set up a bitcon wallet. The propblem is they have left the US market. You can no longer download the wallet on Google Play or the App Store with a US IP address.


### Stacker News
Stacker News is a website where people post articles and send sats to authors of those articles. I should use it more to be quite honest. They give you a custodial lighting address easily though.



### Coinos
Coinos is great for onbaording merchants. It is custodial but it is very easy to sweep the funds into your own wallet and it doesn't reqyuire any more hardware. It is better if you print receiepts and treat it like cash for accounting purposes. You can also download the transactions from the app. This way, you have a record of how much you got in income to tell the IRS, but without the danger of giving up KYC information. If you never spend these sats, you never need to pay capital gains tax anyway, right? Again, I'm not an accountant or a lawyer, but this is my layman point of view.


 **Coinos Video**
 https://flare.pub/w/naddr1qqr47mttdap5jkgpzpmhxue69uhkummnw3ezuamfdejsygr4hu34xxhflxxx9x2m5pcereygat28t96nw8tr6l0ag677r0agj5psgqqqskas3l7q2j

### What About Regulatory Concerns?

I do not know if the powers that be think using bitcoin on the lightning network is legal or illegal. I do know that [privacy is necessary for an open society](#). If we wish to maintain an [open society](https://en.wikipedia.org/wiki/The_Open_Society_and_Its_Enemies), we must preserve privacy. Lightning is a step in the right direction, but it is not 200 proof private. It will give you privacy from the banks and credit cards though. Do you want corporations to know everything you buy? But I'm not doing anything wrong so I don't have anything to hide. Even if you don't shop dildos.com, bullets.com, or abortions.com, this information may still be used against you. Imagine how easy it would be to find every person by searching for the people who buy the most Kosher or Halal food. Nobody cares about privacy until it is too late.

Even if we assume humans will never go full on tribal again, everytime you swipe your card, a bank gets more information. This information is used against you by advertisers trying to get you to spend more money than you otherwise would have. If ads didn't work, why would they be so valuable? Everytime you buy trinket on Amazon, a bank sells an ad for that trinket like an angel gets it's wings everytime a bell rings. The lightning network may not be totally private, but it sure is better than credit cards.  Credit carreds are designed to get you to spend more money. If you spend more money, you save less sats. When you spend sats, you sure think twice about it.


Bitcoin is freedom money. In "A Letter From A Birmingham Jail," Martin Luther King Jr. wrote:
 
`"I would be the first to advocate obeying just laws. One has not only a legal but a moral responsibility to obey just laws. Conversely, one has a moral responsibility to disobey unjust laws. I would agree with St. Augustine that 'an unjust law is no law at all."`

![MLKJr](http://cdn.history.com/sites/2/2014/01/mlk-in-birmingham-jail.jpg)
Martin Luther King Jr. is the quintessential example as to why privacy is necessary in the electronic age. You cannot hide your identity in meatspace. [J. Edgar Hoover prohibited Martin Luther King Jr.'s privacy](https://time.com/5930571/martin-luther-king-jr-fbi/). **Alphabet government organizations like to watch protesters**. [In some countries, they like to shoot protestors](#).CBDC's might be a political talking point, but credit cards give governments all the data they need to track protesters. 

People often think [people wearing masks are suspicious(#).  They assume they must be doing something wrong, but the reality is--People judge you based on your appearance. If you don't wear the right clothes, drive the right car, the right junk in your underware, the right pigmentation, political ideology, or nationality--You could be labeled a persona non-grata--banished from society.

Martin Luther King Jr. was arrested because the powers that be thought he did do something wrong, leading a Good Friday Demonstration, not because he had something to hide. He did not hide his identity. How could he given the issues he protested? He wanted the right to sit in a restaurant and pay for lunch in places that did not want him to sit in their restaurant. Protesting was his only option because he could not selectively reveal himself to the world in meatspace. We should take measures to selectively reveal our transactions in meatspace as long as we can.

Many people think payments are unimportant, but I disagree. Payment systems are designed to favor some people more than others. You never know what people will be targeted in the future. Since we all may ve targets given a change in the political winds, we all need. While not perfect, the lightning network can help us achieve more privacy.



Note, the links in this chapter are not affiliate links.



₿logging ₿itcoin 
[848,231](https://timechaincalendar.com/en/block/848231 )
[debtclock](https://www.usdebtclock.org/)

[Support My Work Using The Value 4 Value Model](https://pay/coinos.io/BloggingBitcoin)

https://nostree.me
