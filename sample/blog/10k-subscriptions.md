{:date #inst "2021-12-02"
 :title "How The Sample drove 10K newsletter subscriptions"
 :image "https://user-images.githubusercontent.com/3696602/139344829-ac9232b4-23a4-483a-bc84-bf947dafbb1f.png"
 :description "A couple weeks ago The Sample hit a big milestone: we've generated over 10,000 new subscriptions for other newsletters via our "subscribe in 1 click" links."}
 
A couple weeks ago The Sample hit a big milestone: we've generated over 10,000 new subscriptions for other newsletters via our "subscribe in 1 click" links. Since the product is evidently working to some degree, I thought this would be a good time to write a post explaining what we're doing, how we're doing it, how well it's working, and our future plans.

### What is The Sample?

I describe it as "a newsletter discovery service." After you sign up, we pick a different newsletter to forward you each day. If you like it, you can hit "subscribe in 1 click" and you'll get added to their list. You can also give a 1-to-5 star rating to help our recommendation algorithm learn your preferences better.

![image](https://user-images.githubusercontent.com/3696602/138955435-4a33da2b-c721-468d-8b6f-6015b2419a11.png)

As a reader, The Sample helps you discover a larger variety of things to read that you normally wouldn't run into. Although we ask you to select some topics you're interested in when you sign up, the algorithm treats those topics more as guidelines than rules&mdash;especially since many newsletters don't even fit into the predefined topics anyway.

*(Sound interesting? You can [subscribe here](https://thesample.ai/))*

The algorithm is also designed to promote long-tail newsletters instead of a few popular ones. We measure this with the Gini index, the same metric used to gauge income inequality in populations. We use a few simple techniques to improve newsletter equality while still trying to send people newsletters we think they'll like.

As a writer, The Sample helps you get more subscribers. If you [submit a link to](https://thesample.ai/submit/) your newsletter, we subscribe to it with an @import.thesample.ai address, and future emails you send will start getting forwarded to people based on how likely they are to subscribe. You also get access to the publisher console, where you can view statistics about the results you're getting.

![image](https://user-images.githubusercontent.com/3696602/138570383-0c512d8b-09d5-4944-8b24-3e1a9271cb88.png)

As alluded to by that screenshot, we dedicate a portion of forwards to cross-promotion and paid sponsorship (10% each, with the remaining 80% of forwards being organic). For paid forwards, we have a bidding system where writers can set a maximum price they'd be willing to pay per conversion (i.e. when someone hits "subscribe in 1 click") and a maximum weekly spend. If enabled, we charge for any 1-click subscribes that come from paid forwards&mdash;if no one subscribes, you don't pay anything. Paid forwards are always marked with the word "sponsored" at the top.

Cross-promotion forwards are given in return for sharing a referral link. Each writer gets a unique link and we track how many people subscribe to The Sample after clicking it. For example, if 1% of all the referrals we've received came from your referral link, then we boost your newsletter until you've received at least 1% of all the cross-promotion forwards. As of writing this, that works out to about 74 forwards per referral.

### Behind the scenes

There is a fair amount of ongoing manual work required to keep this running. To add newsletters, I made a bookmarklet to help copy over the metadata, and then I subscribe with a randomly generated address.

![demo of adding a newsletter](https://user-images.githubusercontent.com/3696602/138573313-330b82e0-5bd5-4c35-bfb2-7f5b87868a1e.gif)

Once we receive the next issue from a newly added newsletter, it can start getting forwarded by the algorithm. To make sure we don't forward welcome emails or promotions, I manually approve or hide each issue based on the subject line. I make mistakes regularly, but the upside is that it only takes 5 minutes per day.

![image](https://user-images.githubusercontent.com/3696602/138573717-a473d23b-1579-482c-840e-ddf173f7c787.png)

A much more time-consuming task is handling the 1-click subscriptions. I have two email folders ("one-click subs" and "paid subs," shown briefly in the GIF above) which receive alerts whenever someone hits "subscribe in 1 click." The alert includes an email address and a link to the newsletter's signup page; I paste the former into the latter and fill out any captchas. I spend 20 - 30 minutes per day on this. (Aside: I wish all subscription forms were as quick and painless as Substack's).

Besides all that, there is the never-ending work of optimizing the recommendation algorithm. My brother specializes in machine learning, and he's in charge of this. I handle all the day-to-day stuff so he can focus on improving our core product.

### Does it actually work?

Since I run into every single newsletter (and issue) before it gets forwarded to anyone, I don't actually use the product myself&mdash;though I do occasionally open issues that look interesting when I'm approving them. So I personally can't give much of a qualitative judgment, but I do get messages like this every now and then which I appreciate:

![image](https://user-images.githubusercontent.com/3696602/138574073-14995f89-d507-494c-b09a-d1519e19cce3.png)

I will mention that at this point, our recommendation algorithm isn't magic. It performs 50% better than purely random recommendations (based on the "positive reaction rate," i.e. the percentage of forwards that result in either a 1-click subscribe or a 4- or 5-star rating), but it often still *feels* random because it tries to send you a wide variety of things. So it probably works best for people who want and are expecting that.

As for metrics, we have 3,851 subscribers, open rate and click-through rate are 55% and 13% respectively, and the landing page converts unique visitors at 21%. The click-through rate for the "subscribe in one click" link is 2.8%.

**Note:** whenever I mention "subscribes" below, I mean only subscribes that happen via that link. Some people will subscribe the normal way by going to the landing page, so the actual number of subscribers we refer to other newsletters is higher than what's discussed below. I haven't done any experiments yet to estimate how many people subscribe without using the 1-click sub link, so for now I'll stick to what we can measure.

Here are some charts with our other main business metrics. All the data used to make these charts is available in [this spreadsheet](https://docs.google.com/spreadsheets/d/1XdEmHPzOpNOf_J35uQ_1_po3bSBL7h4Q4afWgLIaj7c/edit?usp=sharing).

![image](https://user-images.githubusercontent.com/3696602/139163917-4098d131-e994-4b15-a5bd-f83612a782dd.png)

The jump in July was from getting featured in Recomendo.

![image](https://user-images.githubusercontent.com/3696602/138969224-315c69ca-c9af-47e9-83be-f85286217a21.png)

By "active," I mean anyone who opened an email we sent.

![image](https://user-images.githubusercontent.com/3696602/139163850-34716604-b3f3-489f-88d6-1afaeafccea3.png)

I'd like to know how this compares to other daily newsletters.

![image](https://user-images.githubusercontent.com/3696602/139163552-c1a9dec6-019f-4503-9f71-8afadd1737db.png)

It's not enough to pay rent, but our operating expenses are covered.

Anyway, although we've been trapped on a plateau for a few months, I figure if we keep plugging along then we'll start growing consistently at some point. We've made enough progress that I no longer feel anxious about the opportunity cost of doing entrepreneurship full-time. (Long story short, it had already been two years since quitting my job when I got the idea for The Sample).

How well do we drive subscriptions for writers? I've got some more charts below, but in summary:

 - **Organic forwards:** you'll probably get a small handful of subscribers. If your newsletter appeals strongly to a general audience, you might get up to 75 subscribers.
 - **Cross-promotion forwards:** you can expect to get back five 1-click subscribes for every four subscribers you refer to The Sample (up to perhaps 80 referrals or so, since we have a finite subscriber base).
 - **Paid forwards:** if you're willing to pay $3 or more per subscriber, we can get you up to 10 or so per week.

Note that the following charts only include data from "active" newsletters, which I define as "has sent us at least one email in the past 30 days."

This chart breaks down 1-click subscribes by each newsletter's conversion rate, which is the percentage of forwards that result in a 1-click subscribe. A newsletter's conversion rate is partly a measure of its quality, but it's also affected (especially at this early stage) by how many subscribers we have who are interested in its topic (it's nicheness, basically) and how well our algorithm can figure out who those people are.

![image](https://user-images.githubusercontent.com/3696602/139163166-3cdf0bc1-59fe-4d9d-9cdc-f16b4c3f75d6.png)


The median newsletter has received 7 organic subscribers. (At least it's free!)

I keep close tabs on how well we're reciprocating for writers who share cross-promotion links. My main metric for this is the "paid-back rate," the percentage of newsletters which have referred at least five people to The Sample who have also received back at least as many 1-click subscribers as they've referred. I include newsletters in the metric once at least two weeks have passed since they shared the referral link, in order to give the algorithm time to reciprocate. Currently the paid-back rate is 95%. (If you include newsletters which have referred at least one person, the paid-back rate is 90%).

![image](https://user-images.githubusercontent.com/3696602/139157414-ec9da204-a9e6-4443-9bdf-ce3a225440d6.png)

Note that this chart includes only 1-click subscribes that came from cross-promotion forwards&mdash;organic subscribes are excluded.

We started paid forwards at the beginning of September. In total it's resulted in 576 subscribes with an average cost of $2.59 per subscriber, though the cost has been bid up since we started. Most people who are getting any results from paid forwards currently have set their maximum bid in the $3 - $4 range.

![image](https://user-images.githubusercontent.com/3696602/139162515-c6d625e1-f469-442c-b75e-08a6e33a046c.png)

### Going forward

Ideally The Sample's network will become strong enough that the best growth strategy for new writers is to simply improve their writing and then let the algorithm take care of the rest. Realistically, we'll see how close we can get. Our main focus for the foreseeable future will be improving the recommendation algorithm and getting more subscribers. I don't anticipate any significant user-facing changes for a long time (if ever), though I have some ideas for complementary products.

In the bigger picture, I'm excited for email. We've been hitting up against the limitations of large, closed social media platforms for a while, and I think email is the next frontier. It's an open protocol not controlled by any single entity, and *everyone already uses it.* I see The Sample as one piece of an emerging information ecosystem with smaller, interchangeable parts&mdash;and as a result, more innovation. For writers in particular, The Sample provides discoverability without locking you into a platform.
