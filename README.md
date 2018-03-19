# pytudes

Inspired by [norvig/pytudes](https://github.com/norvig/pytudes).

"An *étude* (a French word meaning study) is an instrumental musical composition, usually short, of considerable difficulty, and designed to provide practice material for perfecting a particular musical skill." &mdash; [Wikipedia](https://en.wikipedia.org/wiki/%C3%89tude)

This project contains **pytudes**&mdash;programs in Python (and other languages) for perfecting programming skills.

### Table of Contents

* [Exercises and Small Personal Projects](#small)
* [Larger Personal Projects](#large)

|<a name="small"></a>Exercises and Small Personal Projects|
|---|
|[Very Simple JSON Parser (Python)](https://gist.github.com/py-in-the-sky/02d18c427c07658adf0261a572e442d9)<br>*A simple recursive descent JSON parser in about 150 lines of Python. In some limited performance testing, my parser was ten times slower than Python's [`json.loads`](https://docs.python.org/2/library/json.html#json.loads).*|
|[Very Simple Arithmetic Evaluator (Python)](https://gist.github.com/py-in-the-sky/a2c00053b8a9ae9c70ceb37b871cebae)<br>*A simple arithmetic evaluator in about 150 lines of Python. It parses arithmetic into a binary expression tree and then recursively evaluates the tree. I also implemented an [arithmetic-expression generator](https://gist.github.com/py-in-the-sky/a2c00053b8a9ae9c70ceb37b871cebae#file-very_simple_arithmetic_evaluator-py-L179-L219), which generates random valid arithmetic expressions for use in testing and benchmarking. In extensive performance testing, my evaluator took twice the time that Python's built-in [`eval`](https://docs.python.org/2/library/functions.html#eval) took to evaluate random arithmetic expressions.*|
|[Concentric Diamonds (Clojure)](https://github.com/py-in-the-sky/challenges/blob/master/concentric_diamonds.clj)<br>*Prints out concentric diamonds of any width. For example, [width of two](https://github.com/py-in-the-sky/challenges/blob/master/concentric_diamonds.clj#L47-L56).*|
|[Bisect (Clojure)](https://github.com/py-in-the-sky/challenges/blob/master/bisect.clj)<br>*Port of Python's [`bisect_left`](https://docs.python.org/2/library/bisect.html#bisect.bisect_left) and [`bisect_right`](https://docs.python.org/2/library/bisect.html#bisect.bisect_right) functions to Clojure, with added comments on loop invariants in order to support reasoning about the correctness of the functions.*|
|[Bisect and Binary Search (Python)](https://gist.github.com/py-in-the-sky/e84fd9fc4db0da3f351631ba04b2d91b)<br>*Reflections on and revision of Python's `bisect_left` and `bisect_right` functions, after having read chapter 4 of [Beautiful Code](http://shop.oreilly.com/product/9780596510046.do).*|
|[Rotation Point (Python)](https://github.com/py-in-the-sky/challenges/blob/master/rotation_point.py)<br>*An adaptation of binary search. [A sorted array has been rotated](https://www.interviewcake.com/question/python/find-rotation-point) (e.g., all elements have been shifted to the right by two spots). Can you efficiently find the rotation point? In other words, can you quickly find by how many indices the array has been rotated? The solution runs in O(logN) time. The docstring of the Python file includes extensive analysis of the algorithm's correctness.*|
|[Super Digit (Haskell)](https://github.com/reprah/fp/blob/master/week-1-super-digit.hs)<br>*Recursive solution to [Super Digit](https://www.hackerrank.com/challenges/super-digit/problem).*|
|[Prechelt's Test (Python)](https://github.com/py-in-the-sky/challenges/blob/master/Prechelts_test_program/Prechelts_test_program.py)<br>*My Python solution to [Prechelt's test](http://www.flownet.com/ron/papers/lisp-java/instructions.html).*|
|[Quora Duplicate (Python)](https://github.com/py-in-the-sky/challenges/blob/master/quora_duplicate.py)<br>*A machine-learning program to address the [Quora duplicate-question problem](https://www.hackerrank.com/contests/quora-haqathon/challenges/duplicate). The program learns by example to detect a pair of duplicate Quora questions -- i.e., given two different posts from Quora, it indicates whether the posts represent the same underlying question or two different questions. I achieved third place on the problem, implementing a custom feature-selection function and leveraging ensemble learning methods.*|
|[Welcome to Code Jam (Python)](https://github.com/py-in-the-sky/challenges/blob/master/google-code-jam/welcome_to_code_jam.py)<br>*Given an arbitrary string `S`, how many subsequences of `S` spell out [`"welcome to code jam"`](https://code.google.com/codejam/contest/90101/dashboard#s=p2)? Beware, the brute-force approach of considering all subsequences of `S` that are `K` characters long, where `K = len("welcome to code jam")`, is too inefficient -- there are `O(N choose K)` such subsequences, where `N = len(S)`. My solution runs in `O(N * K**2)` time and `O(K**3)` extra space.*|
|[Good Memories (Python)](https://github.com/py-in-the-sky/challenges/blob/master/hackerrank/good_memories.py)<br>*Each person in a group of friends [tries to remember](https://www.hackerrank.com/contests/booking-passions-hacked-backend/challenges/good-memories/problem) the sequence of events from the previous night. Are all their memories consistent with each other? This problem neatly reduces to determining whether a directed graph has a cycle.*|
|[Rather Perplexing Showdown (Python)](https://github.com/py-in-the-sky/challenges/blob/master/google-code-jam/rather_perplexing_showdown.py)<br>*How to best organize a [peculiar rock-paper-scissors tournament](https://code.google.com/codejam/contest/10224486/dashboard).*|
|[Best Trade (Python)](https://gist.github.com/py-in-the-sky/6e34ffa33d3a8aac5017c5c15ccd57fd)<br>*Given a list of prices of some stock, determine the maximum money that could be made from buying and then selling once. That is, find the value `prices[sell_index] - prices[buy_index]` such that `len(prices) > sell_index >= buy_index >= 0` and for all other such index pairs `(sell_index_2, buy_index_2)`, it is the case that:<br>`prices[sell_index] - prices[buy_index] >= prices[sell_index_2] - prices[buy_index_2]`*|
|[Lucky Dip (Python)](https://gist.github.com/py-in-the-sky/ab54a2de17b2c5379f6fa1b6946a588d)<br>*Solution to the Google Code Jam problem [Lucky Dip](https://codejam.withgoogle.com/codejam/contest/9234486/dashboard#s=p1). Calculates the expected value of a game, assuming the player plays "optimally."*|

|<a name="large"></a>Larger Personal Projects|
|---|
|[Evernote Coding Challenge (Python)](https://github.com/py-in-the-sky/challenges/blob/master/evernote.py)<br>*My submission to the [Evernote Coding Challenge](https://www.hackerrank.com/evernote-coding-challenge). In the first round of the competition, which involved automated testing, my implementation scored 100% correct, allowing me to proceed to the second (and final) round. In the final round, which involved review by the Evernote engineering team, I won second place. The challenge was to implement a sort of "Evernote light" that indexed user notes and supported quick lookup by various search techniques (by date, word, word prefix, etc.). I implemented and reused the trie datastructure to support all search APIs, and I developed my own [test suite](https://github.com/py-in-the-sky/challenges/blob/master/evernote_test.py) to iteratively develop against before submitting my solution to the online judge.*|
|[Intermediate Words Search (Ruby)](https://github.com/py-in-the-sky/challenges/tree/master/intermediate_words_search_ruby)<br>*Solves this problem: given two dictionary words, find the shortest path via single-letter edits (add, subtract, or change a letter) to get from the first word to the second, with the constraint that all intermediate words must also be in the dictionary. For example, a solution to "cat" and "dog" could be "cat--> cot--> dot--> dog". I implement both A\* and breadth-first search (BFS), as well as the heap data structure (used as a priority queue in A\* search) and the trie data structure (used for storing the dictionary and finding all words that are one edit away from a given word). The A\* heuristic is a cheap underestimate of the edit distance between the current word and the target word. Benchmarking with a large dictionary (/usr/share/dict/words) compares the relative performance of A\* and BFS. A\* significantly outperforms BFS both in terms of dictionary words visited and in terms of elapsed time.*|
