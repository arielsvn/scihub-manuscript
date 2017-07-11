# Sci-Hub provides access to nearly all scholarly literature

## Authors


+ **Daniel S. Himmelstein**<br>
  [\@dhimmel](https://github.com/dhimmel) ·
  [0000-0002-3012-7446](https://orcid.org/0000-0002-3012-7446) ·
  Department of Systems Pharmacology and Translational Therapeutics, University of Pennsylvania ·
  Funded by GBMF4552




## Abstract

The website Sci-Hub provides access to scholarly literature via full text PDF downloads.
The site enables users to access articles that would otherwise be paywalled.
Since its creation in 2011, Sci-Hub has grown rapidly in popularity.
However, until now, the extent of Sci-Hub's coverage was unclear.
As of March 2017, we find that Sci-Hub's database contains 68.9% of all 81.6 million scholarly articles, which rises to 85.2% for those published in closed access journals.
Furthermore, Sci-Hub contains 77.0% of the 5.2 million articles published by inactive journals.
Coverage varies by discipline, with 92.8% coverage of articles in chemistry journals compared to 76.3% for computer science.
Coverage also varies by publisher, with the coverage of the largest publisher, Elsevier, at 97.3%.
Our interactive browser at [greenelab.github.io/scihub](https://greenelab.github.io/scihub) allows users to explore these findings in more detail.
Finally, we estimate that over a six month period in 2015–2016, Sci-Hub provided access for 99.3% of valid incoming requests.
Hence, the scope of this resource suggests the subscription publishing model is becoming unsustainable.
For the first time, the overwhelming majority of scholarly literature is available gratis to anyone.

## Introduction

As of 2014, paywalls on the web limited access to an estimated 76% of scholarly literature [@MNHagzoO].
The open access movement strives to increase the accessibility of scholarly literature [@PuP45jrB].
After decades of effort by the open access community [@3k6GM8o4], nearly 50% of newly published articles are available without paywalls [@n1xo9kJ7; @NE5AByb0].
Literature that is free to read is comprised of two categories [@tSEdUvgK].
The first category includes articles that are articles are [openly licensed](http://opendefinition.org/) to freely allow reuse, a group colloquially termed "free as in libre".
The remainder of free to read articles can be accessed without price barriers, but permission barriers may remain (usually due to copyright) [@7aXVorCC]. This set of articles is termed "free as in gratis".
In this work, we refer to availability as "libre" or "gratis" to denote these categories.

The website Sci-Hub, now in its fifth year of existence provides gratis access to scholarly literature, despite the continued presence of paywalls.
Sci-Hub brands itself as "the first pirate website in the world to provide mass and public access to tens of millions of research papers."
The website, started in 2011, is run by Alexandra Elbakyan, a neuroscientist and native of Kazakhstan who now resides in Russia [@JVjciZPv; @sR4uAYxB].
Elbakyan describes herself as motivated to provide universal access to knowledge [@nZZjs6T6; @1BUarVNFD; @K6n65WB0].

Sci-Hub does not restrict itself to only openly licensed content.
Instead, it retrieves and distributes scholarly literature without regard to copyright regimes.
**Readers should note that, in many jurisdictions, use of Sci-Hub may constitute copyright infringement.
Users of Sci-Hub do so at their own risk.
This study is not an endorsement of using Sci-Hub, and its authors and publishers accept no responsibility on behalf of readers.
It is a strong possibility that Sci-Hub users — especially those not using privacy-protecting services such as Tor — could have their usage history unmasked and face consequences, both legal or reputational in nature.**

Sci-Hub is currently served at the domains `sci-hub.cc`, `sci-hub.io`, and `scihub22266oqcxt.onion` (a Tor Hidden Service [@zvVsLNxf]).
Elbakyan recently described the project's technical scope [@1H8x8f4Y7]:

> Sci-Hub technically is by itself a repository, or a library if you like, and not a search engine for some other repository.
But of course, the most important part in Sci-Hub is not a repository, but the script that can download papers closed behind paywalls.

One method Sci-Hub uses to bypass paywalls is by obtaining leaked authentication credentials for educational institutions [@1H8x8f4Y7].
These credentials enable Sci-Hub to use institutional networks as proxies and gain subscription journal access.
While the open access movement has progressed slowly, Sci-Hub represents a seismic shift in access to scholarly literature.
Since its inception, Sci-Hub has experienced sustained growth, with spikes in interest and awareness driven by legal proceedings, news coverage, and social media (Figure 1).
Here we investigate the extent to which Sci-Hub provides access to scholarly literature.
If the coverage of Sci-Hub is widespread, then a radical and rapid shift is likely underway in how individuals access scholarly literature.

![Google Trends Search interest for Sci-Hub and LibGen](https://cdn.rawgit.com/greenelab/scihub/7891082161dbcfcd5eeb1d7b76ee99ab44b95064/explore/trends/google-trends.svg)

**Figure 1: The history of Sci-Hub.**
Weekly interest from Google Trends is plotted over time for the search terms "Sci-Hub" and "LibGen".
The light green period indicates when Sci-Hub used LibGen as its database for storing articles [@1H8x8f4Y7].
The light blue period indicates the public availability of Sci-Hub request logs [@kQFQ8EaO].
The first pink dotted line represents the collection date of the LibGen metadata used in Cabanac's study [@18KKRwlN6].
The second pink dotted line shows the date of Sci-Hub's Tweeted DOI catalog used in this study.
The ⓛⓔⓣⓣⓔⓡⓢ refer to the following events:

+ **Ⓐ** Created by Alexandra Elbakyan, the Sci-Hub website goes live on September 5, 2011.
+ **Ⓑ** Certain LibGen domains go down, allegedly due to the death of a contributor [@Hz2uRUJS].
+ **Ⓒ** Elsevier files a complaint against Sci-Hub and LibGen — at the respective domains `sci-hub.org` and `libgen.org` — in the New York Southern District Court [@6ZrZVv6E; @j3Zl6sH5].
The complaint seeks a "prayer for relief" that includes domain names seizure, damages, and "an order disgorging Defendants' profits."
+ **Ⓓ** Elsevier is granted a preliminary injunction to suspend domain names and restrain the site operators from distributing Elsevier's copyrighted works [@9GOM6WEw; @BpCqwlYS].
Shortly after, Sci-Hub and LibGen resurface at alternative domains outside of U.S. court jurisdiction including on the dark web [@16k28dBmH; @sR4uAYxB].
+ **Ⓔ** The article "Meet the Robin Hood of Science" by Simon Oxenham generates an unprecedented amount of attention and news coverage of Sci-Hub and Alexandra Elbakyan [@SlcfPQQQ], culminating in the _New York Times_ asking "Should all research papers be free?" [@tMPCGeuL].
+ **Ⓕ** The article "Who's downloading pirated papers? Everyone" by John Bohannon shows widespread, global usage of Sci-Hub [@RsNXQAG2; @t4r48QpO].
These findings spark debate amongst scholars, with a large contingent of scientists supporting Sci-Hub's mission [@Zp0s36X0; @cOKy7PSo].
+ **Ⓖ** Alexandra Elbakyan is named one of "_Nature_'s 10", which featured "ten people who mattered" in 2016 [@cUfIvWm6].
Written by Richard Van Noorden, the story profiles Alexandra and includes an estimate that Sci-Hub serves "3% of all downloads from science publishers worldwide".
+ **Ⓗ** The court finds that Alexandra Elbakyan, Sci-Hub, and LibGen are "liable for willful copyright infringement" in a default judgment, since none of the defendants answered Elsevier's complaint [@b5B01CbS; @jlNm94FU; @17drH57zs].
The court makes the injunction permanent and orders the defendants to pay Elsevier $15 million — $150,000 for each of 100 copyrighted works.
The statutory damages, which the defendants do not intend to pay, now bear interest.
+ **Ⓘ** The American Chemical Society files suit against Sci-Hub in the Eastern District of Virginia.
Their prayer for relief requests that Internet search engines and Internet service providers "cease facilitating access" to Sci-Hub [@17REO8hrA; @POar53EX].

Past research sheds some light on Sci-Hub's reach.
From the Spring of 2013 till the end of 2014, Sci-Hub relied the Library Genesis (LibGen) scimag database to store articles [@1H8x8f4Y7].
Whenever a user requested an article, Sci-Hub would check LibGen for a copy.
If the article was not in LibGen, Sci-Hub would fetch the article for the user and also upload it to LibGen.
Cabanac compared the number of articles in the LibGen scimag database at the start of 2014 to the total number of Crossref DOIs.
Accordingly, he estimated LibGen contained 36% of all scholarly articles [@18KKRwlN6].
Coverage was higher for several prominent publishers: 77% for Elsevier, 73% for Wiley, and 53% for Springer (prior to its merger with Macmillan / Nature [@ynhlmOBH]).

Later, Bohannon analyzed six months of Sci-Hub's server request logs starting in September 2015 [@RsNXQAG2].
He found a global pattern of usage.
Based on these logs, Gardner, McLaughlin, and Asher estimated the ratio of publisher to Sci-Hub downloads for several journals [@17rORqxsI].
They estimated this ratio at 20:1 for the Royal Society of Chemistry and 48:1 for Elsevier.
Greshake also analyzed the logs to identify per capita Sci-Hub usage [@uBm4Sor6].
Portugal, Iran, Tunisia, and Greece had the highest usage, suggesting Sci-Hub is preferentially used in countries with poor institutional access to scholarly literature.
In a subsequent study, Greshake found especially high Sci-Hub usage in chemistry, with 12 of top 20 requested journals specializing in chemistry [@iLKgjFDu; @nnSxBFFr].

Since 2015, Sci-Hub has operated its own repository, distinct from LibGen.
On March 19, 2017, Sci-Hub released the list of DOIs for articles in its database.
Greshake retrieved metadata for 77% of Sci-Hub DOIs [@iLKgjFDu; @nnSxBFFr].
He found that 95% articles in Sci-Hub were published after 1950.
Sci-Hub requests were even more skewed towards recent articles with only 5% targeting articles published before 1983.
Greshake's study did not incorporate a catalog of all scholarly literature.
This study analyzes Sci-Hub's catalog in the context of all scholarly literature and thus assesses coverage.
In other words, what percent of articles in a given domain does Sci-Hub possess?

## Results

To define the extent of the scholarly literature, we relied on DOIs from the Crossref database, as downloaded on March 21, 2017.
We define the "scholarly literature" as 81,609,016 texts identified by their DOIs.
We refer to these texts as "articles", although a diverse compilation of text types are encompassed, including book chapters, front matters, and standards. To assess the articles available from Sci-Hub, we relied on a list of DOIs released by Sci-Hub on March 19, 2017.
All DOIs were lowercased to be congruent across datasets (see Methods).
Sci-Hub's offerings included 56,246,220 articles from the corpus of scholarly literature, equating to 68.9% of all articles.

### Coverage by article type

Each article in Crossref's database is assigned a type.
Figure 2 shows coverage by article type.
The scholarly literature consisted primarily of journal articles, for which Sci-Hub had 77.8% coverage.
Sci-Hub's coverage was also strong for the 5 million proceedings articles at 79.7%.
Overall coverage suffered from the 10 million book chapters where coverage was poor (14.2%).
The remaining Crossref types were uncommon, and hence contributed little to overall coverage.

![Sci-Hub coverage by Crossref type](https://cdn.rawgit.com/greenelab/scihub/7891082161dbcfcd5eeb1d7b76ee99ab44b95064/figure/coverage-by-type.svg)

**Figure 2: Coverage by article type.**
Coverage is plotted for the Crossref work types included by this study.
We refer to all of these types as "articles".

### Coverage by year

Next, we investigated coverage based on the year an article was published.
For most years since 1850, annual coverage is between 60–80%.
However, there's a dropoff in coverage, starting in 2010, for recently published articles.
For example, 2016 coverage was 56.0% and 2017 coverage (for part of the year) was 45.3%.
One factor is that it takes some time for Sci-Hub to retrieve articles following their publication, especially since many are not downloaded until requested by a user. 
Another factor could be that some journals are now deploying more aggressive anti-piracy measures [@xn59qVAG; @d9g1ZhPz], making recent articles less accessible.

![Sci-Hub coverage by year](https://cdn.rawgit.com/greenelab/scihub/7891082161dbcfcd5eeb1d7b76ee99ab44b95064/figure/coverage-by-year.svg)

**Figure 2: Coverage of articles by year published.**
Sci-Hub's article coverage is shows for each year since 1850.

### Coverage by journal

We defined a comprehensive set of scholarly publishing venues, referred to as "journals", based on the Scopus database.
In reality, these include conferences with proceedings as well as book series.
For inclusion in this analysis, each required an ISSN and at least one article as part of the Crossref-derived catalog of scholarly literature.
Accordingly, our catalog consisted of 22,193 journals encompassing 57,074,208 articles.
Of these journals, 4,345 were inactive (19.6%, i.e. no longer publishing articles), and 2,650 were open access (11.9%).
Only two journals were inactive and also open access.

We calculated Sci-Hub's coverage for each of the 22,193 journals (examples in Table 1).
The complete journal coverage results are available in our [Sci-Hub Stats Browser](https://greenelab.github.io/scihub/#/).

**Table 1: Coverage for the the ten journals with the most articles.**

| Journal | Sci-Hub | Crossref | Coverage |
|-------|--------|----------|----------|
| The Lancet | 457,650 | 458,580 | 99.80% |
| Nature | 385,619 | 399,273 | 96.58% |
| BMJ (Clinical research ed.) | 17,141 | 392,277 | 4.37% |
| Lecture Notes in Computer Science | 103,675 | 356,323 | 29.10% |
| Science | 230,649 | 251,083 | 91.86% |
| JAMA - Journal of the American Medical Association | 191,950 | 248,369 | 77.28% |
| Journal of the American Chemical Society | 189,142 | 189,567 | 99.78% |
| Scientific American | 22,600 | 186,473 | 12.12% |
| New England Journal of Medicine | 180,321 | 180,467 | 99.92% |
| PLoS ONE | 4,731 | 177,260 | 2.67% |

In general, a journal's coverage was either nearly complete or nearly entirely absent (Figure 4).
As a result, relatively few journals had coverage between 5–75%.
At the extremes, 2,342 journals had zero coverage, whereas 2,067 had perfect coverage.
Of zero-coverage journals, 22.3% were inactive, and 27.2% were open access.
Of perfect-coverage journals, 80.3% were inactive, and 1.9% were open access.
Hence, inactive closed-access journals make up the bulk of perfect-coverage journals.

![Sci-Hub journal/publisher coverage distributions](https://cdn.rawgit.com/greenelab/scihub/7891082161dbcfcd5eeb1d7b76ee99ab44b95064/figure/coverage-distributions.svg)

**Figure 4: the distributions of journal & publisher coverages.**
The histograms show the distribution of Sci-Hub's coverage for journals and publishers. 
Each bin spans 2.5 percentage points.

Next we explored article coverage according to journal attributes (Figure 5).
Sci-Hub covered 83.4% of the 57,074,208 articles that were attributable to a journal.
Articles from inactive journals had slightly lower coverage than active journals (77.0% versus 84.3%).
Strikingly, coverage was substantially higher for articles from closed- rather than open-access journals (85.2% versus 49.1%).
Coverage did vary by subject area, with the highest coverage in chemistry at 92.8% and the lowest coverage in computer science at 76.3%.
Accordingly, no disciplines had coverage below 75%. See Figure S1 for coverage according to a journal's country of publication.

![Sci-Hub coverage by journal attribute](https://cdn.rawgit.com/greenelab/scihub/7891082161dbcfcd5eeb1d7b76ee99ab44b95064/figure/coverage.svg)

**Figure 5: Coverage by journal attributes.**
Coverage was assessed for all articles from journals with the specified Scopus attributes.

We also evaluated whether journal coverage varied by journal impact.
We assessed journal impact using the 2015 CiteScore, which measures the average number of citations articles published in 2012–2014 received during 2015.
Highly-cited journals tended to have higher coverage in Sci-Hub (Figure 7A).
The 1,730 least cited journals (lowest decile) had 40.9% coverage on average, whereas the 1,729 most cited journals (top decile) averaged 90.3% coverage.

### Coverage by publisher

Next, we evaluated coverage by publisher (Figure 6, full table [online](https://greenelab.github.io/scihub/#/publishers)).
The largest publisher was Elsevier, with 13,185,971 articles from 3,356 journals.
Sci-Hub covered 97.3% of Elsevier articles.
For the eight publishers who reached the million article milestone, the following coverage was observed:
97.3% of Elsevier,
89.4% of Springer Nature,
94.8% of Wiley-Blackwell,
96.2% of Taylor & Francis,
79.2% of Wolters Kluwer,
98.8% of American Chemical Society,
95.3% of SAGE, and
84.9% of Oxford University Press.
In total, 4,879 publishers were represented in the journal catalog.
The coverage distribution amongst publishers resembled the journal coverage distribution, with most publishers occupying the extremities (Figure 4).
Sci-Hub had zero coverage for 1,206 publishers and complete coverage for 323 publishers.

![Sci-Hub coverage by publisher](https://cdn.rawgit.com/greenelab/scihub/7891082161dbcfcd5eeb1d7b76ee99ab44b95064/figure/coverage-by-publisher.svg)

**Figure 6: Coverage by publisher.**
Article coverage is shown for all Scopus publishers with at least 200,000 articles.

### Sci-Hub request logs

Sci-Hub released article request records from its server logs covering 165 days from September 2015 through February 2016 [@RsNXQAG2; @t4r48QpO; @kQFQ8EaO].
We filtered for valid requests by restricting to DOIs in our literature catalog and omitting requests that occurred before the article's publication date.
Accordingly, we identified 26,984,851 valid requests for 10,116,937 distinct articles.
Hence on average, Sci-Hub received approximately 164,000 valid requests per day in late 2014 / early 2015.

The logs do not indicate whether requests were fulfilled.
However, if a requested article wasn't in Sci-Hub's database, Sci-Hub would have attempted to retrieve it and store it for future use.
Therefore, we can estimate fulfillment rates by assuming that articles currently in Sci-Hub's database were available in the past, at the time of request.

Accordingly, we estimate that Sci-Hub fulfilled 99.3% of valid requests during this period.
The estimated fulfillment rates were nearly 100% for all article types besides book chapters.
Users that requested book chapters received access 82.1% of the time.
In total, only 141,466 articles were requested that are not presently in Sci-Hub.
Of these inaccessible articles, 14,154 [were](https://github.com/greenelab/scihub/issues/5#issuecomment-298952622) book chapters from _Lecture Notes in Computer Science_.

We computed journal-level metrics based on average article requests.
The "visitors" metric assesses the average number of IP addresses that requested each article published by a journal during the 20 months proceeding September 2015 (the log's start date).
In aggregate, articles from closed access journals average 1.30 visitors, whereas articles from open access journals averaged 0.27 visitors.
Figure 7B shows that articles from highly cited journals were on average much more frequently visited.
Articles in the least cited closed access journals averaged almost zero visitors compared to approximately 15 visitors for the most cited journals.
In addition, Figure 7B shows that Sci-Hub visitors are many times more frequent for articles in closed versus open access journals, even after accounting for journal impact.

![Sci-Hub Coverage & Visitors versus Journal's 2015 CiteScore](https://cdn.rawgit.com/greenelab/scihub/7891082161dbcfcd5eeb1d7b76ee99ab44b95064/figure/citescore.svg)

**Figure 7: Relation to journal impact.**
**A)**
Average coverage for journals divided into 2015 CiteScore deciles.
The CiteScore range defining each decile is shown by the x-axis labels.
The ticks represent 99% confidence intervals of the mean.
This is the only analysis where "Sci-Hub Coverage" refers to journal-level rather than article-level averages.
**B)**
The association between 2015 CiteScore and average visitors per article is plotted for open and closed access journals.
Curves show the 95% confidence band from a Generalized Additive Model.

## Discussion

Sci-Hub's database contains 69% of all scholarly literature.
Coverage for the 50 million articles attributed to closed access journals — where other routes to access may not exist — was 85.2%.
Furthermore, coverage of the most cited journals exceeded 90%.
Journals with very low (including zero) coverage tended to be obscure, less cited venues.
Importantly, Sci-Hub delivers access to scholarly literature at a much higher rate than its database coverage.
Since Sci-Hub can retrieve, in realtime, requested articles that are not in its database, our coverage figures are a lower bound.
In terms of articles actually requested by users, we infer that access is provided 99% of the time.

We find strong evidence that Sci-Hub is primarily used to circumvent paywalls.
Particularly, users requested articles from closed access journals much more frequently than open access journals.
Accordingly, many users likely only resort to Sci-Hub when access via the publisher is cumbersome or costly.

Judging from donations, many users seem to appreciate Sci-Hub's service.
In the past, Sci-Hub accepted donations through centralized and regulated payment processors, such as PayPal, Yandex, WebMoney, and QiQi [@j3Zl6sH5; @1EZBJN9ej].
Now however, Sci-Hub only advertises donation via bitcoin, presumably to avoid banking blockades or government seizure of funds.
Since the ledger of bitcoin transactions is public, we can evaluate the donation activity to known Sci-Hub addresses (`1K4t2vSBSS2xFjZ6PofYnbgZewjeqbG1TM`, `14ghuGKDAPdEcUQN4zuzGwBUrhQgACwAyA`, `1EVkHpdQ8VJQRpQ15hSRoohCztTvDMEepm`).
We find that these addresses have received 1,037 donations totaling 92.63 bitcoins (Figure 8, Figure S2).
Using the U.S. dollar value at the time of transaction confirmation, Sci-Hub has received an equivalent of $60,358 in bitcoins.
However, since the price of bitcoins has risen, the 67.42 donated bitcoins that remain unspent are now worth approximately $175,000.

![Number of bitcoin donations per month to Sci-Hub](https://cdn.rawgit.com/greenelab/scihub/7891082161dbcfcd5eeb1d7b76ee99ab44b95064/explore/bitcoin/monthly-donations-count.svg)

**Figure 8: Number of bitcoin donations per month.**
The number of bitcoin donations to Sci-Hub is shown for each month from June 2015 to June 2017.
Since February 2016, Sci-Hub has received at least 30 donations per month.
Each donation corresponds to an incoming transaction to a known Sci-Hub address.

The largest and most prominent publishers are highly covered by Sci-Hub.
Publishers have taken note.
Elsevier (whose 13 million works are 97.3% covered by Sci-Hub) and the American Chemical Society (whose 1.4 million works are 98.8% covered) have both filed suit against Sci-Hub, despite the limited enforcement options of United States courts.
The widespread gratis access to previously paywalled content calls into question the sustainability of the subscription publishing model.
As distributed and censorship-resistant file storage protocols mature [@16kozZ9Ys; @5gyFSQse], Sci-Hub alternatives may emerge that no longer rely on a centralized service. As such, Sci-Hub's corpus of gratis scholarly literature will be extremely difficult to suppress.

In addition, adoption of pirate sites may accelerate if Universities continue canceling journal subscriptions [@wnNilBvm; @uKvlPbm2], leaving researchers with few alternative access options.
We can also expect biblioleaks — bulk releases of closed access corpuses — to progress despite publisher's best efforts, as articles must only leak once to be perpetually available [@8mg1a0YE].
In essence, scholarly publishers have already lost the access battle.
Publishers will be forced to adapt quickly to open access publishing models.
In the words of Alexandra Elbakyan [@DCZkZXsz]:

> The effect of long-term operation of Sci-Hub will be that publishers change their publishing models to support Open Access, because closed access will make no sense anymore.

Sci-Hub is poised to fundamentally disrupt scholarly publishing.
The transition to gratis availability of scholarly articles is inevitable.
However, we urge the community to take this opportunity to fully liberate scholarly articles.
Only libre access, enabled by [open licensing](http://opendefinition.org/), allows building applications on top of scholarly literature without fear of legal consequences [@7aXVorCC].
Were all articles libre, there would be no such thing as a "pirate website" for accessing scholarly literature.

## Methods

This project was performed entirely in the open, via the GitHub repository [`greenelab/scihub`](https://github.com/greenelab/scihub).
Several authors of this study became involved after we mentioned their usernames in GitHub discussions.
This project's fully transparent and online model enabled us to assemble an international team of individuals with complementary expertise and knowledge.

We managed our computational environment using [Conda](https://conda.io/docs/), allowing us to specify and install dependencies for both Python and R.
The analyses were performed by a sequence of [Jupyter](http://jupyter.org/) notebooks.
In general, data integration and manipulation was performed in Python 3, relying heavily on [Pandas](https://pandas.pydata.org/), whereas plotting was performed with [ggplot2](http://ggplot2.org/) in R.
Tabular data was saved in TSV (Tab Separated Values) format and xz compressed when large.
We used Git Large File Storage ([Git LFS](https://git-lfs.github.com/)) to track large files, enabling us to make nearly all of the datasets generated and consumed by the analyses available.
The Sci-Hub Stats Browser is a single-page application built using React and hosted via GitHub Pages.

### Digital Object Identifiers

We used DOIs (Digital Object Identifiers) to uniquely identify articles.
LibGen scimag and Sci-Hub also uniquely identify articles by their DOIs, making DOIs the natural primary key for our analyses.
The DOI initiative began in 1997, and the first DOIs were registered in 2000 [@8zeVK2hX; @JDfJRWbr].
Note that DOIs can be registered retroactively.
For example, Antony van Leewenhoeck's discovery of protists and bacteria — published in 1677 by _Philosophical Transactions of the Royal Society of London_ [@HhEZiSSR] — has a DOI (`10.1098/rstl.1677.0003`).
While this article was published long before the DOI system existed, the _Royal Society_ retroactively assigned a DOI in 2006.

Not all scholarly articles have DOIs.
By evaluating the presence of DOIs in other databases of scholarly literature (such as PubMed, Web of Science, and Scopus), researchers estimate around 90% of newly published articles in the sciences have DOIs [@9sCtTvlE; @10zxQMO6J].
The prevalence of DOIs varies by discipline and country of publication, with DOI assignment in newly published Arts & Humanities articles around 60% [@9sCtTvlE].
Indeed, DOI registration is almost entirely lacking for publishers from many Eastern European countries [@10zxQMO6J].
In addition, the prevalence of DOI assignment is likely lower for older articles [@10zxQMO6J].
The incomplete and non-random assignment of DOIs to scholarly articles is a limitation of this study.
However, DOIs are presumably the least imperfect and most widespread identifier for scholarly articles. 

An often overlooked aspect of the DOI system is that DOIs are case-insensitive within the ASCII character range [@8zeVK2hX; @LS0mB1CD].
In other words, `10.7717/peerj.705` refers to the same article as `10.7717/PeerJ.705`.
Accordingly, DOIs make a poor standard identifier unless they're consistently cased.
While the DOI handbook states that "all DOI names are converted to upper case upon registration" [@8zeVK2hX], we lowercased DOIs in accordance with Crossref's behavior.
Given the danger of incongruous DOIs, we lowercased DOIs for each input resource at the earliest opportunity in its processing pipeline.
Consistent casing [considerably influenced](https://github.com/greenelab/scihub/issues/9) our findings as different resources used different casings of the same DOI.

### Crossref-derived catalog of scholarly articles

To catalog all scholarly articles, we relied on the Crossref database.
[Crossref](https://www.crossref.org/) is a DOI Registration Agency (an entity capable of assigning DOIs) for scholarly publishing [@Eq78IAX4].
There are presently 10 Registration Agencies.
We [estimate](https://github.com/greenelab/crossref/issues/3) that Crossref has registered 67% of all DOIs in existence.
While several Registration Agencies assign DOIs to scholarly content, Crossref is the preeminent registrar for scholarly publications.
In March 2015, of the 1,464,818 valid DOI links on the English Wikipedia, 99.9% were registered with Crossref [@aUCPtxQc].
This percentage was slightly lower for other languages — 99.8% on the Chinese Wikipedia and 98.0% on the Japanese Wikipedia.
Hence, the overwhelming majority of DOI-referenced scholarly articles are registered with Crossref.
Since Crossref has the most comprehensive and featureful programmatic access, there was a strong incentive to focus solely on Crossref-registered DOIs.
Given Crossref's preeminence, the omission of other Registration Agencies is unlikely to severely influence our findings. 

We queried the `works` endpoint of the [Crossref API](https://api.crossref.org/) to retrieve the metadata for all DOIs, storing the responses in a MongoDB database.
The queries began on March 21, 2017 and took 12 days to complete.
In total, we retrieved metadata for 87,542,370 DOIs corresponding to all Crossref works as of March 21, 2017.
The source code for this step is available on GitHub at [`greenelab/crossref`](https://github.com/greenelab/crossref).
Due to its large file size (7.4 GB), the MongoDB database export of DOI metadata is not available on GitHub and instead hosted via figshare [@1E6E4mpZ].
We created TSV files with the minimal information needed for this study.
First, a DOI table with columns for work type and date issued.
Date issued refers to the earliest known publication date, i.e. the date of print or online publication, whichever occurred first.
Second, a mapping of DOI to ISSN for associating articles with their journal of publication.

We [selected](https://github.com/greenelab/scihub/issues/7) a subset of Crossref work types to include in our Sci-Hub coverage analyses that corresponded to scholarly articles (i.e. publications).
Since we couldn't locate definitions for the Crossref types, we used our best judgment and evaluated sample works of a given type in the case of uncertainty.
We included the following types: `book-chapter`, `book-part`, `book-section`, `journal-article`, `proceedings-article`, `reference-entry`, `report`, and `standard`.
Types such as `book`, `journal`, `journal-issue`, and `report-series` were excluded since they're generally containers for individual articles rather than scholarly articles themselves.
After filtering by type, 81,609,016 DOIs remained (77,201,782 of which had their year of publication  available).
For the purposes of this study, these DOIs represent the entirety of the scholarly literature.

### Scopus-derived catalog of journals

Prior to June 2017, the Crossref API had an [issue](https://github.com/CrossRef/rest-api-doc/issues/179) that prevented exhaustively downloading journal metadata.
Therefore, we instead relied on the [Scopus](https://www.scopus.com) database to catalog scholarly journals.
Scopus uses "title" to refer to all of the following: peer-reviewed journals, trade journals, book series, and conference proceedings.
For this study, we refer to all of these types as journals.
From the January 2017 data release of Scopus titles, we extracted metadata for 62,482 titles including their name, ISSNs, subject areas, open access status, and active status.
Furthermore, we tidied the Scopus Journal Metrics, which evaluate journals based on the number of citations their articles receive.
Specifically, we extracted a 2015 CiteScore for 22,256 titles, 17,295 of which were included in our journal catalog.
Finally, we queried the Elsevier API to [retrieve](https://github.com/dhimmel/journalmetrics/issues/2) homepage URLs for 20,442 Scopus titles.
See [`dhimmel/journalmetrics`](https://github.com/dhimmel/journalmetrics) for the source code and data relating to Scopus.

### LibGen scimag's catalog of articles

Library Genesis (LibGen) is a shadow library of primarily pirated content.
Compared to Sci-Hub, the operations of LibGen are more opaque, as the contributors maintain a low profile and do not contact journalists [@1H8x8f4Y7].
LibGen consists of several collections, including distinct databases for scientific books / textbooks, fiction books, and comics [@18KKRwlN6].
In 2012, LibGen added the "scimag" database for scholarly literature.
Since the spring of 2013, Sci-Hub has uploaded articles that it obtains to LibGen scimag [@1H8x8f4Y7].
At the end of 2014, Sci-Hub forked LibGen scimag and began managing its own distinct article repository.

We downloaded the LibGen scimag metadata database from April 7, 2017 as a SQL dump.
We [imported](https://github.com/greenelab/scihub/issues/2) the SQL dump into MySQL, and then exported the scimag table to a TSV file.
Each row of this table corresponds to an article in LibGen, identified by its DOI.
The `TimeAdded` field indicates when the publication was uploaded to LibGen.
After removing records missing `TimeAdded`, 64,195,940 DOIs remained.
56,205,763 (87.6%) of the DOIs were in our Crossref-derived catalog of scholarly literature.
The 12.4% of LibGen scimag DOIs missing from our Crossref catalog, likely consist of incorrect DOIs, DOIs whose metadata availability postdates our Crossref export, DOIs from other Registration Agencies, and DOIs for excluded work types.

Next, we explored the cumulative size of LibGen scimag over time according to the `TimeAdded` field (Figure S3).
However, when we [compared](https://github.com/greenelab/scihub/issues/8#issuecomment-296710357) our plot to one generated from the LibGen scimag database SQL dump on January 5, 2014 [@18KKRwlN6], we noticed a major discrepancy.
The earlier analysis identified a total of 22,829,088 DOIs, whereas we found only 234,504 DOIs as of January 5, 2014.
We hypothesize that the discrepancy arose because `DateAdded` indicates the date modified rather than created.
Specifically, when an article in the database is changed, the database record for that DOI is entirely replaced.
Hence, the `DateAdded` value is effectively overwritten upon every update to a record.
Unfortunately, many research questions require the date first added.
For example, lag-time analyses (the time from study publication to LibGen upload) may be unreliable.
Therefore, we don't report on these findings in this manuscript.
Instead, we provide Figure S4 as an example analysis that would be highly informative were reliable creation dates available.
In addition, findings from some previous studies may need additional scrutiny.
For example, Cabanac writes [@18KKRwlN6]:

> The growth of LibGen suggests that it has benefited from a few isolated, but massive, additions of scientific articles to its cache.
For instance, 71% of the article collection was uploaded in 13 days at a rate of 100,000+ articles a day.
It is likely that such massive collections of articles result from biblioleaks [@8mg1a0YE], but one can only speculate about this because of the undocumented source of each file cached at LibGen.

While we agree this is most likely the case, confirmation is needed that the bulk addition of articles does not just correspond to bulk updates rather than bulk initial uploads.

### Sci-Hub's catalog of articles

On March 19, 2017, Sci-Hub [tweeted](https://twitter.com/Sci_Hub/status/843546352219017218):

> If you like the list of all DOI collected on Sci-Hub, here it is: `sci-hub.cc/downloads/doi.7z` … 62,835,101 DOI in alphabetical order

The Tweet included a download link for a file with the 62,835,101 DOIs that Sci-Hub claims to provide access to.
Of these DOIs, 56,246,220 were part of the Crossref-derived catalog of scholarly articles.
99.5% of the DOIs from Sci-Hub's list were in the LibGen scimag DOIs (after filtering).
Hence, the LibGen scimag and Sci-Hub repositories have stayed largely in sync since their split. 
On Twitter, the Sci-Hub account confirmed this finding, [commenting](https://twitter.com/Sci_Hub/status/844165613203480576) "with a small differences, yes the database is the same".
Therefore, the LibGen scimag and Sci-Hub DOI catalogs can presumably be used interchangeably for research purposes.

### Sci-Hub request logs

The 2016 study titled "Who's downloading pirated papers? Everyone" analyzed a dataset of Sci-Hub request logs [@RsNXQAG2; @t4r48QpO].
Alexandra Elbakyan worked with journalist John Bohannon to produce a dataset of download requests received by Sci-Hub from September 1, 2015 through February 29, 2016 [@kQFQ8EaO].
In November 2015, Sci-Hub's domain name was suspended as the result legal action by Elsevier [@16k28dBmH; @sR4uAYxB].
According to Bohannon, this resulted in "an 18-day gap in the data starting November 4, 2015 when the domain `sci-hub.org` went down and the server logs were improperly configured."
We show this downtime in Figure 1.

Of the 10,552,418 distinct DOIs in the request logs, 10,293,836 (97.5%) were part of the Crossref-derived catalog of scholarly articles.
Bohannon notes [@AeHqdtRV]: "some DOIs are invalid, due to typos from the Sci-Hub users or … because a website listed the wrong DOI."

We summarized the requests for each article using the following metrics:

1. downloads: total number of requests
2. visitors: number of IP addresses that requested the text
3. countries: number of countries (geolocation by IP address) that requested the text
4. days: number of days the text was requested
5. months: number of months the text was requested

Next, we calculated journal-level request metrics based on articles published from January 1, 2014 up until the start of the Sci-Hub request log records on September 1, 2015.
For each journal, we calculated the average values for the five request log metrics described above.
Interestingly, the journal [_Medicine - Programa de Formación Médica Continuada Acreditado_](http://www.sciencedirect.com/science/journal/03045412) received the most visitors per article, averaging 33.4 visitors for each of its 326 articles.

## Supplementary Information

![Coverage by country of publication](https://cdn.rawgit.com/greenelab/scihub/7891082161dbcfcd5eeb1d7b76ee99ab44b95064/figure/coverage-by-country.svg)

**Figure S1: Coverage by country of publication.**
Scopus assigns each journal a country of publication.
Sci-Hub's coverage is shown for countries with at least 100,000 articles.

![Bitcoin donations per month to Sci-Hub](https://cdn.rawgit.com/greenelab/scihub/7891082161dbcfcd5eeb1d7b76ee99ab44b95064/explore/bitcoin/monthly-donations-faceted.svg)

**Figure S2: bitcoin donations to Sci-Hub per month.**
For months since June 2015, total bitcoin donations (deposits to known Sci-Hub addresses) are assessed. 
Donations to USD refers to the United States dollar value at time of transaction confirmation.

![LibGen cumulative size over time](https://cdn.rawgit.com/greenelab/scihub/7891082161dbcfcd5eeb1d7b76ee99ab44b95064/figure/libgen-cumulative-works.svg)

**Figure S3: Number of articles in LibGen scimag over time.**
The figure shows the cumulative number of articles versus the LibGen scimag `DateAdded` field.
When comparing this plot to Figure 1 of Cabanac 2015 [@18KKRwlN6], we noticed a major discrepancy.
We hypothesize that the `DateAdded` field is replaced upon modification, making it impossible to assess date of first upload.

![LibGen cumulative size over time](https://cdn.rawgit.com/greenelab/scihub/7891082161dbcfcd5eeb1d7b76ee99ab44b95064/figure/libgen-monthly-lagtimes.svg)

**Figure S4: Lag-time from publication to LibGen upload.**
For each year of publication from 2010–2017, we plot the relationship between lag-time and LibGen scimag's coverage.
For example, this plot shows that 75% of articles published in 2011 were uploaded to LibGen within 60 months.
This analysis only considers articles where a month of publication can reliably be extracted, which excludes all articles that are allegedly published on the first day of each year.
This plot portrays lag-times as decreasing over time, but maximum coverage declining.
For example, coverage for 2016 articles exceeded 50% within 6 months, but appears to have reached an asymptote around 60%.
Alternatively, coverage for 2014 took 15 months to exceed 50% but has since then reached 75%.
However, this signal could result from post-dated LibGen upload timestamps.
Therefore, we caution against drawing any conclusions from LibGen `DateAdded` analyses, such as this, until more is known.


# References