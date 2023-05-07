Download Link: https://assignmentchef.com/product/solved-kit103-assignment3-divisibility-of-really-really-big-integers
<br>
<h1>Question 1: Divisibility of really, really big integers</h1>

In many programming languages the native integer data types have an upper limit on their maximum value. To test the divisibility of numbers larger than can be represented natively it can be convenient to instead work with strings of digits, as character strings can grow inde nitely.

<table>

 <tbody>

  <tr>

   <td width="44"></td>

  </tr>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>

Task: There are incomplete functions in the assignment script le that are intended to test large numbers (de ned by strings of the characters ‘0’ through ‘9’) for divisibility by various values. Complete the implementations of these functions by applying the common divisibility rules for 2, 3, 4, and 11 (the functions are named divisible_by_n <sub>∈</sub> {2, 3, 4, 11}). KMA155 students must implement the rules for divisibility by 2, 3 and 4.

Hints:

Your functions will be tested with strings, like ‘1234’, not integers such as 1234. These are not equivalent: the rst occupies more than 64 bits in memory (4 × 2-byte characters), while the small integer value is likely only 32 bits.

Practical 6 (week 7) contains some similar examples and describes how to access individual characters in a string by index (which may count backwards from the end of the string).

String <u>slicing</u> may also be useful in up to two of the above functions.

You might not need to convert any part of the string to a number (but if you’ve applied the common divisibility rules and have reached the point where that makes sense then it’s ne for you to do so).

<h1>Question 2: GCD from a prime factorisation</h1>

Both the math and programming lecture streams have described how to calculate gcd(a, b) using the prime factorisations of a and b. Your task is to complete the stub function q2_factor_gcd(a, b) to implement this behaviour. In your solution you should use the Python <u>Counter</u> class to represent a multiset/bag, and make use of the included helper function factor_list to generate a list of prime factors for each input.

<h1>Question 3: Are a and b coprime (i.e., relatively prime)? (</h1>

In the assignment script le there is a stub function q3_coprime(a, b) that is intended to return True if a and b are relatively prime, False otherwise (coprime is another term for relatively prime, and provides a shorter function name).

Based on your knowledge, the math lecture notes and programming lab exercises, implement q3_coprime. You may, in fact probably should, implement at least one additional helper function, which must use the most direct approach to deriving its answer (i.e., you may not reuse the answer to any other question in this assignment). With that helper function available the body of q3_coprime could be as short as one line of code.

<h1>Information on string slicing</h1>

The following information on string slicing (essentially, taking a substring from a string) may be helpful in some parts of <u>Question 1</u>. For a string s:

s[start:end] <em># characters start through end-1</em>

s[start:]    <em># characters start through the rest of the string</em> s[:end]      <em># characters from the beginning through end-1</em>

s[:]         <em># a copy of the whole string</em>

And you may optionally include a step value:

s[start:end:step] <em># start through not past end, by step</em>

So, for example, s[2::3] copies every third character in s starting with the third character (i.e., position 2) up to the end (because the end position was omitted).