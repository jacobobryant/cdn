{:date #inst "2021-09-13" :subject ", edit title & description, algorithm improvements, classified ads"}

*You can give feedback via email, [Discord](https://discord.gg/xAumsfVyRd) or [Twitter](https://twitter.com/the_sample_umm).*

**Edit title & description**

You can now edit your newsletter's title and description from the publisher console:

![image](https://user-images.githubusercontent.com/3696602/133164547-b6aac9d1-65f3-4751-a4d2-744dcc60772b.png)

**Algorithm improvements**

We made the algorithm more strict about sending you newsletters that match the interests you selected when you signed up. It does this for 50% of
your recommendations; the rest will still have lots of variety.
We started this in an A/B test early last week, and after a couple days it looked like it was actually hurting the algorithm's performance,
since average rating went down. However we later noticed that the total number of ratings we collected went up significantly; i.e. the changes
made people more likely to rate the newsletters.

We started tracking another metric: "positive feedback rate," which is the percentage of recommendations that result in a 1-click subscribe or a 4- or 5-star review.
The positive feedback rate for the new change went up significantly for the new algorithm changes. We think that low ratings are at least a sign that the newsletter was interesting enough for the user to engage with instead of ignoring it completely, kind of like how they say it's a healthy sign when you get a bunch of unsubscribes after sending out an email. Average rating doesn't take that into account, so going forward we'll probably pay more attention to the positive feedback rate when evaluating A/B tests.

As part of all that, I made it so you can update your interests. Click "change settings" at the bottom of one of The Sample's emails.

![image](https://user-images.githubusercontent.com/3696602/133165595-493f99e9-a6eb-4091-a9a8-f7f6d4b79c73.png)

I was originally planning to make an announcement about this to everyone, but I'm concerned about emphasizing the recent algorithm improvements too much.
There's been an improvement, but it's incremental and I don't want to give the impression that we've made bigger changes than we actually have. We'll continue making improvements, and maybe we'll just let people find the new settings on their own.

(Oh, and you can set additional languages now. We don't have many non-English newsletters in the database currently, but I felt bad turning people down when they submitted them.)

**Classified ads**

I re-enabled the ad page. Ads are no longer targeted; instead they work like other newsletters: you book a day and then your ad goes to everyone on that day (not including the 10% of subscribers who get a paid forward). I've scheduled some of our old classified ads to run over the next several days. I'm not sure how the ROI of this will compare to paid forwards. I'm guessing that paid forwards are a better option for newsletters and the classified ads should be left for other kinds of products, but we'll see. After we have some more data, I'll include the median number of clicks.

![image](https://user-images.githubusercontent.com/3696602/133165987-03fbd9ec-4c8d-4262-a99b-3e74a323dbd0.png)


**Future work**

One other update: I added this fancy little graph to the [submit page](https://thesample.ai/submit/):

![image](https://user-images.githubusercontent.com/3696602/133169361-bb4813fa-3d9b-4db0-9d6a-a3432901b7cf.png)

It's part of a new growth strategy. I'm going through newsletters in our database that weren't submitted by the author (i.e. subscribers mentioned them in
response to "what other newsletters do you subscribe to" when they signed up, and I added them) and have a high conversion rate. I email the author
(which is easy because I have each newsletter's Reply-To address in our database already) and say basically "Hey I run this thing, I added your newsletter a while ago
and we've got you some subscribers already, here's a CSV of them, do you want to do some cross promotion and get even more subscribers, here's a graph with
past performance cross promoting with other newsletters."

I've emailed a handful of people so far, and it's been pretty convenient at least. I could even make it totally automatic, but I do some manual vetting anyway (Scientific American probably isn't interested) so pasting a message into my email client is easy enough. I'm crossing my fingers that the response rate will be good. If this works, it might be all we need to grow fast.

Jacob
