## The Anagram Kata

This kata can be found on the excellent site by Dave Thomas: http://codekata.com/kata/kata06-anagrams/. 

It is quite a tricky kata, especially if you want to implement it in the right way, that is with an optimal algorithm. Finding anagrams is not that hard, but finding them efficiently is a little harder. 

### The Kata

The challenge is fairly simple: given a file containing one word per line, print out all the combinations of words that are anagrams; each line in the output contains all the words from the input that are anagrams of each other. For example, your program might include in its output:

```text
kinship pinkish
enlist inlets listen silent
boaster boaters borates
fresher refresh
sinks skins
knits stink
rots sort
```

If you run this on the word list here (anagrams-wordlist.txt) you should find 20683 sets of anagrams (a total of 48162 words), including all-time favorites such as: 

```text
crepitus cuprites pictures piecrust
paste pates peats septa spate tapes tepas
punctilio unpolitic
sunders undress
```

For added programming pleasure, find the longest words that are anagrams, and find the set of anagrams containing the most words (so `parsley players replays sparely` would not win, having only four words in the set).

#### Kata Objectives

Apart from having some fun with words, this kata should make you think somewhat about algorithms. The simplest algorithms to find all the anagram combinations may take inordinate amounts of time to do the job. Working though alternatives should help bring the time down by orders of magnitude. To give you a possible point of comparison, a solution hacked together by Dave in 25 lines of Ruby runs this wordlist in 1.8s on a 1.7GHz i7. It’s also an interesting exercise in testing: can you write unit tests to verify that your code is working correctly before setting it to work on the full dictionary.

## A cute algorithm

This tweet details a cute mathematical algorithm to solve this problem: [https://twitter.com/fermatslibrary/status/875340896379817984](https://twitter.com/fermatslibrary/status/875340896379817984), thanks to the guys behind the [Fermat's Library](https://twitter.com/fermatslibrary) Twitter account. 

It is by no means the only solution.
