{:date #inst "2021-10-04" :subject "; new blog post: Why I changed my mind about advertising"}

*You can give feedback via email, [Discord](https://discord.gg/xAumsfVyRd) or [Twitter](https://twitter.com/the_sample_umm).*

First, a quick reminder: if your newsletter uses double opt-in, you might want to periodically download the CSV of 1-click subscribers from the publisher console and import it, in
case any of them didn't click the confirmation link. Especially if you're using paid forwards&mdash;I'd hate for you to pay for a subscriber and then not actually
get them on your list. The 1-click subscribe link is effectively the same as clicking a confirmation link, as long as you trust
me to not lie about who clicked it.

I've just published a new post, "Why I changed my mind about advertising." If you want to share it, here's a link with your newsletter's
referral code: [https://thesample.ai/blog/advertising/?ref={{ nl.nl/ref-code }}](https://thesample.ai/blog/advertising/?ref={{ nl.nl/ref-code }}). There's also a [Twitter thread](https://twitter.com/the_sample_umm/status/1445084733969289216). I
also finished the other article I mentioned I was working on last week, "Curating the curators" ([referral link](https://thesample.ai/blog/curating-the-curators/?ref={{ nl.nl/ref-code }}) | [Twitter](https://twitter.com/the_sample_umm/status/1443224795470962692)).

Here are my current ideas for future blog posts:

**Designing a recommendation algorithm to boost long-tail content**. Probably need to work out a catchier title, but this would explain (in a mostly non-technical way)
   how The Sample attempts to help small newsletters get more traffic instead of simply forwarding already popular and well-known newsletters.
   In a nutshell, one of the metrics we optimize for is the [gini index](https://en.wikipedia.org/wiki/Gini_coefficient), which we use to measure
   how "equal" newsletters are in terms of how many forwards they've received. It's the same metric used to measure income inequality in populations.
   More generally, I think a lot of people don't realize how much potential there is in using recommendation algorithms to boost long-tail content.
   I suspect this is because most people's perceptions of recommendation algorithms are shaped by their experiences with the large tech platforms,
   which are partly (in)famous for their use of recommendation.

**Farming serendipity**. When you're trying to get something off the ground, the biggest advances often come somewhat randomly. For example,
   about half of The Sample's subscribers came from Recomendo featuring us one week. Yet the amount of direct effort I put into that (about 30 seconds
   to fill out their submission form) is miniscule to all of the other (mostly futile) attempts I've made to get subscribers. I think it helps
   to build habits + a mindset around this kind of thing. You want to be able to react to lots of unforeseen opportunities rather than just trying to create
   opportunities, if that makes sense.

**The future of social media is email**. There's a lot of angst around big tech and content moderation, and I think we'd all like ways
   of finding and discussing great content without having to wade through so much... non-essential stuff. Some of the discussion focuses on decentralization
   in various forms. However, decentralization has its downsides too. In general, when designing software systems, you want a thin-ish foundation that's decentralized, with various centralized things built on top. I think we need *more* decentralization than we currently have, but we don't necessarily need to go all the way to
   e.g. blockchain. I think email is the most promising path forward: it's a decentralized system *that everyone already uses*, and it's Good Enough.
   I think lots more people should be thinking about how to build interesting new applications on top of email. The Sample is obviously one example,
   but I have a few more ideas too.

 **How The Sample has helped newsletters get 10,000 more subscribers**. Within the next two weeks, we'll have hit the milestone of 10k "subscribe in 1 click" links
   clicked. I'm planning to write a general explainer about what The Sample is, how it works behind the scenes, business model, etc etc anything else
   that might be interesting. Probably will include a bunch of charts and statistics. Might be good for pitching to certain people/publications, like the Indie Hackers newsletter.
   
I've also got a handful of updates planned:

 - Tweak the way the algorithm repays referral link credit. Basically, we dedicate 10% of forwards to people who have shared their referral link, in proportion
   to how many subscribers they've referred. If 1% of the referrals have come via your referral link, then you should receive 1% of all our referral-repayment forwards. However there are different orders in which we can repay referrals, and I think some are better than others. For example, if you've referred some subscribers to us but haven't received any subscribers from us yet, then we probably want to prioritize your newsletter over someone else who has already received some subscribers from us, even if you've both made the same number of referrals. However we don't want to give *too much* prioritization, otherwise we'll end up always prioritizing newsletters that simply have low conversion rates (either because our subscriber base just doesn't include many people in the relevant niche yet, or because the author needs to improve their writing, or because our algorithm isn't smart enough to figure out which of our subscribers would be interested). Anyway, I have some small experiments I'd like to try, and I'll continue monitoring how equitable it is.

 - Add a chart showing the # of forwards you've received by day (perhaps for the past 30 days) to the publisher console and email report. Right now we just tell you how many forwards etc. you've received in total,
   and you can see it broken down by issue in the publisher console.

 - Improve the way we boost long-tail newsletters. This is related to my discussion above about the Gini index. The way we optimize for it right now is kind of ok
   but could be better. We've had some ideas lately for improving it. Ideally it'd be nice if we could say "X% of newsletters get at least Y forwards per week," with relatively high values for X and Y. Though obviously we'd like to do that while still sending people newsletters that we think they'll personally enjoy.

At some point I might also like to add a "demo" feature where people can opt to receive 2 more issues from a newsletter (so they can try it out a bit more
before deciding if they want to subscribe). However I've decided this is non-essential and should wait until after we're growing consistently (we're not, by the way--we've been on a plateau for a few months, hence my recent focus on blogging). I'd also like to A/B test it too. In some cases, this will result in people subscribing
who otherwise wouldn't have, but it could also have the opposite effect: people who would've hit 1-click subscribe instead do a demo and then don't subscribe. That's
not necessarily a bad thing (I mean, still seems like a positive thing from the reader's perspective), but it'd be nice to see just how big the effect is in both directions.

In any case, that'll probably wait until after I write integrations to automate the 1-click subscribes....

Jacob
