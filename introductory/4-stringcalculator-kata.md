## The String Calculator Kata

### The Kata

1) Create a simple String calculator with a method `int add(String numbers)`

The method can take 0, 1 or 2 numbers, and will return their sum. 
For an empty string it will return 0. 

example inputs include: `""`, `"1"` or `"1,2"`.

* Start with the simplest test case of an empty string and move to 1 and two numbers.
* Remember to solve things as simply as possible so that you force yourself to write tests you did not think about.
* Remember to refactor after each passing test.

2) Allow the `add()` method to handle any number of numbers. eg: `"1,2,3,4"`

3) Allow the `add()` method to also handle new lines between numbers instead of simply commas.
* the following input is ok:  `"1\n2,3"`, the result is 6.
* the following input is NOT ok:  `"1,\n"`, nor is `"1\n,"`. In short, empty tokens are not allowed, aside from the empty string.

4)  Support different delimiters.
* To change a delimiter, the beginning of the string will contain a separate line that looks like this:   `//[delimiter]\n[numbers…]` for example `//;\n1;2` should return three where the default delimiter is `;`.
* The first line is optional. all existing scenarios should still be supported

5) Calling `add()` with a negative number will throw an exception `negatives not allowed` - and the negative that was passed. If there are multiple negatives, show all of them in the exception message.

6) Numbers bigger than 1000 should be ignored, so adding 2 + 1001  = 2