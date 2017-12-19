## The Roman Numerals Kata

### The Kata

The Romans were a clever bunch. They conquered most of Europe and ruled it for hundreds of years. They invented concrete and straight roads. One thing they never discovered though was the number zero. This made writing and dating extensive histories of their exploits slightly more challenging, but the system of numbers they came up with is still in use today. For example, the BBC uses Roman numerals to date their programs.

The Romans wrote numbers using letters: I, V, X, L, C, D, M. I is for one, V for 5, X for 10, L for 50, C for 100, D for 500 and M for 1000. There is no 5000.

#### Part I

You should write a function to convert from normal numbers to Roman Numerals: eg

- `1` => `I`
- `10` => `X`
- `7` => `VII`

There is no need to be able to convert numbers larger than about 3000. The Romans themselves didn't tend to go any higher.

Note that you can't write numerals like "IM" for 999. Generally, symbols are placed in order of symbol value, starting with the largest values. When a smaller symbol precedes a larger one, the smaller value is subtracted from the larger one, and the result is added to the total.

Here are some additional rules:

* A number written in Arabic numerals can be broken into digits. To write a number in Roman numerals, each digit should be processed separately. For 1903, 1000 = M, 900 = CM, 3 = III. Thus, 1903 = MCMIII.
* The symbols I, X, C and M can be repeated three times in succession, but not more. 
* D, L and V can never be repeated.
* The symbol I can be subtracted from from V and X only. 
* X can be subtracted from D and C only. 
* C can be subtracted from M only.
* V, L and D can never be subtracted.
* Only smaller-value symbols may be subtracted from any large value symbol. (no negative numbers)

#### Part II

Write a function to convert in the other direction, ie numeral to digit. You can use 1999 (MCMXCIX) as an acceptance test.


