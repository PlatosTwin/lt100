---
layout: page
---

## Some Data from the LT100

1. [Preamble](#preamble)
2. [Data](#data)
    * [The basics](#data-basics)
    * [Cumulative percentages](#data-cumulative-percentages)
    * [Age, gender, time](#data-age-gender-time)
    * [Splits](#data-splits)
    <!-- * [Split prediction](#data-split-prediction) -->
3. [Data sourcing and processing](#sources-processing)
4. [Footnotes](#footnotes)

<h3 id="preamble" class="header-seps">Preamble</h3>
I spent the summer of 2016—and 2017, 2018, and 2019—in Leadville, CO, working as an instructor at the Colorado Outward Bound School It was then that I first learned of the Leadville Trail 100. By the time I started at COBS, the organization had been running the Outward Bound Aid Station at the LT100 for a number of years and drew heavily from its staff to man the aid station and stock a pool of volunteer pacers. Having spent all summer working in the mountains, I figured I was up to the challenge of pacing and that first year accompanied a runner from Outward Bound to Mayqueen. The experience was incredible, and in 2017 I was lucky enough to pace a runner from Outward Bound all the way to the finish. 

![The author and the runner he paced in 2017, posing at the finish line.]({{"images/lt100_2017.jpg" | relative_url }})

While my course schedule didn't align with the race in 2018 and 2019, somewhere along the way I decided that I would one day run the LT100 myself. Until recently, this was a goal without much conviction behind it: in 2018 we moved from Colorado to New York City, and with the change of scenery it was challenging to hold on to the self I had grown into while living and working in the mountains.

...until David Roche set the course record at this year's LT100. I'm still many years away from running in the LT100 myself, but with David's record-setting debut—and a commitment to moving back to the Mountain West in the not-too-distant future—I wanted to reconnect with my own experiences with the race and to start taking seriously that one day it'll be running into the Outward Bound aid station. And so I did what I'm reasonably good at doing: I pulled some historical and played around with making some graphs.

To be clear, this data falls pretty solidly into the category that I call "data porn"—data that's interesting to look at but ultimately of little or no practical utility. Indeed, there are plenty of websites, blogs, and Reddit threads devoted to the topic of strategizing for ultras generally and the LT100 specifically, and those looking for practical advice should most certainly turn to sources such as those. The purely curious, however, can scratch their data itch here.

<h3 id="data" class="header-with-top">Data
<a href="#top" class="go-to-top">Go to top</a>
</h3>

<h4 id="data-basics">The Basics</h4>

The Leadville Trail 100 started in 1983 with 10 finishers; in 2024, it had just over 400.[^1] That's a 40x increase in finishes in roughly as many years—and assuming the DNF rate has remained approximately constant, which I think is likely, ditto for the number of entrants. But the race's growth trajectory has been far from steady, with just periods of rapid growth: 1987 and 1988, which initiated a trend that would last through 2008, and 2009 and 2010, which initiated the trend that dominates to this day. What happened in 2009 and 2010? These years follow on the heels of the financial crisis, so it's possible that recently unemployed bankers took up ultra running; much more salient, however, is that on May 5th, 2009, Christopher McDougall published _Born to Run_.

![Finishers by year, showing a 40x increase from 1983 to 2024.]({{"images/finishers_by_year.png" | relative_url }})

On their [SWAP Podcast](https://podcasts.apple.com/us/podcast/some-work-all-play/id1521532868), David and Megan Roche often say that we're in the middle of a performance revolution in endurance sports, with top times getting faster across a variety of events. Without saying anything about causation—because there are too many confounding variables to list—it's anecdotally interesting that we see this phenomenon in the LT100, but only among top finishers. For most everyone else, even the top 25th percentile, finishing times have remained roughly constant across the years.

![Top times and P25, P50, and P75 finishing times from 1983 to 2024.]({{"images/percentiles_by_year.png" | relative_url }})

<h4 id="data-cumulative-percentages">Cumulative percentages</h4>

The vast majority of DNFs take place prior to the 18-hour mark, making for a pretty even split in time between those who DNF and those who finish. Roughly, and all else being equal, if you make it past hour 18, odds are that you're not going to DNF.

![Cumulative percentage of runners—finishers and DNFs—by time on course, 2024.]({{"images/cumulative_all_runners_2024.png" | relative_url }})

Zooming into just those who finished the race, we can see that the median finishing time in 2024 was just north of 28:00. By the 24-hour mark, only about 15% of finishers had come through.

![Cumulative percentage of runners—finishers only—by time on course, 2024.]({{"images/cumulative_finishers_only_2024.png" | relative_url }})

The percentages vary slightly from year to year, but as a whole the shapes of both curves are surprisingly durable.

![Cumulative percentage of runners—finishers and DNFs—by time on course, 2017-2024.]({{"images/cumulative_all_runners_2017_2024.png" | relative_url }})

What's especially stunning in the chart below is the durability of the inflection point around the 25-hour mark. The rate at which runners cross the finish line in the few hours before the 25-hour mark is qualitatively quite different than the rate at which runners cross the finish line in the few hours after the 25-hour mark. For one reason or another, if you're not finishing ahead of the 25-hour mark, you're finishing (at least) several hours after it.

![Cumulative percentage of runners—finishers only—by time on course, 2017-2024.]({{"images/cumulative_finishers_only_2017_2024.png" | relative_url }})

<h4 id="data-age-gender-time">Age, gender, and time</h4>

Outside of the observation that older runners tend to be slower, there's not much of interest when we break down finishing times by age and gender. But, this graph does reinforce the oddity I pointed out just above, about the 25-hour mark being a sort of inflection point. Here, the inflection manifests as a decrease in "dot density" in the band between 25:00 and 26:00.

![Finishing time by age, colored by gender, from 1983 through 2024.]({{"images/finishing_time_age_gender.png" | relative_url }})

<h4 id="data-splits">Splits</h4>
For 2019 through 2024, we can also look at performance within splits—i.e., in between aid stations.[^2] Here, we're looking at [box and whisker plots](https://datavizcatalogue.com/methods/box_plot.html) of pace data by split. So, e.g., in 2019 the median pace of finishers on the start-to-12.6-mile split was 10:37.

A few features stand out to me.
* First, outside of 2024 having a large number of fast outliers, there's not much year-to-year variation.
* Second, as the race progresses the bulk of the pack slows down markedly if not substantially more than do the fastest runners.[^3] Take 2019 as an example. The median pace at 12.6 miles was 10:37; by 87.8 miles, it had slowed down by 6:19 (59.5%) to 16:56. By contrast, the lower-fence pace at 12.6 miles was 7:39; by 87.8 miles, it had slowed down only 3:45 (49%), to 11:24.

{% include graphs/split_paces_2019_2024.html %}

We can also look at splits from the angle of DNFs. Below, we chart out the overall DNF rate (top subplot) and the split-to-split DNF rate (bottom subplot) as a function of aid station. The observant reader will notice that the DNF rate does not [decrease monotonically](https://mathworld.wolfram.com/MonotoneDecreasing.html), which is a result of dirty data, discussed in the next section.

The bottom subplot shows the number of runners who DNF'd between two aid stations as a percentage of the number of runners still active at the preceding aid station. E.g., in 2019 nearly 20% of the runners who were still active at 56.5 miles had DNF'd by the time they came into mile 62.5. While I would have expected this chart to have less year-to-year variation, it's at least not surprising to see that the highest split-to-split DNF rates occur at miles 43.5, 50, 56.5, and 62.5—i.e., in the stretch of trail 7 miles before and 12 miles after Hope Pass.

{% include graphs/dnfs_finishers_drop_by_split.html %}

Finally, we can take a closer look at what happens on the trail by examining how often runners change ranks, i.e., pass each other. The table below examines finisher-only split-to-split rank differences from 2019 through 2024. As column four indicates, north of 90% of runners are passing someone at some point _each and every split_. In general, the movement isn't large, with runner ranks changing on average between 9 and 23 places. Perhaps somewhat surprisingly, there is substantial movement in ranks all the way up through the final split.[^4]

{% include rank_table.html %}

<!-- <h4 id="data-split-prediction">Split prediction</h4> -->

<h3 id="sources-processing" class="header-with-top">Data sources and processing
<a href="#top" class="go-to-top">Go to top</a>
</h3>

All data is derived from [Athlinks](https://www.athlinks.com/event/33913). Surprisingly, the source data is quite dirty. A non-exhaustive list of issues includes:
* Some runners have age = 0
* Some finishing times are under 13 hours but attached to runners who are marked as having finished rather than DNF'd
* Within a single year and filtering to just finishers, there are aid stations later on in the race that have more runners than some aid stations earlier on in the race

Additionally, DNF'd runners who finish after the cut-off time do not appear in the data at all. This is annoying and unfortunate, but the effect on the data in most if not all of the charts above is likely negligible.

A more comprehensive approach would combine the data on Athlinks (2017-2024; 1999-2001) with data from the Leadville Race Series website (1983-1986; 2002-2011), ultrarunning.com (1987-1998), raceresult.com (2012-2013), and chronotrack.com (2014-2016). While creating a centralized and standardized repository of this sort is a worthy goal, doing so requires more time than I have. Given the scale of the Leadville Race Series, however, I am a little surprised at just how disorganized data from the event is.

<h3 id="footnotes" class="header-with-top">Footnotes
<a href="#top" class="go-to-top">Go to top</a>
</h3>

[^1]: We're limited to looking at _finishers_ rather than _entrants_ because Athlinks does not have split data prior to 2017, meaning that all we get for 1983 to 2016 is a list of _finishers_.
[^2]: Technically splits data goes back to 2017, but 2017 and 2018 data is messy, so I've chosen to exclude it from these views.
[^3]: This assumes—I think reasonably—that whatever passing goes on does not materially affect where a runner is relative to the rest of the pack. E.g., this assumes that the runners we identified as fast and median at 12.8 miles are roughly still near the lower fence and the median at mile 87.8.
[^4]: There is undoubtedly some noise in these figures—e.g., I find it unlikely that someone jumped 351 places—but they should be correct directionally.