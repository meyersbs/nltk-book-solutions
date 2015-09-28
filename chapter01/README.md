### Chapter 1

## Exercises

(01) Try using the Python interpreter as a calculator, and typing expressions like 12 / (4 + 1).

(02) Given an alphabet of 26 letters, there are 26 to the power 10, or 26 ** 10, ten-letter strings we can form. That works out to 141167095653376. How many hundred-letter strings are possible?

(03) The Python multiplication operation can be applied to lists. What happens when you type the following?
``` python
    ['Monty', 'Python'] * 20
    # OR
    3 * sent1
```

(04) Review [Section 1](http://www.nltk.org/book/ch01.html#sec-computing-with-language-texts-and-words) on computing with language. How many words are there in ``` text2 ``` ? How many distinct words are there?

(05) Compare the lexical diversity scores for humor and romance fiction in [Section 1.1](http://www.nltk.org/book/ch01.html#tab-brown-types). Which genre is more lexically diverse?

(06) Produce a dispersion plot of the four main protagonists in Sense and Sensibility: <i>Elinor</i>, <i>Marianne</i>, <i>Edward</i>, and <i>Willoughby</i>. What can you observe about the different roles played by the males and females in this novel? Can you identify the couples?

(07) Find the collocations in ``` text5 ```.

(08) Consider the following Python expression: ``` len(set(text4)) ```. State the purpose of this expression. Describe the two steps involved in performing this computation.

(09) Review [Section 2](http://www.nltk.org/book/ch01.html#sec-a-closer-look-at-python-texts-as-lists-of-words) on lists and strings.
* Define a string and assign it to a variable, e.g., ``` my_string = 'My String' ``` (but put something more interesting in the string). Print the contents of this variable in two ways, first by simply typing the variable name and pressing enter, then by using the ``` print ``` statement.
* Try adding the string to itself using ``` my_string + my_string ```, or multiplying it by a number, e.g., ``` my_string * 3 ```. Notice that the strings are joined together without any spaces. How could you fix this?

(10) Define a variable ``` my_sent ``` to be a list of words, using the syntax ``` my_sent = ["My", "sent"] ``` (but with your own words, or a favorite saying).
* Use ``` ' '.join(my_sent) ``` to convert this into a string.
* Use ``` split() ``` to split the string back into the list form you had to start with.

(11) Define several variables containing lists of words, e.g., ``` phrase1, phrase2 ```, and so on. Join them together in various combinations (using the plus operator) to form whole sentences. What is the relationship between ``` len(phrase1 + phrase2) ``` and ``` len(phrase1) + len(phrase2) ```?

(12) Consider the following two expressions, which have the same value. Which one will typically be more relevant in NLP? Why?
``` python
    "Monty Python"[6:12]
    ["Monty", "Python"][1]
```

(13) We have seen how to represent a sentence as a list of words, where each word is a sequence of characters. What does ``` sent1[2][2] ``` do? Why? Experiment with other index values.

(14) The first sentence of ``` text3 ``` is provided to you in the variable ``` sent3 ```. The index of the in ``` sent3 ``` is ``` 1 ```, because ``` sent3[1] ``` gives us ``` 'the' ```. What are the indexes of the two other occurrences of this word in ``` sent3 ```?

(15) Review the discussion of conditionals in [Section 4](http://www.nltk.org/book/ch01.html#sec-making-decisions). Find all words in the Chat Corpus (``` text5 ```) starting with the letter ``` b ```. Show them in alphabetical order.

(16) Type the expression ``` list(range(10)) ``` at the interpreter prompt. Now try ``` list(range(10, 20)) ```, ``` list(range(10, 20, 2)) ```, and ``` list(range(20, 10, -2)) ```. We will see a variety of uses for this built-in function in later chapters.

(17) Use ``` text9.index() ``` to find the index of the word <i>sunset</i>. You'll need to insert this word as an argument between the parentheses. By a process of trial and error, find the slice for the complete sentence that contains this word.

(18) Using list addition, and the set and sorted operations, compute the vocabulary of the sentences ``` sent1 ... sent8 ```.

(19) What is the difference between the following two lines? Which one will give a larger value? Will this be the case for other texts?
``` python
    sorted(set(w.lower() for w in text1))
    sorted(w.lower() for w in set(text1))
```

(20) What is the difference between the following two texts: ``` w.isupper() ``` and not ``` w.islower() ```?

(21) Write the slice expression that extracts the last two words of ``` text2 ```.

(22) 
