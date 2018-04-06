# Rick & Morty Transcript Natural Language Processing

Using transcripts scraped from [Rickipedia](http://rickandmorty.wikia.com/wiki/Rickipedia), I'll apply try my hand at various Natural Language Processing techniques.

Wrangling (Scraping and cleaning of raw data) of the data is handled in `RandMWrangle.ipynb`. Final scraped transcripts in .txt and .csv form can be found in the respective seasonfolder. Much of season 3 is, at this time, unable to be input into the dataset. Additionally I had a hard time scraping subtitles for "the ricks must be crazy" from Hulu.

Further cleaning (standardizing the raw data) Is handled in `RandMClean.ipynb` Final cleaned data is saved as `clean_RandMtranscript.csv`.
Data is a standard csv file with the columns that index by sentence number, and indicate the episode, season, character, and line spoken. Note that this was saved with index_label set to false, so labels are shifted if you open in excel, but it should load into R and python correctly. One more note, as data was scraped from transcripts, subtitles, and other sources, various scene action detail is found in the data. This extra information is categorized under the "character" of `Scene_Action`.

Some minor cleaning and Natural Language Processing (NLP) is then performed in `RandM_Words_and_NLP.ipynb`. As this is my first time doing some serious NLP, I added a bunch of references and notes at the beginning of this document. Most are reprocessed and paraphrased/restated in my own words for my own purposes from referenced pages. This is a work in progress, However some neat Word Clouds can be found in the `word_cloud` folder.
