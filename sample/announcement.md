{:date #inst "2021-08-30" :subject " + paid forwards"}

Big news: I've replaced our classified ads with a paid forwards system. You can access it from
your (new) [publisher account]({{ signin }}), which replaces the stats links I've been giving people when they submit their newsletters.
There's a form that looks like this:

![image](https://user-images.githubusercontent.com/3696602/131396648-1ce89bbe-b59a-4baf-b8ec-1694c537eddf.png)

After I flip the switch, we'll start dedicating 10% of the emails we send to paid forwards. For each of those forwards, we'll estimate how
likely the user in question is to subscribe to your newsletter and then we'll multiply that percentage by your bid price.
We'll pick whichever newsletter has the highest score. If we pick your newsletter and the user clicks the "subscribe in 1 click" button, then we'll charge
the minimum amount you would've had to bid in order to win the auction. I haven't actually written the code to charge your card yet, but we'll probably wait until you owe at least $15 or something.

Note that we won't charge for people who go to your landing page and subscribe there, since we
have no way to measure that. So if you know how much you can spend to acquire a subscriber, you could set a higher bid price and still get good ROI.
I don't know what percentage of subscriptions are direct instead of via the 1-click links, but one person said it was about 50% for their newsletter.

Also, to give you a sense of scale, we currently generate about 800 1-click subscribes per week, so paid forwards _at most_ will result in 80 per week. I don't expect that we'll hit anyone's maximum weekly spend... but that'll change with time!

One last note: for those of you who have already bought ads, if we haven't gotten you 20 clicks yet, I'll convert your balance over to the new system and set your bid price at $0.75 (since the old pricing was $0.75 per click). If you'd like to continue doing paid forwards after the balance runs out, just add a payment method.

Besides that, I've also added a couple more small features to your publisher account. You can pin an issue, in which case we'll always forward that one instead of the most recent issue; and you can also send yourself a test email so you can see what an issue will look like when we forward it.

![image](https://user-images.githubusercontent.com/3696602/131399951-6e23f3e1-6d96-4384-9591-5204f1c5ca65.png)

Last month I talked about how I was considering making a directory of all the newsletters that have been submitted to us. I got a fair amount of positive feedback, and at some point I think it'll be a good thing to do. However I've decided to shelve the idea for now. I just don't think it's essential enough to spend time on at this early stage.

**Future plans**

Now that we have a much better monetization setup, I'm not planning on any big changes until sometime far away in the future. My priorities are to refine what we have, keep improving the algorithm, and get more subscribers. On the topic of refinement, I'd like to add a Zapier integration or similar soon so that 1-click subscribers can be imported to your lists immediately instead of me pasting them into your landing page after a few hours. With that I'll also include a CSV download link which will include a list of all the subcribers we've sent you. However before either of those happen, I need to add a verification step so that we know you're actually the owner of the newsletter you've submitted. Probably we'll send a 4-digit code to the email address that sends your newsletter, then you paste it into a form.

As for getting new subscribers, I am, ahem, hoping that sending these reports regularly will increase the number of people who share referral links. I'll also do some more work on the newsletter submission page, including adding some info about paid forwards. I've been tweeting more regularly from [The Sample's Twitter account](https://twitter.com/the_sample_umm), which you should follow by the way, and in general I'm keeping my eyes out for opportunities to tell newsletter authors about The Sample. If you have any leads or other growth ideas, please let me know!

Jacob
