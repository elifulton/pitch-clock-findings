# pitch-clock-findings

# Overview

I thought that the pitch clock might cause pitchers to perform worse overall, and that this would be signified by a positive change in FIP (Fielding Independent Pitching). 2023 pitchers had higher FIPs on average, but this couldn't be significantly linked to the pitch clock.

# Context

The MLB pitch clock was introduced starting this past season, leaving pitchers with 15 seconds between pitches with no runners on base and 20 seconds *with* runners on. Fielding Independent Pitching is a metric on the same scale as ERA, but which only accounts for walks, strikeouts, and homeruns (the "three true outcomes", or the ones which pitchers most directly influence), so if the pitch clock affected overall pitching performance, I thought it would be reflected in this statistic.

# Results

To start, I uploaded data from FanGraphs and made functions to filter the columns of the tables. As a first test I checked the percentage of of all pitches thrown (among pitches from the past 10 years with 50 IP or more before the All-Star Break) that were called as balls, and found that this percentage trended down over time. Then I made normalized bell curves of the FIP difference year-to-year for the past 10 years, with the same pitchers (this is the first image below; the most recent year-to-year difference, 2022-23, had its curve highlighted in red). I made these bell curves into more detailed bar graphs to show the distribution more specifically (the one for 2022-23 is the second image shown below). After this, I checked the correlation between FIP difference and pitcher pitch clock violations in 2023. There was a slight negative correlation, but the p-value was too large to deem it statistically significant. The same thing happened when I tried to correlate the year-to-year difference (in seconds) in time taken between pitches with FIP difference (data for time between pitches was taken from Baseball Savant).

<img width="579" alt="Screenshot 2023-09-17 at 9 38 08 PM" src="https://github.com/elifulton/pitch-clock-findings/assets/4471336/cdf4e3c1-d772-49de-bebb-c16dcb084e41">

<img width="568" alt="Screenshot 2023-09-17 at 9 38 18 PM" src="https://github.com/elifulton/pitch-clock-findings/assets/4471336/ca7250e7-ce59-4bf7-b50e-ac0d5b9dac7d">

# Next Steps

Since no significant changes were shown in FIP, the next step might be to look at exact pitch location. Given that they have less time to command their pitches the way they want them, pitchers might throw more or less to certain parts of the strike zone.
