{:date #inst "2021-11-29" :subject ""}

*You can give feedback via email, [Discord](https://discord.gg/xAumsfVyRd) or [Twitter](https://twitter.com/the_sample_umm).*

Updates from the past week (I discussed some of these in last week's announcements):

 - I've finished migrating to a new backend system for generating recommendations and sending emails. No user-visible changes, but it makes my life easier.
 - Non-English newsletters are now given higher priority than English newsletters for people who speak the relevant language. I've noticed we've been getting a few more one-click subscribes for non-English newsletters now (mainly Italian).
 - Newly submitted newsletters are now boosted until they've received at least 150 organic forwards. (For the "boosted" forwards, we just pick a random person to send them to). This helps the algorithm collect data on new newsletters so that it can make more intelligent recommendations.
 - The charts in the publisher console now update daily (about 4 PM Pacific) instead of weekly. Note that the right-most value of each chart will be incomplete until the week finishes (Saturday evening). I wanted to indicate that with dotted lines etc but it looked like a headache. I've also fixed some minor bugs with the charts.
 - You can now edit your newsletter's URL from the publisher console.

I also started writing [my personal newsletter](https://jacobobryant.com/newsletter/2021-11-28/) again. (Got three new subscribers from The Sample already!)

Stuff in the pipeline (again, some of this I mentioned last week):

 - Demo button. Let people get the next two issues of a newsletter if they're on the fence about subscribing.
 - Send time optimization. Try to send emails in the morning for everyone, not just people in the Americas.
 - Various other funnel optimizations--planning to do a little work on the landing page, welcome emails and daily email design, before I start spending a bunch (more) money on ads.
 - Make the publisher console load faster. It takes like 5 seconds currently because it's running some slow queries (for the statistics) every time you go there.
 - Take location into account for recommendations. This will help with local/region-specific newsletters.
 - Some algorithm improvements and a handful of other behind-the-scenes/maintenance stuff.

I'm hoping to power through all that quickly and then take a break from writing code (for The Sample, at least) for a while; instead focusing on growth. We're still trying to see if we can get FB ads to work, and I'm still planning on giving newsletter ads another go. I'd like to get into more of a writing habit again as well (hence starting up my personal newsletter again).

I'll also do some thinking about how I might pitch more people on cross-promotion. We've had several people share referral links recently which each resulted in a large number of subscribers (80 - 180 each), which will be pushing the limits of how many subscribers we can give in return with our current list size. I'm interested to see if we can match in all cases or if we'll need to keep promoting them as we get more subscribers. Either way, I'll update [the performance csv](https://docs.google.com/spreadsheets/d/1pVQC7WznrQ8MNaRrmbfIDbutvnjbKGaB_rtXcXmFjFc/edit#gid=0) in a few weeks. Hopefully we continue to reciprocate well and I'll thus have more positive data points to show potential partners.

Jacob
