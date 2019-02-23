# Final Project for practical python learning

This project is meant to give you an actual, useful application which you will build using basics of python you have learned in the tutorials so far.

As different students seek different levels of learning, this project can be done at 2 different levels - EASY and  HARD. The way it is designed is that solving the EASY project gives you material which can be used in the medium project, and similarly, the solving the medium project gives you material for the hard. So, it's 2 steps in some sense. For each project we will explain to you what you need to do in words, to convert that into code has been left to you.

# EASY PROJECT: Text manipulation

### 1. Downloading data to work with

Please install the package nltk, using - 

```
pip install nltk
```

Now, open a python shell and run these commands to download the "brown corpus" (https://www.nltk.org/book/ch02.html) -

```
import nltk
nltk.download('brown')
```

This will give you access to a bunch of sentences. The code for reading these sentences from the Brown corpus is 2-3 lines of code, but you will have to write these yourselves. Go to section 1.3 Brown Corpus on the link above. Read the code there, it clearly shows how to get the sentences from it.

### 2. Finding lines which contain one out of a list of few words.

Define a list of 4 words of your choice. Let's call these "important words". For ex - list with words "hello","nation","technology","book". Now, go through each sentence in the brown corpus, one by one, searching which sentence contains one of the 4 important words.

### 3. Store sentences which contain a match.

Create a dictionary. In this dictionary, you will store information such that the keys of the dictionary will be the important words, i.e. 4 keys. The corresponding value for each key will be a list of all sentences which contain that word.
Your task is to read files from disk, filter lines which contain a specific word, store it in a dictionary


# HARD PROJECT: Text manipulation

In the easy project we learned how to manipulate text, to go through the text and find lines which contain a match for certain pre-defined words. However, we got our dataset simply by downloading from python. In the medium project, the task is to download your own dataset.

You will be scraping movie summaries from Wikipedia for this. Most movies have a Wikipedia page, and they almost always contain a synopsis or plot section. This will take some effort, but is great practice. 

1. Get a list of movies from here - https://github.com/enilsen16/imdb-top-250/blob/master/top_250.txt
2. For each movie. This is going to be significant effort, but you can follow this project - https://medium.com/@Alexander_H/scraping-wikipedia-with-python-8000fc9c9e6c
3. For each movie link, you can now download all the text on the wikipedia page.
4. Now that you have the text, see how you can get the text in the plot/synopsis section.These summaries are your new dataset. 

5. Use the code you wrote in the EASY project to find movies who's summaries contain the important words. This time, make a dictionary where keys are the important words, and corresponding values are lists of movie names who's summary contains the important word.
