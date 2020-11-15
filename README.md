# tweet_filter
This is simple scoring-filtering system that allows the user to filter to tweets that are irrelevant to their search intent.<br>

## How it works
The idea is to construct a word corpus that is related to the search terms (eg. heart attack). This is being done by utilising a python package called wikipedia, which parse artilces from Wikipedia website based on the search term.<br>

Content from Wikipedia is then used to contruct a word corpus noting the number of occurrence it appreaded in the article. Frequency of the word will serve as a scoring factor when used in the dataset.

When running the scoring system through the dataset, the sentence will get a positive score for every word it matches with the word corpus and get a negative -0.25 score for every word that does not match the word courpus. Scoring can be applyed to the sentence in a separate column in the dataframe. 
