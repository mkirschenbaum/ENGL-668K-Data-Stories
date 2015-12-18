*Below is Ed Summers' response to the submitted data stories...*

I really enjoyed reading the data stories that everyone was able to put
together. One phrase that will stick with me for a while is Jen's *hashtag
salad* as a term (or neologism really) for tweets that are mostly made up 
of a coordination of hashtags. I'm going to use it from now on!

I was surprised to find that the stories that established a strong personal voice were particulary effective in drawing out a narrative in the data. Perhaps I shouldn've have been, but I was :) I guess it makes sense that a narrative about data would need to have a narrator, and that the narrator needs a voice. So it stands to reason that attention to this voice is important for communicating the perspective that the data story is taking. I think this is one reason (among many) that humanists are needed in the STEM dominated field of data science. Voice and perspective matter.

Another important aspect to the stories that worked well was an attention to the
data. For example Michael's analysis of the device used (mobile vs desktop) and
time of day was quite interesting. The treatment is suggestive of the way the
data is intertwined with events in the physical world, and the degree to which
social media can and cannot mediate those events. Filipa's analysis of the use
of language (English, Spanish and Portuguese) by a particular individual in
different contexts was another example of this type of treatment.

But there were *many* interesting things that were discussed, so it's probably
not fair for me to start highlighting them. The stories contained several 
comments about the limitations of collecting data from Twitter using TAGS.
For example:

Andy:

> Not only does TAGS give us a very brief snapshot of a giant conversation, but we Twitter users must figure out what we need before too much time passes and the data starts to become very hard to draw out.

Dan:

> This is one limitation of TAGS, as it removes the physical layout of Twitter, requiring users to cut and paste hyperlinks to read the original content of tagged Tweets. 

> The first was that it still takes a human to connect all of the patterns together.  Google spreadsheets do not contain a function to sort text by theme, so the user still needs to look at the text to see if there is a pattern to the Tweets.

> The second is in the limitations of TAGS.  Setsuko and I were both initially surprised with the seemingly low volume of results we received.  After a little research, we realized that TAGS only collects seven to nine days of Tweets.

Ruth:

> Of course, it is impossible to tell just from the data how much @Farmerboy or the other’s meant to, or not, to refer to the Little House on the Prairie franchise.

DB:

> For me, temporality posed the largest problem in that it was important to time when to run the script to capture certain kinds of data.

>  Not only is the process capped by a maximum number of tweets archived at a specific moment, it is also difficult to explore a topic outside of the “now” because of its relegation to the last seven days, rather than allowing for a specified date range. Additionally, the more tweets I attempted to archive at one time, the greater likelihood the script would fail and yield zero results.

I thought I remembered mentioning that the search API was limited to the last
7-9 days, but even if I did I clearly didn't emphasize it enough. The search API
*does* restrict access mostly for business reasons since Twitter have a service
called [Gnip](http://gnip.com) which allows people to purchase access to
historical data in bulk. So, if you are interested in a topic, and don't want to
pay Twitter thousands of dollars for data, it is important to collect continuously over a period of time.

TAGS tries to do this for you by allowing you to schedule your search to be rerun, but there are [limits] to the size of a Google Sheet: 2,000,000 cells, or 111,111 TAGS rows. It also isn't clear to me how TAGS deals with duplicate data, or how it ensures that it doesn't have gaps in time. At any rate these observations about the limits of TAGS and the underlying Twitter API are great examples of getting insight into Twitter as a platform, in [Tarleton Gillespie]'s use of the term. If this sort of thing is of interest there is an emerging literature that looks at Twitter's as a platform, including these two recent papers that are focused on the APIs specifically:

Sandra González-Bailóna, Ning Wang, Alejandro Riveroc, Javier Borge-Holthoefer and Yamir Morenoc. Assessing the bias in samples of large online networks. Social Networks, 38:16–27, 2014. http://cosnet.bifi.es/wp-content/uploads/2014/04/SN_paper.pdf

K. Driscoll and S. Walker. Working within a black box: Transparency in the collection and production of big twitter data. International Journal of Communication, 8:1745–1764, 2014. http://ijoc.org/index.php/ijoc/article/view/2171

Just as an aside Twitter's [web search] isn't limited to the last 7-9 days like the API. For example you can [do a search] for the tweets mentioning the word `twttr` (Twitter's original name) before March 22, 2006 which will show you some of the first day of tweets from Twitter's founders. 

The comments also point to another limitation of TAGS as a tool. The spreadsheet has the text of the tweet, but it is extremely data centric. To see embedded media, the users profile information, the responses and the full presentation of the tweet it is necessary to visit the twett on the Web using the URL located in the `status_url` column. This can prove to be quite a barrier, when you are attempting to decode the intent or intended meaning of a message by simply browsing the spreadsheet. The additional context found in the human readable presentation of the Web page makes it much easier to get at the intent or meaning of a tweet. But how do you do this sort of analysis with thousands of messages? This raises good questions about distant reading, which also are an area where a DH perspective has a lot to offer to the data science profession.

[limits]: https://support.google.com/drive/answer/37603?hl=en
[web search]: https://twitter.com/search-advanced
[do a search]: https://twitter.com/search?f=tweets&vertical=default&q=twttr%20until%3A2006-03-22
[Tarleton Gillespie]: http://papers.ssrn.com/sol3/papers.cfm?abstract_id=1601487
