![DSL Logo][dsllogo]


# Harvesting Tweets for Data Visualisation

The goal of this example is to show off [I am not sure about using "show off" here. Perhaps some different language with an opening sentence? Like..."The Brock University Digital Scholarship Lab has implemented use of the Twitter Archive (TWARC). TWARC is" a command line based Twitter harvesting script that is one of [the][remove the] many tools available as part of the Digital Scholarship Labs [Lab's] Research Tools On Demand [(RTOD)].  TWARC can ha[r]vest tweets based on keywords in two main ways,[;] search and filter.

### Search

The search tool in TWARC can look at every tweet from the last seven days and harvest each [one] that matches with [remove "one of"]one of your keywords.  This is great for quickly getting an idea of the [maybe..." This is great for quickly understanding the latest trends....or learning more about the latest trends...pertaining to a topic"] latest trends pertaining to a topic.

### Filter

The filter tool in TWARC is an active filter that captures any tweet that matches one of your keywords as it happens.  This is excellent for if there is an event that last[s] [or"spans a few hours or days"] for a few hours or days that you want to gather data on.  It can also be used to get an idea of how live [do you mean active?] a topic is withing [within - removeg?] windows of minutes, hours, days, or even months.

## Our Example

At the DSL we are big fans of data visualization so we set TWARC to harvest all tweets that included the keyword "datavisualization"(did you harvest "datavisualization" or "data visualization"?] for twenty-four hours.  This produced a file containing over four-hundred tweets!  We then used the R programming language to remove duplicate tweets (there were quite a few) and strip away the extra metadata that came with the tweets so that we could run some [perform instead of run some] text analysis on them.  Once we had a clean text file to work with we uploaded it into the Lexos software provided free online by Wheaton College in Massachusetts (check it out [here](https://wheatoncollege.edu/academics/special-projects-initiatives/lexomics/lexos-installers/) if you are interested) and using a curated list of stopwords, we created a wordcloud out of our tweets showing the fifty most commonly used words.

![Data Viz Word Cloud][wordcloud]

We have provided all of the data that was used in this example [here](https://github.com/BrockDSL/TWARC_Case_Study/tree/master/Example_Files).  Included is:

- The original .json file that was produced by TWARC
- A Jupyter Notebook containing the R code used to clean the data
- The text file produced by the R scripts
- Stopword lists formatted for use in either Lexos or Voyant


<!--- Please use reference style images so that it is easier to update pictures later --->

[dsllogo]: dsl_logo.png
[wordcloud]: dataviz_wordcloud.png
