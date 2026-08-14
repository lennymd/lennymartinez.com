+++
date = '2018-08-01'
draft = true
title = 'Prosecuting Hate Crimes'
description = 'Building a dataset of federal hate crime prosecutions from DOJ press releases'
headImage = "img/projects/news21/[FILENAME].png"
headImageAlt = "[DESCRIBE THE IMAGE]"
+++

Since the Matthew Shepard and James Byrd, Jr. Hate Crimes Prevention Act passed in 2009, there has been no single public record of which federal crimes were actually prosecuted under it. I built one by applying natural language processing to Department of Justice press releases, identifying and classifying every federal prosecution brought under the various hate crime statutes. [ONE SENTENCE ON WHAT THE FINISHED DATASET COVERED — how many prosecutions, what date range, what fields.]

## Method

1. **Collection.** [How you obtained the DOJ press releases — scraped, bulk
   download, API. How many documents, covering what date range.]
2. **Filtering.** [How you narrowed the corpus to hate crime prosecutions.
   What the classifier or rules looked for, and what stack you used.]
3. **Extraction.** [What you pulled from each release — defendant, statute,
   district, charge, outcome — and how.]
4. **Statute matching.** [How you determined which hate crime law applied to
   each prosecution.]
5. **Validation.** [How you checked the output. Sample size, error rate, what
   the pipeline got wrong and how you corrected it.]

[CLOSING SENTENCE — what the finished dataset let the newsroom do that it
couldn't do before. This is the payoff; don't skip it.]

The analysis was produced during my fellowship with [Carnegie-Knight
News21](https://news21.com/about/), a national reporting initiative
headquartered at Arizona State University's Walter Cronkite School of
Journalism and Mass Communication. Findings from this work supported reporting
across the newsroom's _Hate in America_ investigation.

### Stories supported by this analysis

- [Millions are victims of hate crimes, though many never report them](https://hateinamerica.news21.com/millions-victims-of-hate-crimes/)
- [Black Americans still are victims of hate crimes more than any other group](https://hateinamerica.news21.com/black-americans-hate-crime-victims-more-than-any-group/)
- [As intolerance grows, targeted religious groups join forces](https://hateinamerica.news21.com/intolerance-grows-targeted-religious-groups-join-forces/)
- [Lack of trust in law enforcement hinders reporting of LGBTQ crimes](https://hateinamerica.news21.com/lack-of-trust-in-law-enforcement-hinders-reporting-LGBTQ-crimes/)
- [Police trained in hate crimes are key to convictions](https://hateinamerica.news21.com/police-trained-in-hate-crimes-key-to-convictions/)

---

OLD DRAFT BELOW

_Carnegie-Knight News21 is a national reporting initiative, headquartered at Arizona State University’s Walter Cronkite School of Journalism and Mass Communication, which brings top journalism students from across the country to report and produce in-depth, multimedia projects for major media outlets, such as The Washington Post, NBC News and USA Today. ([News21](https://news21.com/about/))_

## Data journalism

As part of my time as a News21 Fellow, I investigated the occurrences and prosecution of hate crimes since the passing of the Matthew Shepard and James Byrd, Jr. Hate Crimes Prevention Act (2009). This work involved using NLP techniques to identify and process press releases from the Department of Justice to determine all federal crimes prosecuted under the various hate crime laws. Findings from this analysis supported the reporting of other stories. **More process insights to come**

### Stories supported by analysis

- [Millions are victims of hate crimes, though many never report them](https://hateinamerica.news21.com/millions-victims-of-hate-crimes/)
- [Black Americans still are victims of hate crimes more than any other group](https://hateinamerica.news21.com/black-americans-hate-crime-victims-more-than-any-group/)
- [As intolerance grows, targeted religious groups join forces](https://hateinamerica.news21.com/intolerance-grows-targeted-religious-groups-join-forces/)
- [Lack of trust in law enforcement hinders reporting of LGBTQ crimes](https://hateinamerica.news21.com/lack-of-trust-in-law-enforcement-hinders-reporting-LGBTQ-crimes/)
- [Police trained in hate crimes are key to convictions](https://hateinamerica.news21.com/police-trained-in-hate-crimes-key-to-convictions/)

## State of Hate

As part of my time as a News21 Fellow, I traveled across the US to meet citizens and understand the tensions brought by the Trump Administration's stance on immigrants. For this project, I worked as a photojournalist. On the road, I photographed and interviewed individuals in Spanish and English, and contributed to the team's blog. At the end of the trip, I produced an interactive story highlighting our findings.

{{< button href="https://hateinamerica.news21.com/roadtrip/" label="Visit live project" >}}

### The State of Hate blog posts

- [The State of Hate: News21 is crossing the country](https://hateinamerica.news21.com/blog/2018/06/26/the-state-of-hate-news21-is-crossing-the-country/)
- [Fear of the unknown](https://hateinamerica.news21.com/blog/2018/06/28/the-state-of-hate-fear-of-the-unknown/)
- [In Marine Corps town, respect for others is respected](https://hateinamerica.news21.com/blog/2018/06/29/the-state-of-hate-in-marine-corps-town-respect-for-others-is-respected/)
- [‘America was pretty cool for a while’](https://hateinamerica.news21.com/blog/2018/07/02/the-state-of-hate-america-was-pretty-cool-for-a-while/)
- [‘You don’t see all the anger you see on the news’](https://hateinamerica.news21.com/blog/2018/07/05/the-state-of-hate-you-dont-see-all-the-anger-you-see-on-the-news-out-west/)
- [Rushmore inspires American unity in a divided time](https://hateinamerica.news21.com/blog/2018/07/07/the-state-of-hate-rushmore-inspires-american-unity-in-a-divided-time/)
- [The divide is about the jobs, not race](https://hateinamerica.news21.com/blog/2018/07/10/the-state-of-hate-the-divide-is-about-the-jobs-not-race/)
- [Americans still march to July 4th tunes](https://hateinamerica.news21.com/blog/2018/07/12/the-state-of-hate-americans-still-march-to-july-4th-tunes/)
- [Americans still long to get along](https://hateinamerica.news21.com/blog/2018/07/12/state-of-hate-americans-still-long-to-get-along-news21/)
- [‘We Bleed the Same Way’](https://hateinamerica.news21.com/blog/2018/07/16/the-state-of-hate-we-bleed-the-same-way/)
- [Kentuckians talk freedom, free speech](https://hateinamerica.news21.com/blog/2018/07/20/the-state-of-hate-kentuckians-talk-freedom-free-speech/)
- [Oklahomans satisfied with current times](https://hateinamerica.news21.com/blog/2018/07/31/the-state-of-hate-oklahomans-satisfied-with-current-times/)

### Other images

![Screenshot of the State of Hate interface](img/projects/news21/state-of-hate-2.png)
![Screenshot of the Evidence Map interface](img/projects/news21/state-of-hate-3.png)
![Screenshot of the Evidence Map interface](img/projects/news21/state-of-hate-4.png)
