---
title: 'Replication Markets: Can You Predict Which Social Science Papers Will Replicate?'
subtitle: Discussing the mechanics of the Replication Markets platform and my priors on the replicability of different social science fields.
layout: default
date: 2019-08-21
keywords: replication, sociology, social science
published: true
permalink: /replication-markets/
---
### What are Replication Markets?

Replication Markets are a type of [prediction market](http://mason.gmu.edu/~rhanson/ideafutures.html), mechanisms that enable individuals to bet on the outcome of events. Just as financial markets efficiently determine the perceived value of a security by aggregating the beliefs of buyers and sellers (e.g., I think this stock will rise in price, so I will buy more), [prediction markets](https://www.investopedia.com/terms/p/prediction-market.asp) determine the perceived likelihood of an event by aggregating the beliefs of many individuals. Both financial and prediction markets draw on the [wisdom](https://en.wikipedia.org/wiki/Wisdom_of_the_crowd) (or sometimes lunacy) of crowds and the power of financial incentives. 

There are many demonstrated applications of prediction markets, like predicting political events ([PredictIt](https://www.predictit.org) enables betting on who will be the Democratic nominee in the 2020 US election).

Replication Markets are another such application, and they will be the focus of this article. Replication Markets aggregate predictions about which scientific claims will successfully replicate (i.e., demonstrate a statistically significant effect when the experiment is repeated). Replication markets for social science research have a track record of success, reaching upwards of 75% accuracy and sometimes even surpassing the predictive performance of experts (see [this paper](https://www.pnas.org/content/112/50/15343) and [this other paper](https://www.sciencedirect.com/science/article/pii/S0167487018303283), or the papers [here](https://www.citationfuture.com/), for example).

A DARPA project called [SCORE](https://www.darpa.mil/program/systematizing-confidence-in-open-research-and-evidence) (Systematizing Confidence in Open Research and Evidence) intends to use prediction markets to forecast if social science research claims will replicate. 3000 such claims will be in the market. [The claims](https://predict.replicationmarkets.com/main/#!/about) come &#8220;from social and behavioral science articles published in the last 10 years&#8221; (psychology, economics, education research, management and marketing, political science, and sociology and criminology).

There is a public website, [Replication Markets](http://replicationmarkets.com) (RM), that is crowdsourcing these predictions for SCORE. Nearly anyone can participate and there are financial rewards for top forecasters. (When I refer to RM, I&#8217;m referring to the contest the site is currently hosting.)

In this essay, I&#8217;ll explain how RM works, explain the market mechanisms and game theory of it, and walk through my thought process and strategy.

## How Replication Markets Works

### What Counts as Replication?

I myself am participating in the RM game. Because I&#8217;m competitive, I want to keep score. Though the total financial rewards sum to over $100k, realistically the chance of anyone person winning a lot of money is pretty low, so I&#8217;m doing this mostly for fun. Nonetheless, I&#8217;ll use money as my metric for success.

To win money, we need to predict replication. To do that, we need to know what the criterion for replication is. 

[According to Replication Markets](https://www.replicationmarkets.com/index.php/2019/06/24/what-is-high-powered-replication/), for each of the claims (i.e., the social science assertions) selected to be tested, SCORE&#8217;s data team &#8220;will run a single high-quality replication of each selected claim.&#8221; A replication will be [deemed successful](https://www.replicationmarkets.com/index.php/frequently-asked-questions/) if they get a statistically significant result in the same direction as the original claim. Markets for claims are binary: ultimately, each claim will either replicate or not.

### Format of the Game

Replication Markets is composed of 10, 4-week rounds, starting in September 2019 (plus a special Round 0 for meta-claims in August 2019, which I&#8217;ll address later). [Each round has two components](https://www.replicationmarkets.com/index.php/frequently-asked-questions/payouts/): markets and surveys, both of which are ways to aggregate many opinions and achieve the [wisdom of crowds.](https://www.google.com/search?q=wisdom+of+crowds&rlz=1C1CHBF_enUS851US851&oq=wsidom+of+c&aqs=chrome.1.69i57j0l5.3192j1j0&sourceid=chrome&ie=UTF-8)

#### **Surveys** 

Surveys are private evaluations (i.e., opinion polls) of the probability that a given claim is true. These evaluations are made a week prior to the market&#8217;s opening. Surveys come in batches of 10 claims (all from the same journal, I believe), and there are around 15 per round. Surveys pay out at the end of the following round, with top 4 participants receiving $80, $40, $20, and $20. 

RM isn&#8217;t specifying how exactly the surveys will be scored. Because they resolve a month after closing, before the actual replication attempts, they must involve predicting what probabilities the prediction markets will give each claim. I emailed RM to find out about the scoring and was told this:

<blockquote class="wp-block-quote">
  <p>
    There is actually an extensive academic literature studying more sophisticated and in many ways superior methods of aggregating crowd forecasts. We are experimenting with such cutting edge methods. In other words, <strong>in the survey you are scored against our best judgment of the right forecast, having processed all the forecasts of other participants using our best aggregation techniques. </strong>
  </p>
  
  <cite>Personal Communication</cite>
</blockquote>

#### **Markets**

Markets are the prediction market aspect of RM. Each participant is given a set number of points, which she can use to buy Yes or No shares for a claim. Markets &#8220;pay out proportionally to winning shares&#8221; and will resolve by mid-2020, once the replications have been attempted.

According to the [rules](https://www.replicationmarkets.com/index.php/frequently-asked-questions/rules/), only 100 of the 3000 (i.e., 3.33%) claims will be selected _and_ pay out (these claims will be directly replicated; the data-replicated claims do not pay out). Each of these has a total payout of $900, paid proportional to the number of winning shares in a resolved claim (e.g., I have 10 Yes shares for Claim X; the total number of Yes shares held by RM participants in 1,000; so, I am paid 10/1,000 out of $900, which equals $9). 

For the meta round, Round 0, &#8220;Meta-claims resolve as the proportion of successful direct replications, so a meta-claim resolving as 60% would pay 0.6 points per ‘Yes’ share and 0.4 points per ‘No’ share.&#8221; The total payout for this round is $360 for each of the 12 meta-claims. 

## Pricing and Game Theory for Markets

### How Are Shares Priced?

Unlike traditional financial markets that use a [Double Auction process](https://en.wikipedia.org/wiki/Double_auction), if you want to buy/sell a share of a claim in RM, you don&#8217;t need someone on the other end of the transaction willing to sell/buy at that price. Rather, in RM you buy directly from the market manager using a pricing system developed by Robin Hanson, the [Logarithmic Market Scoring Rules](http://mason.gmu.edu/~rhanson/mktscore.pdf) (LMSR)

LMSR made no sense to me when I first learned about it. And frankly, it doesn&#8217;t totally make sense to me now. Robin Hanson wrote a couple of papers on it, so look into them if you want to deeply understand it. 

Since I&#8217;m not a finance guy, I don&#8217;t care enough to understand it deeply. Most of my knowledge I&#8217;ve gleaned from the equations [here.](http://beza1e1.tuxen.de/articles/LMSR.html) These are, in my opinion, the important points:

  1. The price of buying shares at time _t_ depends on the cost of the share at time _t-1_; the cost of the share changes after every trade.
  2. The cost of shares depends on how many &#8216;Yes&#8217; and &#8216;No&#8217; shares have been bought. The market&#8217;s prediction of a claim (i.e., its price), p, depends on the number of &#8216;Yes&#8217; and &#8216;No&#8217; shares bought. p is equal to the market&#8217;s probability rating of the claim.
  3. &#8216;Yes&#8217; shares get cheaper as p decreases whereas &#8216;No&#8217; shares get more expensive, and vice versa.
  4. The relationship between p and the cost of a &#8216;Yes&#8217; or &#8216;No&#8217; share is essentially linear or slightly concave upward or downward, depending on if you&#8217;re buying minority or majority shares. 

### How to Win the Markets

The game-theoretic aspect of RM is that the price of a &#8216;Yes&#8217; or &#8216;No&#8217; share depends on the market&#8217;s evaluation of that claim, which can change volatilely. This presents the opportunity for arbitrage, especially in Round 0. 

As one participant in RM explains: 

<blockquote class="wp-block-quote">
  <p>
    If you buy &#8220;yes&#8221; when the market is at 30% then sell when it is at 50% you end up with more points. Of course, points are only useful for buying shares in other markets, so you should only &#8220;cash out profits&#8221; if you think there&#8217;s another market that is further off than the one you&#8217;re cashing out of.
  </p>
  
  <cite>&#8211; <a href="https://predict.replicationmarkets.com/main/#!/users/188">Davidoj</a>, RM participant</cite>
</blockquote>

Here&#8217;s an example of arbitrage, converting 23 &#8216;No&#8217; shares to 36 &#8216;Yes&#8217; shares (with the help of 2 other points, which buy about 6 of the 36 shares):<figure class="wp-block-image">

<img loading="lazy" width="620" height="246" src="https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/arbitrage_1.png?resize=620%2C246&#038;ssl=1" alt="" class="wp-image-1403" srcset="https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/arbitrage_1.png?w=891&ssl=1 891w, https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/arbitrage_1.png?resize=300%2C119&ssl=1 300w, https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/arbitrage_1.png?resize=768%2C304&ssl=1 768w" sizes="(max-width: 620px) 100vw, 620px" data-recalc-dims="1" /> </figure> <figure class="wp-block-image"><img loading="lazy" width="620" height="242" src="https://i2.wp.com/adamlgreen.com/wp-content/uploads/2019/08/arbitrage_2.png?resize=620%2C242&#038;ssl=1" alt="" class="wp-image-1404" srcset="https://i2.wp.com/adamlgreen.com/wp-content/uploads/2019/08/arbitrage_2.png?w=893&ssl=1 893w, https://i2.wp.com/adamlgreen.com/wp-content/uploads/2019/08/arbitrage_2.png?resize=300%2C117&ssl=1 300w, https://i2.wp.com/adamlgreen.com/wp-content/uploads/2019/08/arbitrage_2.png?resize=768%2C299&ssl=1 768w" sizes="(max-width: 620px) 100vw, 620px" data-recalc-dims="1" /></figure> 

### Round 0

For Round 0, you must predict the percentage of claims that will replicate per field and per time period. There are 12 such &#8220;meta-claims&#8221;. Pay outs are based on the number of &#8216;Yes&#8217; or &#8216;No&#8217; shares you have for each of these 12 meta-claims. 

To determine the proper strategy and expected payout, we must consider the following parameters:

  * N = the number of total RM participants (as of August 2019, the site claims 500 people have signed up; however, it seems only a 100 or so people are actively participating in the markets; this bodes well, as the fewer participants, the greater your chances of winning.)
  * The number of points (participants start with 100)
  * The proportion of N that spend all their points (I&#8217;ll assume this is 100% to be conservative)

A toy example: assume that every meta-claim had a replication rate of 50%. This means that &#8216;Yes&#8217; and &#8216;No&#8217; shares are paid the same amount. The total prize money is $4320 for these 12 claims. The total pool of points is 50,000, assuming N = 500. So, if everyone bought their shares at the exact same price, each point is worth about $0.086. Given that everyone started with 100 points, each person earns around $8.60. If we change our assumptions and let N = 100, each person earns around $43. 

A more realistic example: assume that each meta-claim has a 0.5 chance of being either 40% or 60%. Suppose that you end up being on the correct side of all 12 of these markets (i.e., if the replication rate is 60%, you bought all &#8216;Yes&#8217; shares). Also, suppose that the prediction market&#8217;s final estimates for all these claims are 50%. Then, if you start with 100 points and evenly distribute them across claims, your earnings will be around 10% more, as you receive 0.6 points for every &#8220;correct&#8221; share.

**Strategy** 

There are possible arbitrage and subterfuge opportunities, but frankly, I don&#8217;t think they&#8217;re worth going into given how small the rewards are.

### Rounds 1-10

The more interesting game theory is in Rounds 1-10. Should we uniformly distribute our points, or should we focus on areas in which we have more expertise, and therefore are more likely to correctly predict?

Replication Markets [suggests](https://www.replicationmarkets.com/index.php/2019/06/24/what-to-do/) the following: 

&#8220;The market is probably most accurate when forecasters specialize, because one kind of forecaster won’t have enough points.&#8221;

Per round, each forecaster has 300 points to spend on 300 claims, 10 of which will be directly replicated and paid out. Assuming (obviously a simplification) that replication rate is constant across all six fields, that means around 1.67 claims per field will be directly replicated each round. The total prizes per round are $9000, meaning that the expected prize money for each claim is $30. 

**Strategy**

Conditional on a claim being selected for replication and you predicting the correct outcome, the fewer the number of participants in that market, the higher your payout. **So, your best option is to participate in the markets that have the fewest participants (such a rule wouldn&#8217;t function in a traditional double auction financial market, but in RM it works because you buy shares from the market manager).** Other than that, there isn&#8217;t much strategy to give at the individual level (prediction markets are about aggregate behavior, after all). 

(Note, however, that this isn&#8217;t an evolutionarily stable strategy; if everyone were to realize markets with fewer participants increased their chances of winning, the equilibrium condition would be an even distribution of participants among all markets.)

## How to Win the Surveys

Surveys are by far the more financially rewarding opportunity in RM. They have a [tournament payout structure](https://www.truepoker.eu/poker-tournaments/payout-structure/), with only the top 4 forecasters winning. And they don&#8217;t involve the confusing LMSR the markets use. To win the surveys, you need to be good at predicting which claims will replicate, which I&#8217;ll focus on below. But first, let&#8217;s focus on the second-order function of which claims the rest of the survey-takers _believe_ will replicate, as this is key to the survey scoring function.

#### Survey Scoring Rules

RM will use some secret crowd aggregation technique for scoring surveys. All they&#8217;re willing to reveal is that &#8220;in the survey you are scored against our best judgment of the right forecast, having processed all the forecasts of other participants using our best aggregation techniques.&#8221; 

So, I imagine that if you want to win the surveys, your private survey opinions must align with the aggregate survey predictions. Setting aside any sort of nested/higher-order logic on the part of other survey participants (e.g., if everyone adopted a strategy of biasing their survey results towards what they thought everyone else would say, that strategy wouldn&#8217;t work), how could we optimally align our survey answers?

This depends on the survey scoring method. A good candidate is to be found in the recent arXiv paper by Yang Liu and Yiling Chen (two members of the [RM scoring team](https://www.replicationmarkets.com/index.php/our-team/)), &#8220;[Surrogate Scoring Rules and a Uniform Dominant Truth Serum](https://arxiv.org/pdf/1802.09158.pdf)&#8220;. Considering that RM will be experimenting with novel methods of survey aggregation, I think this fits the bill. The question is: will understanding the scoring system allow us to game it?

##### Surrogate Scoring Rules

The scoring problem Liu and Chen address is the following: 

If you want to aggregate the opinions of many individuals, you must **elicit** these opinions and **verify** them. In markets, for example, opinions are elicited by the prospect of financial reward and verified against the ground truth (whether or not a security&#8217;s price rises or falls). An agent&#8217;s **score** is how well his prediction matches the ground truth. These are called &#8220;**Strictly Proper Scoring Rules**&#8221; (SPSR). Under an SPSR, an agent is expected to maximize his expected score and truthfully reveal his beliefs.

Conversely, situations in which verification is noisy or unavailable (e.g., Replication Markets, as we won&#8217;t know if the claims replicate until mid-2020) are called &#8220;**Information Elicitation Without Verification**&#8221; (IEWV), and they face a host of issues. A family of _peer prediction_ mechanisms has been developed to deal with these issues. One such issue is that because an agent&#8217;s score depends on the beliefs of others, an agent can benefit from misrepresenting his beliefs. 

The question for the principal (i.e., RM) is: 

<blockquote class="wp-block-quote">
  <p>
    Can we design scoring mechanisms to quantify the quality of information as SPSR do and achieve truthful elicitation in a certain form of dominant strategy for IEWV?
  </p>
  
  <cite><a href="https://arxiv.org/pdf/1802.09158.pdf">Liu and Chen</a></cite>
</blockquote>

One of their proposed solutions is &#8220;surrogate scoring rules&#8221; (SSR). 

While Hansons&#8217; LMSR makes a bit of sense to me, SSR makes absolutely no sense at this time. One might be able to derive some value from really digging into this topic, but I think honestly representing your opinions offers a pretty optimal strategy for the surveys. Just give your honest belief about if a claim will replicate.

To that end, how should we predict if a claim will replicate?

## The Replication Crisis and Our Base Rate of Replication

If we want to predict which studies will replicate, we first need a base rate of replication among all social science. To determine this, we must ask ourselves: is social science actually science? Some are skeptical: 

<blockquote class="twitter-tweet">
  <p lang="en" dir="ltr">
    The core of the problem:<br />1) social scientists want to &#8220;learn statistics&#8221; w/o understanding probability.<br />2) social science is NOT science. <a href="https://t.co/k064zytNBB">https://t.co/k064zytNBB</a>
  </p>— Nassim Nicholas Taleb (@nntaleb) 
  
  <a href="https://twitter.com/nntaleb/status/881500380479279104?ref_src=twsrc%5Etfw">July 2, 2017</a>
</blockquote>

Though I&#8217;m not Taleb-level skeptical, I believe there&#8217;s an inkling of truth in his claim that many academics are &#8220;[intellectuals-yet-idiots](https://medium.com/incerto/the-intellectual-yet-idiot-13211e2d0577)&#8221; who lack &#8220;[skin in the game](https://medium.com/incerto/what-do-i-mean-by-skin-in-the-game-my-own-version-cc858dc73260)&#8221; (though Taleb himself is an IYI on topics like behavioral genetics and psychometrics). Evidence includes the following list of&nbsp;social science and medicine research areas and claims that were once taken seriously but have failed to replicate:

  * The [candidate gene era](https://slatestarcodex.com/2019/05/07/5-httlpr-a-pointed-review/) in psychology/genetics 
  * The [early, small N](https://www.biorxiv.org/content/10.1101/681700v2) work done in [cognitive neuroscience](http://tomstafford.staff.shef.ac.uk/reliable/IsCognitiveNeurosciencereliable.html)
  * Much of nutritional research and epidemiology, the methods of which are extremely suspect (e.g., doing a proper RCT is nearly impossible, retrospective food tracking is unreliable, genetic confounding, etc.)
  * The social psychology literature on priming, which is p-hacked and riddled with publication bias
  * The educational research on [growth mindset](https://twitter.com/Russwarne/status/1152857329181704192)
  * The effect of early-childhood educational interventions on academic outcomes (which has [clear publication bias](https://rpubs.com/EmilOWK/pub_bias_early_intervention))
  * &nbsp;[Candidate drug targets](https://www.nature.com/articles/nrd3439-c1) in [oncology](https://www.ncbi.nlm.nih.gov/pubmed/22460880?dopt=Abstract&holding=npg); one replication effort had a 6/53 **(~11%) replication rate**

This list doesn&#8217;t inspire confidence. Ex post facto, it&#8217;s easy to call these fields BS and impugn the motivations of the researchers doing the spurious research within them. (And sure, some of these fields still suffer from collective delusions inspired by political ideology.) But in most cases, we should remember [Hanlon&#8217;s razor](https://en.wikipedia.org/wiki/Hanlon%27s_razor): 

<blockquote class="wp-block-quote">
  <p>
    &#8220;Never attribute to malice that which is adequately explained by stupidity.&#8221;
  </p>
</blockquote>

And, frankly, I don&#8217;t think we can chalk it all up to stupidity. All the list of failed replications demonstrates is that the social science publishing game has a lot of **perverse incentives**. For example, there&#8217;s a massive **[principal-agent problem](https://en.wikipedia.org/wiki/Principal%E2%80%93agent_problem)**: the incentives of the agent—the researcher who wants to get tenure and publish novel findings—do not necessarily align with those of the principal—humanity as a whole, which (in theory) has much to gain from the public good, science, that the agent is contributing to. 

Consequently, [academic malpractice](https://en.wikipedia.org/wiki/Malpractice)—whether due to malfeasance, obstinance, or negligence—is much more common then we think. 

**These failures of social science and ethics notwithstanding, and despite claims that** [most published research findings might be false](http://robotics.cs.tamu.edu/RSS2015NegativeResults/pmed.0020124.pdf)**, large parts of social science _are_ replicable.** 

Case in point, a [2018 replication project](https://www.nature.com/articles/s41562-018-0399-z) for 21 social science papers published in _Science_ and _Nature_ (two of the top general science journals) between 2010 and 2015 had a replication rate of 62%.

## Does Replication Rate Vary Significantly By Field?

A single general social science replication project is useful, but certainly not dispositive. A much better approach is to look at replication on a field-by-field basis, set these as our priors, and forecast replication of specific claims using these priors. 

It&#8217;s clear that certain fields have better [epistemic hygiene](https://wiki.lesswrong.com/wiki/Epistemic_hygiene) than others. One index of poor epistemic hygiene is the percentage of publications in a field that feature results confirming the tested hypothesis, i.e., positive results. Psychology [is the worst culprit](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2850928/) in this regard. <figure class="wp-block-image">

<img loading="lazy" width="447" height="515" src="https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/positive_publication_bias-1.jpg?resize=447%2C515&#038;ssl=1" alt="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2850928/" class="wp-image-1370" srcset="https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/positive_publication_bias-1.jpg?w=447&ssl=1 447w, https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/positive_publication_bias-1.jpg?resize=260%2C300&ssl=1 260w" sizes="(max-width: 447px) 100vw, 447px" data-recalc-dims="1" /> </figure> 

Typically, among the social sciences, it&#8217;s the &#8220;harder&#8221; social sciences (e.g., much of economics, parts of psychology like behavioral genetics and quantitative psychology) that have better epistemic hygiene. Therefore, we&#8217;d expect replication to be higher in these fields.

However, I&#8217;d like to put concrete estimates on the replication rates and rank-order the fields. To do this, I&#8217;ll consider the following for each field:

  * Replication rates from existing replication efforts
  * Any indices of publication bias
  * How strong the culture of replication is
  * How much dissent and debate is tolerated
  * How mathematical each field is (which isn&#8217;t to say mathematical models are better—excessive math is often a form of formalist obscurantism, and dressing up a poor model with complex math doesn&#8217;t make the underlying model any better)
  * A gut feeling for how ideologically motivated members of each field are (I&#8217;ll glance at the journals in each field and see if my BS detector goes off)
  * Any major replication scandals that have occurred in the field

I&#8217;ll weigh the existing replication attempts most heavily, so here they are:

**Economics:** 

A [replication project](https://science.sciencemag.org/content/351/6280/1433) done by the Experimental Economics Replication Project (EERP) had a [**61% replication rate**](https://experimentaleconreplications.com/). 

##### **Psychology:**

2015: The &#8220;[Reproducibility Project: Psychology](https://science.sciencemag.org/content/349/6251/aac4716)&#8221; attempted to replicate 100 papers published in three top psychology journals in 2008. [**39%**](https://www.nature.com/news/over-half-of-psychology-studies-fail-reproducibility-test-1.18248) **of papers successfully replicated).**

[The Many Labs Projects 1, 2, and 3](https://www.sciencedirect.com/science/article/pii/S0167487018303283#b0280) performed [ideal,](https://www.replicationmarkets.com/index.php/2019/06/24/what-is-high-powered-replication/) high-[quality replications](https://www.replicationmarkets.com/index.php/2019/06/24/what-is-high-powered-replication/) (i.e., multiple labs attempted to replicate findings). The replication rates were 77%, 50%, and 30%, respectively. The total replication rate (i.e., the weighted sum) was **53%**. 

#### Other Metrics of Epistemic Hygiene

**Economics:** 

Economists have been discussing replication for [quite a while.](https://www.nber.org/papers/w13026)

That said, economics is having [its own replication crisis](https://www.bloomberg.com/opinion/articles/2018-09-17/economics-gets-it-wrong-because-research-is-hard-to-replicate). Consider publication bias among three of the top economics journals, for example:

<blockquote class="wp-block-quote">
  <p>
    We observe a two-humped camel shape with missing p-values between 0.25 and 0.10 that can be retrieved just after the 0.05 threshold and represent 10-20 percent of marginally rejected tests. Our interpretation is that researchers inflate the value of just-rejected tests by choosing &#8220;significant&#8221; specifications.
  </p>
  
  <cite><a href="http://ftp.iza.org/dp7268.pdf">Brodeur et al., 2016</a></cite>
</blockquote><figure class="wp-block-image">

<img loading="lazy" width="620" height="694" src="https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/p_hacking_econ.png?resize=620%2C694&#038;ssl=1" alt="" class="wp-image-1372" srcset="https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/p_hacking_econ.png?w=744&ssl=1 744w, https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/p_hacking_econ.png?resize=268%2C300&ssl=1 268w" sizes="(max-width: 620px) 100vw, 620px" data-recalc-dims="1" /> </figure> 

If there weren&#8217;t publication bias, we&#8217;d expect the distribution of z-statistics to smoothly decrease, approximating the tail of a normal distribution.<figure class="wp-block-image is-resized">

<img loading="lazy" src="https://i1.wp.com/adamlgreen.com/wp-content/uploads/2019/08/z-scores.png?resize=434%2C397&#038;ssl=1" alt="" class="wp-image-1395" width="434" height="397" srcset="https://i1.wp.com/adamlgreen.com/wp-content/uploads/2019/08/z-scores.png?w=578&ssl=1 578w, https://i1.wp.com/adamlgreen.com/wp-content/uploads/2019/08/z-scores.png?resize=300%2C275&ssl=1 300w" sizes="(max-width: 434px) 100vw, 434px" data-recalc-dims="1" /> </figure> 

Additionally, certain &#8220;causal&#8221; inference methods in economics, like [difference in differences](https://en.wikipedia.org/wiki/Difference_in_differences)—exploiting natural experiments in longitudinal data, e.g., the effects of a new state policy on some outcome—seem to be particularly [prone to publication bias and p-hacking](http://ftp.iza.org/dp11796.pdf). Whereas, randomized controlled trials (the gold standard of causal inference) and regression discontinuity (using putatively random, exogenous treatments to mimic an RCT) don&#8217;t demonstrate the same degree of publication bias.<figure class="wp-block-image">

<img loading="lazy" width="620" height="515" src="https://i1.wp.com/adamlgreen.com/wp-content/uploads/2019/08/z_density_econ_methods.png?resize=620%2C515&#038;ssl=1" alt="" class="wp-image-1371" srcset="https://i1.wp.com/adamlgreen.com/wp-content/uploads/2019/08/z_density_econ_methods.png?w=871&ssl=1 871w, https://i1.wp.com/adamlgreen.com/wp-content/uploads/2019/08/z_density_econ_methods.png?resize=300%2C249&ssl=1 300w, https://i1.wp.com/adamlgreen.com/wp-content/uploads/2019/08/z_density_econ_methods.png?resize=768%2C638&ssl=1 768w" sizes="(max-width: 620px) 100vw, 620px" data-recalc-dims="1" /> </figure> 

<p class="has-text-align-left">
  In the above graph, the stars correspond to the <a href="https://en.wikipedia.org/wiki/Z-test">z-scores</a> that give p-values of 0.1, 0.05, and 0.01.
</p>

Effect sizes in economics are [wildly overestimated](https://onlinelibrary.wiley.com/doi/abs/10.1111/ecoj.12461), too.

**Psychology:**

I&#8217;m pretty sure most academics have heard about the psychology replication crisis; there&#8217;s a lot of talk about it. Given this and the fact that there have been many more replication efforts in psychology than in other fields, I&#8217;ll just stick to the empirical data for my priors. 

**Education:**

With the exception of [research on exceptional children](https://adamlgreen.com/smpy/) and educational acceleration/tracking (as they&#8217;re grounded in strong psychometric foundations), most education research won&#8217;t replicate, I imagine. 

Per [Inside Higher Ed](https://www.insidehighered.com/news/2014/08/14/almost-no-education-research-replicated-new-article-shows), &#8220;Only 0.13 percent of education articles published in the field’s top 100 journals are replications, write Matthew Makel, a gifted-education research specialist at Duke University, and Jonathan Plucker, a professor of educational psychology and cognitive science at Indiana University. In psychology, by contrast, 1.07 percent of studies in the field’s top 100 journals are replications, a 2012 study found.&#8221; 

Education research also places a premium on novelty (which is what happens when you&#8217;re grasping at straws for an education intervention that produces long-lasting, positive effects):<figure class="wp-block-embed-youtube wp-block-embed is-type-video is-provider-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio">

<div class="wp-block-embed__wrapper">
  <span class="embed-youtube" style="text-align:center; display: block;"></span>
</div></figure> 

With regard to specific replication failures in education research, growth mindset comes to mind (which I suppose is part of Psychology, too). Though initially hyped (TED talks and all), the most recent, largest replication studies have all flopped, demonstrating tiny effect sizes. Five days after posting a preprint of one such massive replication, the authors took the preprint down:

<blockquote class="twitter-tweet">
  <p lang="en" dir="ltr">
    This is extremely strong evidence that growth mindset does not have any important causal impact on academic achievement. It was a huge embarrassment for the authors, and they removed the preprint 5 days later. <a href="https://twitter.com/hashtag/psychology?src=hash&ref_src=twsrc%5Etfw">#psychology</a> <a href="https://twitter.com/hashtag/edutwitter?src=hash&ref_src=twsrc%5Etfw">#edutwitter</a> 3/
  </p>— Russell T. Warne 🇺🇸🇨🇱 (@Russwarne) 
  
  <a href="https://twitter.com/Russwarne/status/1107555420636274688?ref_src=twsrc%5Etfw">March 18, 2019</a>
</blockquote>

When pressed about the minuscule effect sizes, Dweck (the researcher who popularized mindset theory) was evasive:<figure class="wp-block-embed-youtube wp-block-embed is-type-video is-provider-youtube wp-embed-aspect-4-3 wp-has-aspect-ratio">

<div class="wp-block-embed__wrapper">
  <span class="embed-youtube" style="text-align:center; display: block;"></span>
</div></figure> 

Dweck is just a single bad-faith actor (\*cough\* [financial incentives](https://twitter.com/Russwarne/status/1159594269818138624?ref_src=twsrc%5Etfw%7Ctwcamp%5Etweetembed%7Ctwterm%5E1159594269818138624&ref_url=https%3A%2F%2Fpublish.twitter.com%2F%3Fquery%3Dhttps%253A%252F%252Ftwitter.com%252FRusswarne%252Fstatus%252F1159594269818138624%26widget%3DTweet) \*cough\*) in education/psychology research; she doesn&#8217;t represent the field as a whole. But the fact that growth mindset theory has been taken seriously for this long and still won&#8217;t die suggests that education research is hostile to dissent and has bad epistemic hygiene. 

Other educational claims that have failed, are p-hacked to death, or have inflated/overhyped effect sizes (that I can recall off the top of my head):

  * Flipped classrooms, which _[exacerbate](http://seii.mit.edu/research/study/effects-of-the-flipped-classroom-evidence-from-a-randomized-trial/)_ [achievement gaps](http://seii.mit.edu/research/study/effects-of-the-flipped-classroom-evidence-from-a-randomized-trial/) between the worst and best students
  * Teacher value-added studies, which have tiny effect sizes (viz., work done by Raj Chetty, who is an economist)
  * Early-life educational interventions to improve academic outcomes (viz., the work of Heckmann); these interventions seem to have a positive effect on non-academic outcomes, though. That said, the literature is [rife with publication bias](https://rpubs.com/EmilOWK/pub_bias_early_intervention).

**Criminology and Sociology:**

<blockquote class="wp-block-quote">
  <p>
    In criminology journals in particular, <strong>replication studies constitute just</strong> <strong>over 2 percent of the articles</strong> published between 2006 and 2010. Further, those replication studies that were published in criminology journals in that period tended to conflict with the original studies.
  </p>
  
  <cite><a href="https://journals.sagepub.com/doi/abs/10.1177/1477370815578197?journalCode=euca">&#8220;Replication in criminology: A necessary practice&#8221;</a></cite>
</blockquote>

I don&#8217;t know much about criminology, but apparently it does replications at twice the rate of psychology, which bodes well. However, like education research and psychology, [criminology has](https://osf.io/qmeba/) extolled novel interventions that ended up not replicating with similarly large effect sizes. 

In Sociology, on the other hand, a large proportion of researchers aren&#8217;t willing to release their data (see this informal 2015 [study, N = 53](https://orgtheory.wordpress.com/2015/08/11/sociologists-need-to-be-better-at-replication-a-guest-post-by-cristobal-young/)), suggesting a lack of replication culture. Here&#8217;s what the sociologists [Jeremy Freese and David Peterson](https://osf.io/preprints/socarxiv/5bck9/) have to say: 

<blockquote class="wp-block-quote">
  <p>
    As sociologists, the most striking thing in reviewing recent developments in social science replication is how much all our neighbors seem to be talking and doing about improving replicability. Reading economists, it is hard not to connect their relatively strict replication culture with their sense of importance: shouldn’t a field that has the ear of policy-makers do work that is available for critical inspection by others? The potential for a gloomy circle ensues, in which sociology would be more concerned with replication and transparency if it was more influential, but unwillingness to keep current on these issues prevents it from being more influential. In any case, the integrative and interdisciplinary ambitions of many sociologists are obviously hindered by the field’s inertness on these issues despite the growing sense in nearby disciplines that they are vital to ensuring research integrity.
  </p>
</blockquote>

Unsurprisingly, like in most social sciences, [we see evidence](https://www.gwern.net/docs/statistics/bias/2008-gerber.pdf) of publication bias:<figure class="wp-block-image">

<img loading="lazy" width="620" height="557" src="https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/soc_pub_bias.png?resize=620%2C557&#038;ssl=1" alt="" class="wp-image-1376" srcset="https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/soc_pub_bias.png?w=658&ssl=1 658w, https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/soc_pub_bias.png?resize=300%2C269&ssl=1 300w" sizes="(max-width: 620px) 100vw, 620px" data-recalc-dims="1" /> </figure> 

**Political Science:**

I don&#8217;t know much about political science, but it seems to have had its fair share of shoddy findings and [data fabrication](https://www.nytimes.com/2015/05/26/science/maligned-study-on-gay-marriage-is-shaking-trust.htmlhttps://www.nytimes.com/2015/05/26/science/maligned-study-on-gay-marriage-is-shaking-trust.html). That said, researchers have responded with [calls for better epistemic hygiene practices](https://politicalsciencereplication.wordpress.com/2018/07/14/replication-and-transparency-in-political-science-did-we-make-any-progress/) and journals have adjusted accordingly. There&#8217;s even an [active page](https://dataverse.harvard.edu/dataverse/gov2001) with replications of prominent political science papers.<figure class="wp-block-embed-youtube wp-block-embed is-type-video is-provider-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio">

<div class="wp-block-embed__wrapper">
  <span class="embed-youtube" style="text-align:center; display: block;"></span>
</div></figure> 

**Management and Marketing**

Management and Marketing (M&M) seem to be a mix of social psychology, industrial/organizational [(IO) psych](https://www.apa.org/ed/graduate/specialize/industrial), and political science. For example, one of the [most cited articles](https://academic.oup.com/jpart/article/27/1/197/2629303) in a top M&M journal showcases some priming interaction effects, which is essentially something straight out psychology (that, we should note, hasn&#8217;t had the best replication record). So, we might imagine that the replication rate of M&M will be equal to that of psychology. 

Unfortunately, there&#8217;s not a lot of data out there on M&M replication. It&#8217;s clear that the field [doesn&#8217;t talk about replication much](https://www.tandfonline.com/doi/full/10.1080/14719037.2017.1282003#), though [apparently](https://link.springer.com/article/10.1007/s11301-018-0149-3) &#8220;_Management Review Quarterly (MRQ)_&nbsp;[a top journal] publishes structured literature reviews, meta-analyses and, since 2018, replications.&#8221;

My impression is that **Replication Markets participants are systematically underpredicting the replicability of research in Management and Marketing**, probably because many of them are technical types allergic to business, marketing, and soft skills (even though most M&M papers aren&#8217;t specifically about those topics). This presents an interesting opportunity. 

#### My Priors

So, I&#8217;ll put my money where my mouth is (metaphorically, as there is no financial downside, just opportunity cost and being wrong) and provide my replication base rates:

**Economics:** 60 ± 5%

**Psychology:** 55 ± 5%

**Marketing and Management:** 50 ± 10%

**Political Science:** 45 ± 10% 

**Sociology and Criminology:** 45% ± 10% 

**Education Research:** 40 ± 10% (I hope my priors aren&#8217;t too influenced by my research on the topic)

## Will Replication Rates Vary Significantly By Year?

One might intuit that as norms around scientific best practice change, so too will the quality of science. How could we confirm this before the replications are attempted? 

A naïve approach would be to look at Google search term trends over time. For example, here are the trends for &#8220;psychology replication&#8221; and &#8220;open science&#8221; from 2004 to 2019:<figure class="wp-block-image">

<img loading="lazy" width="1676" height="841" src="https://i2.wp.com/adamlgreen.com/wp-content/uploads/2019/08/Untitled-picture.png?fit=640%2C321" alt="" class="wp-image-1379" srcset="https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/Untitled-picture.png?w=1676&ssl=1 1676w, https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/Untitled-picture.png?resize=1024%2C514&ssl=1 1024w, https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/Untitled-picture.png?resize=300%2C151&ssl=1 300w, https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/Untitled-picture.png?resize=768%2C385&ssl=1 768w, https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/Untitled-picture.png?resize=900%2C452&ssl=1 900w, https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/Untitled-picture.png?resize=1280%2C642&ssl=1 1280w" sizes="(max-width: 620px) 100vw, 620px" /> </figure> 

A better approach would be to look at trends in journal articles, as these are written by those who actually write the journal articles. Using [Dimensions.ai](https://app.dimensions.ai/analytics/publication/overview/timeline?search_text=replication%20AND%20psychology&search_type=kws&search_field=full_search), we see that use of the terms &#8220;replication&#8221; and &#8220;psychology&#8221; in publications has gone up over time, doubling between 2010 and 2018:<figure class="wp-block-image">

<img loading="lazy" width="620" height="423" src="https://i2.wp.com/adamlgreen.com/wp-content/uploads/2019/08/dimensions_econ.png?resize=620%2C423&#038;ssl=1" alt="" class="wp-image-1378" srcset="https://i2.wp.com/adamlgreen.com/wp-content/uploads/2019/08/dimensions_econ.png?w=930&ssl=1 930w, https://i2.wp.com/adamlgreen.com/wp-content/uploads/2019/08/dimensions_econ.png?resize=300%2C205&ssl=1 300w, https://i2.wp.com/adamlgreen.com/wp-content/uploads/2019/08/dimensions_econ.png?resize=768%2C524&ssl=1 768w, https://i2.wp.com/adamlgreen.com/wp-content/uploads/2019/08/dimensions_econ.png?resize=900%2C615&ssl=1 900w" sizes="(max-width: 620px) 100vw, 620px" data-recalc-dims="1" /> </figure> 

Likewise with [economics](https://app.dimensions.ai/analytics/publication/overview/timeline?search_text=replication%20AND%20economics&search_type=kws&search_field=full_search), which has seen a similar 2x increase:<figure class="wp-block-image">

<img loading="lazy" width="620" height="421" src="https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/Untitled-picture-econ.png?resize=620%2C421&#038;ssl=1" alt="" class="wp-image-1380" srcset="https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/Untitled-picture-econ.png?w=930&ssl=1 930w, https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/Untitled-picture-econ.png?resize=300%2C204&ssl=1 300w, https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/Untitled-picture-econ.png?resize=768%2C521&ssl=1 768w, https://i0.wp.com/adamlgreen.com/wp-content/uploads/2019/08/Untitled-picture-econ.png?resize=900%2C611&ssl=1 900w" sizes="(max-width: 620px) 100vw, 620px" data-recalc-dims="1" /> </figure> 

The trends look similar for all other social science fields being replicated in SCORE. However, these graphs show total publications over time, which increase as the fields grow larger. **If we compare these trends to the number of publications in the fields as a whole, we see that the number of publications with the term &#8220;replication&#8221; has kept pace with the field (that is, it hasn&#8217;t accelerated).**&nbsp; 

This is what we&#8217;d expect. Yes, there have been some incredibly cool developments in open science over the past five years or so, like the Open Science Framework (OSF), which takes the friction out of preregistration, public sharing of data, methods, code, and more. There have also been a few notable replication projects. Many of these things are possible thanks to the Center for Open Science (COS), which is funded by [Arnold Ventures, DARPA, and others.](https://cos.io/about/our-sponsors/) In 2016 the COS released new opensource preprint servers (e.g., PsyArXiv), which has coincided with increased publication of preprints (which have been available in the hard sciences [for nearly 30 years](https://en.wikipedia.org/wiki/ArXiv), and in [biology for around 5](https://www.nature.com/articles/d41586-019-00199-6).)&nbsp; All of these trends have conspired to make science more open, presumably limiting publication bias, p-hacking, the [garden of forking paths](http://www.stat.columbia.edu/~gelman/research/unpublished/p_hacking.pdf), and other forms of academic malpractice and epistemic pollution.

**All that said, talk is cheap. Though these trends indicate a growing awareness of replication and scientific best practices, it doesn&#8217;t guarantee that such trends have affected social scientists.** My subjective impression from various academic Twitter-verses is that young scientists tend to be quite excited about open science, replication, etc., whereas older, more established scientists aren&#8217;t quite as excited.

The question is: do these young scientists publish in the high-prestige journals that Replication Markets will investigate? Probably so, but the majority of papers are likely published by better-established, older scientists. **I think there will be a 10-year lag before we see the quality of science increase significantly.** 

So, no, I don&#8217;t believe replication rates will vary a lot over time. Yes, there will probably be a slight upward trend, maybe about 1-2% per year, but I imagine much more of the variation will be among fields.

## Forecasting Specific Claims

How should we forecast specific claims? 

If we wanted to be lazy (i.e., use heuristics), we&#8217;d take [the outside view](https://wiki.lesswrong.com/wiki/Outside_view) every time, meaning we&#8217;d bet the replication rate of study X would be equal to the replication rate of the field as a whole. If we have an inkling of epistemic humility, we might update this to reflect the belief of the prediction market as a whole, as prediction markets [have been shown](https://www.pnas.org/content/112/50/15343) to be [pretty good](https://www.sciencedirect.com/science/article/pii/S0167487018303283) at predicting replication outcomes.

However, if we have subject-matter expertise, or are willing to do a bit of digging, we might take the inside view and update these priors accordingly. 

### General Principles

1. Start with the replication rate for the field as a whole or, absent that, the replication rate for social science as a whole updated with our prior for the specific field.

2. Update on any relevant knowledge you might have, but only slightly. This is a gross simplification, but: forecasting tournaments show that **small, incremental updates of our priors result in the best forecasts.** 

3. Be skeptical of certain methods (e.g., difference-in-differences designs in economics, as I discussed before) and statistical effects. For example, give less credence to interaction effects, as they [require a much larger sample size](https://statmodeling.stat.columbia.edu/2018/03/15/need-16-times-sample-size-estimate-interaction-estimate-main-effect/) to [be properly estimated](https://approachingblog.wordpress.com/2018/01/24/powering-your-interaction-2/) and aren&#8217;t as likely to hold up in replication:

<blockquote class="wp-block-quote">
  <p>
    Interaction effects are notorious for being much easier to publish than to replicate, partly because it is easy for researchers to forget (?) how they tested many dozens of possible interactions before finding one that is statistically significant and can be presented as though it was hypothesized by the researchers all along.
  </p>
  
  <p>
    Various things ought to heighten suspicion that a statistically significant interaction effect has a strong likelihood of not being “real.” Results that imply a plot like the one above practically scream “THIS RESULT WILL NOT REPLICATE.” There are so many ways of dividing a sample into subgroups, and there are so many variables in a typical dataset that have low correlation with an outcome, that it is inevitable that there will be all kinds of little pockets for high correlation for some subgroup just by chance.
  </p>
  
  <cite><a href="https://scatter.wordpress.com/2008/08/19/lil-didactic-aside/> &#8220;>Jeremy Freese</a></cite>
</blockquote>

#### 4. Use your gut and have fun!