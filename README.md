# pytudes

Inspired by [norvig/pytudes](https://github.com/norvig/pytudes).

"An *étude* (a French word meaning study) is an instrumental musical composition, usually short, of considerable difficulty, and designed to provide practice material for perfecting a particular musical skill." &mdash; [Wikipedia](https://en.wikipedia.org/wiki/%C3%89tude)

This project contains **pytudes**&mdash;programs in Python (and other languages) for perfecting programming skills.

### Table of Contents

* [Exercises and Small Personal Projects](#small)
* [Larger Personal Projects](#large)

|<a name="small"></a>Exercises and Small Personal Projects|
|---|
|[Very Simple JSON Parser (Python)](https://gist.github.com/py-in-the-sky/02d18c427c07658adf0261a572e442d9)<br>*A simple recursive descent JSON parser in about 150 lines of Python. In some limited performance testing, my parser was only ten times slower than Python's [`json.loads`](https://docs.python.org/2/library/json.html#json.loads).*|
|[Very Simple Arithmetic Evaluator (Python)](https://gist.github.com/py-in-the-sky/a2c00053b8a9ae9c70ceb37b871cebae)<br>*A simple arithmetic evaluator in about 150 lines of Python. Parses arithmetic into a binary expression tree and then recursively evaluates the tree. I also implemented an [arithmetic-expression generator](https://gist.github.com/py-in-the-sky/a2c00053b8a9ae9c70ceb37b871cebae#file-very_simple_arithmetic_evaluator-py-L179-L219), which generates random valid arithmetic expressions for use in testing and benchmarking. In extensive performance testing, my evaluator took only twice the time that Python's built-in [`eval`](https://docs.python.org/2/library/functions.html#eval) took to evaluate random arithmetic expressions.*|
|[Concentric Diamonds (Clojure)](https://github.com/py-in-the-sky/challenges/blob/master/concentric_diamonds.clj)<br>*Prints out concentric diamonds of any width. For example, [width of two](https://github.com/py-in-the-sky/challenges/blob/master/concentric_diamonds.clj#L47-L56).*|
|[Bisect (Clojure)](https://github.com/py-in-the-sky/challenges/blob/master/bisect.clj)<br>*Port of Python's [`bisect_left`](https://docs.python.org/2/library/bisect.html#bisect.bisect_left) and [`bisect_right`](https://docs.python.org/2/library/bisect.html#bisect.bisect_right) functions to Clojure, with added comments on loop invariants in order to support reasoning about the correctness of the functions.*|
|[Super Digit (Haskell)](https://github.com/reprah/fp/blob/master/week-1-super-digit.hs)<br>*Recursive solution to [Super Digit](https://www.hackerrank.com/challenges/super-digit/problem).*|
|[Prechelt's Test (Python)](https://github.com/py-in-the-sky/challenges/blob/master/Prechelts_test_program/Prechelts_test_program.py)<br>*My Python solution to [Prechelt's test](http://www.flownet.com/ron/papers/lisp-java/instructions.html).*|
|[Quora Duplicate (Python)](https://github.com/py-in-the-sky/challenges/blob/master/quora_duplicate.py)<br>*A machine-learning program to address the [Quora duplicate-question problem](https://www.hackerrank.com/contests/quora-haqathon/challenges/duplicate). The program learns by example to detect a pair of duplicate Quora questions -- i.e., given two different posts from Quora, it indicates whether the posts represent the same underlying question or two different questions. I achieved third place on the problem, implementing a custom feature-selection function and leveraging ensemble learning methods.*|

|<a name="large"></a>Larger Personal Projects|
|---|
|[Evernote Coding Challenge (Python)](https://github.com/py-in-the-sky/challenges/blob/master/evernote.py)<br>*My submission to the [Evernote Coding Challenge](https://www.hackerrank.com/evernote-coding-challenge). In the first round of the competition, which involved automated testing, my implementation scored 100% correct, allowing me to proceed to the second (and final) round. In the final round, which involved review by the Evernote engineering team, I won second place. The challenge was to implement a sort of "Evernote light" that indexed user notes and supported quick lookup by various search techniques (by date, word, word prefix, etc.). I implemented and reused the trie datastructure to support all search APIs, and I developed my own [test suite](https://github.com/py-in-the-sky/challenges/blob/master/evernote_test.py) to iteratively develop against before submitting my solution to the online judge.*|
|[Intermediate Words Search (Ruby)](https://github.com/py-in-the-sky/challenges/tree/master/intermediate_words_search_ruby)<br>*Solves this problem: given two dictionary words, find the shortest path via single-letter edits (add, subtract, or change a letter) to get from the first word to the second, with the constraint that all intermediate words must also be in the dictionary. For example, a solution to "cat" and "dog" could be "cat--> cot--> dot--> dog". I implement both A\* and breadth-first search, as well as the heap data structure (used as a priority queue in A\* search) and the trie data structure. The A\* heuristic is a cheap underestimate of the edit distance between the current word and the target word. Benchmarking with a large dictionary (/usr/share/dict/words) compares the relative performance of A\* and BFS.*|
