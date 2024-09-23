---
layout: page
---

<h2 style="text-align: center;">Some data from the LT100</h2>

<div style="text-align: center;">

<span style="color: dark-gray; font-size: 14px">**Nikita Bogdanov**</span>

<span style="color: gray; font-size: 12px">_First published: 9/21/24_ &nbsp; &#124; &nbsp; _Last updated: 9/23/24_</span>

</div>

<hr style="margin-bottom: 15px; border: 0.5px solid gainsboro;">

1. [Preamble](#preamble)
2. [Course profile](#course)
3. [Data](#data)
    * [The basics](#data-basics)
    * [Cumulative percentages](#data-cumulative-percentages)
    * [Age, gender, time](#data-age-gender-time)
    * [Splits and pace](#data-splits)
    <!-- * [Split prediction](#data-split-prediction) -->
4. [Data sourcing and processing](#sources-processing)
5. [Other LT100 data projects](#other-projects)
6. [Footnotes](#footnotes)

<em>Note: If you'd like to reference the course as you read along, you can find an <a href="https://caltopo.com/m/DJ1HV" target="_blank">interactive version</a> on CalTopo, or a basic course profile [down below](#course).</em>


<h3 id="preamble" class="header-seps">Preamble</h3>
I spent the summer of 2016—and 2017, 2018, and 2019—in Leadville, CO, working as an instructor at the Colorado Outward Bound School. It was then that I first learned of the Leadville Trail 100. By the time I started at COBS, the organization had been running the Outward Bound aid station at the LT100 for a number of years and drew heavily from its ranks to staff the aid station and stock a pool of volunteer pacers. Having spent all summer working in the mountains, I figured I was up to the challenge of pacing; that first year I accompanied a runner from Outward Bound to Mayqueen. The experience was incredible, and in 2017 I was lucky enough to pace a runner from Outward Bound all the way to the finish. 

![Me, left, and the runner I paced, right, posing at the finish line.]({{"images/lt100_2017.jpg" | relative_url }})

While my course schedule didn't align with the race in 2018 and 2019, somewhere along the way I decided that I would one day run the LT100 myself. Until recently, this was a goal without much conviction behind it: in 2018 we moved from Colorado to New York City, and with the change of scenery it was challenging to hold on to the self I had grown into while living and working in the mountains.

...until David Roche [set the course record at this year's LT100](https://stories.strava.com/articles/david-roche-the-journey-to-the-leadville-100-course-record). I'm still many years away from running in the LT100 myself, but with David's record-setting debut—and a family commitment to moving back to the Mountain West in the not-too-distant future—I wanted to reconnect with my own experiences with the race and to start taking seriously that one day it will hopefully be me coming through the Outward Bound aid station. And so I did what I'm reasonably good at doing: I pulled some historical data and played around with making some graphs.

To be clear, this data falls pretty solidly into the category that I call "data porn"—data that's interesting to look at but that is ultimately of little or no practical utility and from which you can't draw (m)any statistically robust conclusions. Indeed, there are plenty of websites, blogs, and Reddit threads devoted to the topic of strategizing for ultras generally and the LT100 specifically, and those looking for practical advice should most certainly turn to sources such as those. The purely curious, however, can go some way toward scratching their data itch here.

<h3 id="course" class="header-with-top">Course profile
<a href="#top" class="go-to-top">Go to top</a>
</h3>

For those interested, this profile is derived from the course in the above-linked CalTopo map, which in turn is from the Leadville Race Series website (I believe).

![Course profile, with aid stations.]({{"images/course_profile.png" | relative_url }})

<h3 id="data" class="header-with-top">Data
<a href="#top" class="go-to-top">Go to top</a>
</h3>

Below, I've put together a collection of data cuts that I think are interesting and that I hope others find reasonably interesting as well. That said, if you'd like to see a cut that I haven't looked at, let me know and I'll see if: 1) the data structure will support it; and 2) I have the time to do it. Feel free to let me know, too, if you see anything wrong, confusing, or otherwise worth taking another look at. My contact information is below, in the footer.

<h4 id="data-basics">The Basics</h4>

The Leadville Trail 100 started in 1983 with 10 finishers; in 2024, it had just over 400.[^1] That's a 40x increase in finishers in roughly as many years—and assuming the DNF rate has remained approximately constant, which I think is likely, ditto for the number of entrants. But the race's growth trajectory has been far from steady, with just two periods of rapid growth: 1) 1987 and 1988, which brought participation to levels that lasted through 2008; and 2) 2009 and 2010, which brought participation to modern-day levels. What happened in 2009 and 2010? These years follow on the heels of the financial crisis, so it's possible that recently unemployed bankers took up ultra running; much more salient, however, is that on May 5th, 2009, Christopher McDougall published _Born to Run_.

![Finishers by year, showing a 40x increase from 1983 to 2024.]({{"images/finishers_by_year.png" | relative_url }})

On their [SWAP Podcast](https://podcasts.apple.com/us/podcast/some-work-all-play/id1521532868), David and Megan Roche often say that we're in the middle of a performance revolution in endurance sports, with top times getting faster across a variety of events. Without saying anything about causation—because there are too many confounding variables to list—it's anecdotally interesting that we see this phenomenon in the LT100, but only among top finishers. For most everyone else, even the top 25th percentile, finishing times have remained roughly flat across the years.

![Top times and P25, P50, and P75 finishing times from 1983 to 2024.]({{"images/percentiles_by_year.png" | relative_url }})

<h4 id="data-cumulative-percentages">Cumulative percentages</h4>

The vast majority of DNFs take place prior to the 18-hour mark, meaning that by the time the first runner crosses the finish line, the roster of finishers-to-be is more or less set. Roughly, and all else being equal, if you make it past hour 18, odds are that you're not going to DNF.

![Cumulative percentage of runners—finishers and DNFs—by time on course, 2024.]({{"images/cumulative_all_runners_2024.png" | relative_url }})

Zooming into just those who finished the race, we can see that the median finishing time in 2024 was just north of 28:00. By the 24-hour mark, only about 15% of finishers had come through.

![Cumulative percentage of runners—finishers only—by time on course, 2024.]({{"images/cumulative_finishers_only_2024.png" | relative_url }})

The percentages vary slightly from year to year, but as a whole the shapes of both curves—all runners and finishers only—are surprisingly durable.

![Cumulative percentage of runners—finishers and DNFs—by time on course, 2017-2024.]({{"images/cumulative_all_runners_2017_2024.png" | relative_url }})

What's especially stunning in the chart below is the durability of the inflection point around the 25-hour mark. The rate at which runners cross the finish line in the few hours before the 25-hour mark is qualitatively quite different than the rate at which runners cross the finish line in the few hours after the 25-hour mark. For one reason or another, if you're not finishing ahead of the 25-hour mark, you're finishing (at least) a few hours after it.

![Cumulative percentage of runners—finishers only—by time on course, 2017-2024.]({{"images/cumulative_finishers_only_2017_2024.png" | relative_url }})

<h4 id="data-age-gender-time">Age, gender, and time</h4>

Outside of the observation that older runners tend to be slower, there's not much of interest when we break down finishing times by age and gender. But, this graph does reinforce the oddity I pointed out just above, about the 25-hour mark being a sort of inflection point. Here, the inflection manifests as a decrease in "dot density" in the band between 25:00 and 26:00.

![Finishing time by age, colored by gender, from 1983 through 2024.]({{"images/finishing_time_age_gender.png" | relative_url }})

<h4 id="data-splits">Splits and pace</h4>
For 2019 through 2024, we can also look at performance within splits—i.e., in between aid stations.[^2] Here, we're looking at [box and whisker plots](https://datavizcatalogue.com/methods/box_plot.html) of pace data by split.[^3] So, e.g., in 2019 the median pace of finishers on the start-to-12.6-mile split was 10:37.

A few features stand out to me.
* First, there's not much year-to-year variation in either the overall shape or the spreads of individual splits.
* Second, Hope Pass is brutal in both directions, but more so on the way out than on the way back. How so? Runners consistently move slowest on the portion of trail from mile 38 or so to mile 43.5, which corresponds to the outbound uphill portion of Hope Pass; the stretch from mile 50 to mile 56.6, where runners head up the backside of the pass, has the second-slowest pace.
* Third, uphills bring out performance differences. The interquartile range (IQR) of the four splits leading up to Hope Pass hovers between 2 and 2:30. I've heard Leadville described as a road race for the first 40 miles, and this data goes some way towards supporting that characterization. Once runners begin to ascend, however, the IQR widens to nearly 5:00 and we see the spread increase as well between the Q3 and the upper fence and Q1 and the lower fence.
* Fourth, we can see Hope Pass reflected in every split that follows. The IQR of the last four splits, which runners hit once they descend Hope Pass, hovers around 3:00, a 25% to 50% increase compared to the IQR of the first four splits.

{% include graphs/split_paces_2019_2024.html %}

The companion view to split paces is a view of how the cumulative pace evolves over time. What's notable here is that as the race progresses the bulk of the pack slows down markedly if not substantially more than do the fastest runners.[^4] Take 2019 as an example. The median pace in the first 12.6 miles was 10:37; across 87.8 miles, it had slowed down by 6:19 (59.5%) to 16:56. By contrast, the lower-fence pace in the first 12.6 miles was 7:39; across 87.8 miles, it had slowed down only 3:45 (49%), to 11:24.

{% include graphs/cumulating_paces_2019_2024.html %}

We can also look at splits from the angle of DNFs. Below, we chart out the overall DNF rate (top subplot) and the split-to-split DNF rate (bottom subplot) as a function of aid station. The observant reader will notice that the DNF rate does not [decrease monotonically](https://mathworld.wolfram.com/MonotoneDecreasing.html), which is a result of dirty data, discussed in the next section.

The bottom subplot shows the number of runners who DNF'd between aid station A and B as a percentage of the number of runners still active at aid station A. E.g., in 2019 nearly 20% of the runners who were still active at 56.5 miles had DNF'd by the time they came into mile 62.5. While I would have expected this chart to have less year-to-year variation, it's at least not surprising to see that the highest split-to-split DNF rates occur at miles 43.5, 50, 56.5, and 62.5—i.e., in the stretch of trail 7 miles before and 12 miles after the half-way turnaround and Hope Pass.

{% include graphs/dnfs_finishers_drop_by_split.html %}

Finally, we can take a closer look at what happens on the trail by examining how often runners change ranks, i.e., pass each other. The table below examines finisher-only split-to-split rank differences from 2019 through 2024. As column four indicates, north of 90% of runners are passing someone or being passed _each and every split_. In general, the movement isn't large, with runner ranks changing on average between 9 and 23 places. Perhaps somewhat surprisingly, there is substantial movement in ranks all the way up through the final split.[^5] (Note that on small screens the table scrolls.)

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

<h3 id="other-projects" class="header-with-top">Other LT100 data projects
<a href="#top" class="go-to-top">Go to top</a>
</h3>

A quick Google search shows a few similar projects, linked below. If you know of any others, feel free to reach out; my contact information is in the footer.
* <a href="https://lt100analysis.com/" target="_blank">https://lt100analysis.com/</a>
* <a href="https://www.mitchleblanc.com/2012/09/leadville-100-2012-race-report-part-3-data-analysis/" target="_blank">https://www.mitchleblanc.com/</a>

<h3 id="footnotes" class="header-with-top">Footnotes
<a href="#top" class="go-to-top">Go to top</a>
</h3>

[^1]: We're limited to looking at _finishers_ rather than _entrants_ because Athlinks does not have split data prior to 2017—since outside of 1999 to 2021, Athlinks was not the time keeper for the race. This means that all we get for 1983 to 2016 is a list of finishers.
[^2]: Technically splits data goes back to 2017, but 2017 and 2018 data is messy, so I've chosen to exclude it from these views.
[^3]: The lower and upper fences are positioned at +/- 1.5x the interquartile range (75th percentile - 25 percentile).
[^4]: This assumes—I think reasonably—that whatever passing goes on does not materially affect where a runner is relative to the rest of the pack. E.g., this assumes that the runners we identified as fast and median at 12.8 miles are roughly still near the lower fence and the median at mile 87.8.
[^5]: There is undoubtedly some noise in these figures—e.g., I find it unlikely that someone jumped 351 places—but they should be correct at least directionally.