{:date #inst "2021-11-22" :subject ""}

*You can give feedback via email, [Discord](https://discord.gg/xAumsfVyRd) or [Twitter](https://twitter.com/the_sample_umm).*

Just a few notes this week. Last week I talked about buying ads in newsletters. I spent a few hours sourcing newsletters, and then I decided it'd be best to
finish all my coding tasks first and then focus more fully on ads, rather than trying to do both concurrently. I do have the results from the ad I ran in Maker Mind on Thursday: 63 clicks, 39 unique clicks, and 18 signups, for a CPA of $8.33.

As for coding, we just finished redoing the daily machine learning pipeline which calculates recommendations, and now we need to redo the parts that take those recommendations and send them as emails. There won't be any user visible changes, but going forward the code will be much easier for us to work with. After that, I'm making a few small product changes:

 - We'll start boosting non-English newsletters, so those will get forwarded relatively quickly to everyone who has selected the relevant language in their preferences. I'll also make a general announcement about this since a lot of our subscribers signed up before I added a language setting, and they may not be aware it exists.
 - Demo button. This has been suggested to me twice by regular subscribers and twice by publishers. I'll add a button to the bottom of the email, right after the 1-click subscribe link, that says something like "On the fence? [Demo this newsletter] and we'll send you the next two issues as they come in."
 - Send time optimization. Instead of sending everyone their email at 6 AM or so Pacific time, we'll look at the window of when people are usually active and try to pick the best time to send.
 - Various bug fixes with rendering emails and handling clicks. It seems for a small percentage of people, GMail messes up the rating links which causes them to show an "invalid link" page.
 - Maybe do some A/B testing on the landing page and/or email design.

While I work on that, my cofounder will be continuing to experiment with FB ads and running some more A/B tests on the recommendation algorithm.

By the way, there is one somewhat significant change that'll go out once we finish the refactoring work I mentioned. We're modifying how we handle cross-promotion. Going forward, we'll give you additional cross-promotion forwards until one of the following conditions is met:

- The number of 1-click subscribers you've received from cross-promotion forwards matches or exceeds the number of subscribers you've referred to us.
- You've received at least 100 cross-promotion forwards for each subscriber you've referred to us.

Right now we have a slightly more complicated system: we dedicate a fixed percentage (10%) of forwards to cross-promotion, and then we make sure you receive a share of the forwards in proportion to how many people you refer. With the new system, for those of you have sent us referrals: if you *didn't* get as many subscribers in return, you'll get some more forwards (the old system worked out to about 75 forwards/referral, so this'll be a 33% boost); if you *did* get as many subscribers in return and you've been continuing to receive cross-promotion forwards, you'll stop getting those forwards until you refer more people.

The new system requires less code, is easier to explain, and is IMO still fair. One downside is that if the algorithm has already "overshot" on cross-promotion, you might have to refer a bunch of people before it starts to do anything again. For example, if you've referred 20 people and received 30 people, you wouldn't get any more cross-promotion forwards until you've referred more than 10 additional people. I could do something to fix that, but only a handful of people are in this boat, and most people share the link just once or twice anyway, so I figure it's not a big deal.

Hopefully that all makes sense--let me know if you have any questions.

In other news, my 11-month old daughter got her first cold last week. I thought I would be safe thanks to my robust adult immune system, but alas, no. Fortunately that's over with now.

Anyone else have a tendency to start their newsletters with "just a short one this week" and then end up with 10 paragraphs anyway?

Jacob
