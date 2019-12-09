![DSL Logo][dsllogo]


# Harvesting Tweets for Data Visualisation

The goal of this example is to show off TWARC, a command line based Twitter harvesting script that is one of the many tools available as part of the Digital Scholarship Labs Research Tools On Demand.  TWARC can havest tweets based on keywords in two main ways, search and filter.

#### Search

The search tool in TWARC can look at every tweet from the last seven days and harvest each that matches with one of your keywords.  This is great for quickly getting an idea of the latest trends pertaining to a topic.

#### Filter

The filter tool in TWARC is an active filter that captures any tweet that matches one of your keywords as it happens.  This is excellent for if there is an event that last for a few hours or days that you want to gather data on.  It can also be used to get an idea of how live a topic is withing windows of minutes, hours, days, or even months.

## Our Example

At the DSL we are big fans of data visualization so we set TWARC to harvest all tweets that included the keyword "datavisualization" for twenty-four hours.  This produced a file containing over four-hundred tweets!  We then used the R programming language to remove duplicate tweets (there were quite a few) and strip away the extra metadata that came with the tweets so that we could run some text analysis on them.  For mor information on that process feel free to check out the Jupyter Notebook file containing the code we used [here](https://github.com/BrockDSL/TWARC_Case_Study/blob/master/Example_Files/TWARC%20Json%20File%20Parsing%20in%20R.ipynb)
 


![Data Viz Word Cloud][wordcloud]



<!--- Please use reference style images so that it is easier to update pictures later --->

[dsllogo]: dsl_logo.png
[wordcloud]: dataviz_wordcloud.png
