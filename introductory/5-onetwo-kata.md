## The One Two Kata

### The Kata

#### Part 1

We need a method to convert strings to other strings in the following way. To understand the conversion, just read the input string. The first example string shows one two. There is indeed one number, and this number is two.

* ``2`` -> ``one two``
* ``1 2`` -> ``one one one two``

Easy. Now, we can also count numbers, as in the following examples.

* ``2 2`` -> ``two two``
* ``3 9 9 9 8 8`` -> ``one three three nine two eight``
* ``1 1 1 1 1 1 1`` -> ``seven one``
* ``2 4 4 4 6 6 6 6 6`` -> ``one two three four five six``

Got it? Now, to keep things simple, we do not count past 9. Thus the conversion of the following string.

* ``5 5 5 5 5 5 5 5 5 5 5 5`` -> ``nine five three five``

#### Part 2

And of course we would like a second method to do the opposite conversion.