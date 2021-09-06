{:date #inst "2021-09-06" :subject ", paid forwards results, download subscribers"}

*You can give feedback via email, [Discord](https://discord.gg/xAumsfVyRd) or [Twitter](https://twitter.com/the_sample_umm).*

**Paid forwards results**

It's been four days since paid forwards started. My expectations were exceeded: I estimated it would generate about $10/day in revenue, but in fact daily revenue has been in the range of $20 - $40. This has been pretty invigorating&mdash;it's been 2.5 years since I quite my job to do entrepreneurship full-time, and now it looks quite likely that this will be sustainable.

Another surprise (though not so much in hindsight) is that the paid forwards have been pretty concentrated. 19 newsletters are participating, and the distribution of
forwards looks like this:

![image](https://user-images.githubusercontent.com/3696602/132256945-8cb212c6-965d-4a1f-b29b-ecbef6f66150.png)

In other words, most people are getting completely outbid. I mentioned that for the four people who had bought classified ads in the old system which hadn't finished running, I would convert your remaining ad spend into paid forwards credit and set the bid price at $0.75. Turns out that was a little naive&mdash;it seems the max bid price needs to be *at least* $1.50 - $2.00 in order to be competitive. (If you're one of those four people: I'll probably put classified ads back into the non-paid-forward emails soon, and then I'll start running your ads again like before). I added the median winning bid price to the publisher console as an attempt to make that more transparent:

![image](https://user-images.githubusercontent.com/3696602/132257518-9a44e0f4-37b2-4703-93d0-c872bc21b51d.png)

Ideally we'd give you some kind of (reliable) prediction, e.g. "With this max bid price, you'll probably get X forwards and Y subscribes per week." We might add that some time.

Keep in mind that your bid price is combined with the algorithm's predicted rating for each user. You can still win auctions against people with a higher bid
price if the algorithm thinks the user will like your newsletter more. As we improve the algorithm, the amount you'll have to bid to get subscribers will (maybe? hopefully?) go down.

**Download subscribers CSV**

I added a CSV download link to the publisher console so you can get a list of everyone who clicked the 1-click subscribe
link on your newsletter:

![image](https://user-images.githubusercontent.com/3696602/132257937-373b1a2c-39b9-4382-8f35-7786249cde7f.png)

For the sake of privacy, you'll need to verify ownership of your newsletter before you can download the CSV. The first
time you click the link, you'll go to a page that'll send a code to your newsletter's Reply-To address, then you paste the code
in. If you don't see the download link, try again after your next issue goes out. I only started recording the Reply-To address last week,
and if it's absent, the link won't be there.

The CSV includes email address, which issue they were forwarded, the time they hit "subscribe in 1 click," and (for paid forwards)
how much you paid for them.

**Future work**

Next up, I really need to do some more algorithm improvements. We've been getting more complaints from people getting newsletters that
aren't related to the topics they selected when they signed up. To an extent, this is [by design](https://silken-cafe-474.notion.site/About-The-Sample-a989b5bd39054b37a51432d6999beac3#9571b2d19732498eb23774ce42aac99f)&mdash;but only to an extent. We need to hit the right balance between showing people
things they expect to receive and showing them new things outside their current/explicit interests, and we're still weighted too heavily on the latter.
Fortunately, with the crowd-sourced keywords we've been collecting, this'll be easier to fix now. So that's what I'll be up to for the next day or two. Hopefully this
will improve our retention, which has been slipping a bit.

(That is, after I write some code to actually charge people for the paid forwards. We've made about $135 on paper, though it isn't quite in the bank yet!)

After that, I'll start doing classified ads again, though I won't put them in the paid forwards. I'm going to simplify it. I'll just let people pick a day(s)
and then show the same ad to everyone on that day, like every other newsletter does. Later on, if we're selling out all our inventory, we might make them targeted again.

I also have a handful of minor improvements planned, like letting you edit your newsletter's title and description from the publisher console.

Jacob
