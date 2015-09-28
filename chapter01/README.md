### Chapter 1

## Exercises

(01)&nbsp;&nbsp;&nbsp;&nbsp; Try using the Python interpreter as a calculator, and typing expressions like ``` 12 / (4 + 1) ```.

(02)&nbsp;&nbsp;&nbsp;&nbsp; Given an alphabet of 26 letters, there are 26 to the power 10, or 26 ** 10, ten-letter strings we can form. That works out to 141167095653376. How many hundred-letter strings are possible?

(03)&nbsp;&nbsp;&nbsp;&nbsp; The Python multiplication operation can be applied to lists. What happens when you type the following?
``` python
    ['Monty', 'Python'] * 20
    # OR
    3 * sent1
```

(04)&nbsp;&nbsp;&nbsp;&nbsp; Review [Section 1](http://www.nltk.org/book/ch01.html#sec-computing-with-language-texts-and-words) on computing with language. How many words are there in ``` text2 ``` ? How many distinct words are there?

(05)&nbsp;&nbsp;&nbsp;&nbsp; Compare the lexical diversity scores for humor and romance fiction in [Section 1.1](http://www.nltk.org/book/ch01.html#tab-brown-types). Which genre is more lexically diverse?

(06)&nbsp;&nbsp;&nbsp;&nbsp; Produce a dispersion plot of the four main protagonists in Sense and Sensibility: <i>Elinor</i>, <i>Marianne</i>, <i>Edward</i>, and <i>Willoughby</i>. What can you observe about the different roles played by the males and females in this novel? Can you identify the couples?

(07)&nbsp;&nbsp;&nbsp;&nbsp; Find the collocations in ``` text5 ```.

(08)&nbsp;&nbsp;&nbsp;&nbsp; Consider the following Python expression: ``` len(set(text4)) ```. State the purpose of this expression. Describe the two steps involved in performing this computation.

(09)&nbsp;&nbsp;&nbsp;&nbsp; Review [Section 2](http://www.nltk.org/book/ch01.html#sec-a-closer-look-at-python-texts-as-lists-of-words) on lists and strings.
* Define a string and assign it to a variable, e.g., ``` my_string = 'My String' ``` (but put something more interesting in the string). Print the contents of this variable in two ways, first by simply typing the variable name and pressing enter, then by using the ``` print ``` statement.
* Try adding the string to itself using ``` my_string + my_string ```, or multiplying it by a number, e.g., ``` my_string * 3 ```. Notice that the strings are joined together without any spaces. How could you fix this?

(10)&nbsp;&nbsp;&nbsp;&nbsp; Define a variable ``` my_sent ``` to be a list of words, using the syntax ``` my_sent = ["My", "sent"] ``` (but with your own words, or a favorite saying).
* Use ``` ' '.join(my_sent) ``` to convert this into a string.
* Use ``` split() ``` to split the string back into the list form you had to start with.

(11)&nbsp;&nbsp;&nbsp;&nbsp; Define several variables containing lists of words, e.g., ``` phrase1, phrase2 ```, and so on. Join them together in various combinations (using the plus operator) to form whole sentences. What is the relationship between ``` len(phrase1 + phrase2) ``` and ``` len(phrase1) + len(phrase2) ```?

(12)&nbsp;&nbsp;&nbsp;&nbsp; Consider the following two expressions, which have the same value. Which one will typically be more relevant in NLP? Why?
``` python
    "Monty Python"[6:12]
    ["Monty", "Python"][1]
```

(13)&nbsp;&nbsp;&nbsp;&nbsp; We have seen how to represent a sentence as a list of words, where each word is a sequence of characters. What does ``` sent1[2][2] ``` do? Why? Experiment with other index values.

(14)&nbsp;&nbsp;&nbsp;&nbsp; The first sentence of ``` text3 ``` is provided to you in the variable ``` sent3 ```. The index of the in ``` sent3 ``` is ``` 1 ```, because ``` sent3[1] ``` gives us ``` 'the' ```. What are the indexes of the two other occurrences of this word in ``` sent3 ```?

(15)&nbsp;&nbsp;&nbsp;&nbsp; Review the discussion of conditionals in [Section 4](http://www.nltk.org/book/ch01.html#sec-making-decisions). Find all words in the Chat Corpus (``` text5 ```) starting with the letter ``` b ```. Show them in alphabetical order.

(16)&nbsp;&nbsp;&nbsp;&nbsp; Type the expression ``` list(range(10)) ``` at the interpreter prompt. Now try ``` list(range(10, 20)) ```, ``` list(range(10, 20, 2)) ```, and ``` list(range(20, 10, -2)) ```. We will see a variety of uses for this built-in function in later chapters.

(17)&nbsp;&nbsp;&nbsp;&nbsp; Use ``` text9.index() ``` to find the index of the word <i>sunset</i>. You'll need to insert this word as an argument between the parentheses. By a process of trial and error, find the slice for the complete sentence that contains this word.

(18)&nbsp;&nbsp;&nbsp;&nbsp; Using list addition, and the set and sorted operations, compute the vocabulary of the sentences ``` sent1 ... sent8 ```.

(19)&nbsp;&nbsp;&nbsp;&nbsp; What is the difference between the following two lines? Which one will give a larger value? Will this be the case for other texts?
``` python
    sorted(set(w.lower() for w in text1))
    sorted(w.lower() for w in set(text1))
```

(20)&nbsp;&nbsp;&nbsp;&nbsp; What is the difference between the following two texts: ``` w.isupper() ``` and not ``` w.islower() ```?

(21)&nbsp;&nbsp;&nbsp;&nbsp; Write the slice expression that extracts the last two words of ``` text2 ```.

(22)&nbsp;&nbsp;&nbsp;&nbsp; Find all the four-letter words in the Chat Corpus ( ``` text5 ```). With the help of a frequency distribution (``` FreqDist ```), show these words in decreasing order of frequency.

(23)&nbsp;&nbsp;&nbsp;&nbsp; Review the discussion of looping with conditions in [Section 4](http://www.nltk.org/book/ch01.html#sec-making-decisions). Use a combination of for and if statements to loop over the words of the movie script for Monty Python and the Holy Grail (``` text6 ```) and print all the uppercase words, one per line.

(24)&nbsp;&nbsp;&nbsp;&nbsp; Write expressions for finding all words in ``` text6 ``` that meet the conditions listed below. The result should be in the form of a list of words: ``` ['word1', 'word2', ...] ```.
* Ending in <i>ize</i>
* Containing the letter <i>z</i>
* Containing the sequence of letters <i>pt</i>
* Having all lowercase letters except for an initial capital (i.e., <i>titlecase</i>)

(25)&nbsp;&nbsp;&nbsp;&nbsp; Define sent to be the list of words ``` ['she', 'sells', 'sea', 'shells', 'by', 'the', 'sea', 'shore'] ```. Now write code to perform the following tasks:
* Print all words beginning with <i>sh</i>
* Print all words longer than four characters

(26)&nbsp;&nbsp;&nbsp;&nbsp; What does the following Python code do? ``` sum(len(w) for w in text1) ``` Can you use it to work out the average word length of a text?

(27)&nbsp;&nbsp;&nbsp;&nbsp; Define a function called ``` vocab_size(text) ``` that has a single parameter for the text, and which returns the vocabulary size of the text.

(28)&nbsp;&nbsp;&nbsp;&nbsp; Define a function ``` percent(word, text) ``` that calculates how often a given word occurs in a text, and expresses the result as a percentage.

(29)&nbsp;&nbsp;&nbsp;&nbsp; We have been using sets to store vocabularies. Try the following Python expression: ``` set(sent3) < set(text1) ```. Experiment with this using different arguments to ``` set() ```. What does it do? Can you think of a practical application for this?
