# Benchmarking Code Generation with LLMs

📖 Related article: [Challenges in code generation with GPT-4](https://medium.com/@jamesmurdza/challenges-in-code-generation-with-gpt-4-3cc7cac71ff3)

Below is a comparison LLM code generation success on the <a href="https://github.com/jamesmurdza/human-eval">HumanEval</a> problem dataset. Each task was evaluated ten times per model, by first making a call to the OpenAI API, then running generated code against unit tests. Traces from each run are linked in the table below.

These results were generated with the [HumanEval-LangChain workflow](https://github.com/jamesmurdza/humaneval-langchain).

## Results

<table>
  <tr>
    <th></th>
    <th>Runs per task</th>
    <th>Tasks</th>
    <th>Overall success</th>
  </tr>
  <tr>
    <td>CodeLlama-34b-Instruct-hf</td>
    <td>10</td>
    <td>163</td>
    <td>45.1%</td>
  </tr>
  <tr>
    <td>gpt-3.5-turbo</td>
    <td>10</td>
    <td>163</td>
    <td>77.0%</td>
  </tr>
  <tr>
    <td>gpt-4</td>
    <td>10</td>
    <td>163</td>
    <td>84.8%</td>
  </tr>
</table>

## Results by task

<table>
  <tr>
    <th>Task</th>
    <th width="100">Code Llama</th>
    <th width="100">GPT-3.5</th>
    <th width="100">GPT-4</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>HumanEval/0</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/0.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/0.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/0.md">100%</a>
    </td>
    <td>
      Check if there are any two numbers in the given list that are closer to
      each other than the given threshold.
    </td>
  </tr>
  <tr>
    <td>HumanEval/1</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/1.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/1.md">40%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/1.md">60%</a>
    </td>
    <td>
      Separate multiple groups of nested parentheses into separate strings and
      return a list of those strings.
    </td>
  </tr>
  <tr>
    <td>HumanEval/2</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/2.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/2.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/2.md">100%</a>
    </td>
    <td>Return the decimal part of a positive floating point number.</td>
  </tr>
  <tr>
    <td>HumanEval/3</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/3.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/3.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/3.md">100%</a>
    </td>
    <td>
      Detect if at any point the balance of the bank account falls below zero
      and return True, otherwise return False.
    </td>
  </tr>
  <tr>
    <td>HumanEval/4</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/4.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/4.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/4.md">100%</a>
    </td>
    <td>Calculate the mean absolute deviation of a given list of numbers.</td>
  </tr>
  <tr>
    <td>HumanEval/5</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/5.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/5.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/5.md">100%</a>
    </td>
    <td>
      Insert a number 'delimeter' between every two consecutive elements of the
      input list `numbers`.
    </td>
  </tr>
  <tr>
    <td>HumanEval/6</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/6.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/6.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/6.md">100%</a>
    </td>
    <td>
      Parse a string representing multiple groups of nested parentheses and
      return a list of the deepest level of nesting for each group.
    </td>
  </tr>
  <tr>
    <td>HumanEval/7</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/7.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/7.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/7.md">100%</a>
    </td>
    <td>
      Filter an input list of strings to only include strings that contain a
      given substring.
    </td>
  </tr>
  <tr>
    <td>HumanEval/8</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/8.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/8.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/8.md">100%</a>
    </td>
    <td>Calculate the sum and product of all the integers in a given list.</td>
  </tr>
  <tr>
    <td>HumanEval/9</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/9.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/9.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-4/9.md">0%</a>
    </td>
    <td>
      Generate a list of rolling maximum elements found until a given moment in
      the sequence.
    </td>
  </tr>
  <tr>
    <td>HumanEval/10</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/10.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/10.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/10.md">100%</a>
    </td>
    <td>
      The function `make_palindrome` should find the shortest palindrome that
      begins with the supplied string.
    </td>
  </tr>
  <tr>
    <td>HumanEval/11</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/11.md">90%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/11.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/11.md">100%</a>
    </td>
    <td>
      Perform binary XOR on two input strings and return the result as a string.
    </td>
  </tr>
  <tr>
    <td>HumanEval/12</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/12.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/12.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/12.md">100%</a>
    </td>
    <td>
      Return the longest string from a list of strings, or None if the list is
      empty.
    </td>
  </tr>
  <tr>
    <td>HumanEval/13</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/13.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/13.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/13.md">100%</a>
    </td>
    <td>Calculate and return the greatest common divisor of two integers.</td>
  </tr>
  <tr>
    <td>HumanEval/14</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/14.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/14.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/14.md">100%</a>
    </td>
    <td>
      Return a list of all prefixes of the input string, from shortest to
      longest.
    </td>
  </tr>
  <tr>
    <td>HumanEval/15</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/15.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/15.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/15.md">100%</a>
    </td>
    <td>
      Return a string containing space-delimited numbers starting from 0 up to n
      inclusive.
    </td>
  </tr>
  <tr>
    <td>HumanEval/16</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/16.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/16.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/16.md">100%</a>
    </td>
    <td>
      Count the number of distinct characters in a given string, regardless of
      case.
    </td>
  </tr>
  <tr>
    <td>HumanEval/17</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/17.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/17.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/17.md">100%</a>
    </td>
    <td>
      Parse a string representing musical notes and return a list of integers
      representing the duration of each note in beats.
    </td>
  </tr>
  <tr>
    <td>HumanEval/18</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/18.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/18.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/18.md">100%</a>
    </td>
    <td>
      Count how many times a given substring can be found in the original
      string, including overlapping cases.
    </td>
  </tr>
  <tr>
    <td>HumanEval/19</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/19.md">90%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/19.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/19.md">100%</a>
    </td>
    <td>Sort the numbers in the input string from smallest to largest.</td>
  </tr>
  <tr>
    <td>HumanEval/20</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/20.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/20.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/20.md">100%</a>
    </td>
    <td>
      Find and return the two numbers in a list that are closest to each other.
    </td>
  </tr>
  <tr>
    <td>HumanEval/21</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/21.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/21.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/21.md">100%</a>
    </td>
    <td>
      Rescale a list of numbers to the unit interval [0, 1] using a linear
      transformation.
    </td>
  </tr>
  <tr>
    <td>HumanEval/22</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/22.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/22.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/22.md">100%</a>
    </td>
    <td>
      Filter a given list of any python values and return only the integers.
    </td>
  </tr>
  <tr>
    <td>HumanEval/23</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/23.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/23.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/23.md">100%</a>
    </td>
    <td>Return the length of a given string.</td>
  </tr>
  <tr>
    <td>HumanEval/24</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/24.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/24.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/24.md">100%</a>
    </td>
    <td>
      Find the largest number that evenly divides a given number n, smaller than
      n.
    </td>
  </tr>
  <tr>
    <td>HumanEval/25</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/25.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/25.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/25.md">100%</a>
    </td>
    <td>
      Factorize should return a list of prime factors of a given integer in
      ascending order.
    </td>
  </tr>
  <tr>
    <td>HumanEval/26</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/26.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/26.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/26.md">100%</a>
    </td>
    <td>
      Remove all elements from the list that occur more than once while keeping
      the order of the remaining elements the same.
    </td>
  </tr>
  <tr>
    <td>HumanEval/27</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/27.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/27.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/27.md">100%</a>
    </td>
    <td>
      The function should flip the case of each character in the given string.
    </td>
  </tr>
  <tr>
    <td>HumanEval/28</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/28.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/28.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/28.md">100%</a>
    </td>
    <td>Concatenate a list of strings into a single string.</td>
  </tr>
  <tr>
    <td>HumanEval/29</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/29.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/29.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/29.md">100%</a>
    </td>
    <td>
      Filter an input list of strings to only include strings that start with a
      given prefix.
    </td>
  </tr>
  <tr>
    <td>HumanEval/30</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/30.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/30.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/30.md">100%</a>
    </td>
    <td>
      Return a new list containing only the positive numbers from the input
      list.
    </td>
  </tr>
  <tr>
    <td>HumanEval/31</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/31.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/31.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/31.md">100%</a>
    </td>
    <td>Determine whether a given number is prime or not.</td>
  </tr>
  <tr>
    <td>HumanEval/32</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/32.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/32.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/32.md">30%</a>
    </td>
    <td>
      The function `find_zero` should find a zero point of a polynomial with
      given coefficients.
    </td>
  </tr>
  <tr>
    <td>HumanEval/33</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/33.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/33.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/33.md">100%</a>
    </td>
    <td>
      Sort the values at indices divisible by three in the given list, while
      keeping the values at other indices unchanged.
    </td>
  </tr>
  <tr>
    <td>HumanEval/34</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/34.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/34.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/34.md">100%</a>
    </td>
    <td>Return a sorted list of unique elements from the input list.</td>
  </tr>
  <tr>
    <td>HumanEval/35</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/35.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/35.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/35.md">100%</a>
    </td>
    <td>Return the maximum element in the given list.</td>
  </tr>
  <tr>
    <td>HumanEval/36</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/36.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/36.md">90%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/36.md">100%</a>
    </td>
    <td>
      Count the number of times the digit 7 appears in integers less than n that
      are divisible by 11 or 13.
    </td>
  </tr>
  <tr>
    <td>HumanEval/37</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/37.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/37.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/37.md">100%</a>
    </td>
    <td>
      Sort the even indices of a list in ascending order, while keeping the odd
      indices unchanged.
    </td>
  </tr>
  <tr>
    <td>HumanEval/38</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/38.md">10%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/38.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/38.md">100%</a>
    </td>
    <td>
      The function `encode_cyclic` should return an encoded string by cycling
      groups of three characters, while the function `decode_cyclic` should
      return the decoded string from an encoded string.
    </td>
  </tr>
  <tr>
    <td>HumanEval/39</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/39.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/39.md">20%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/39.md">100%</a>
    </td>
    <td>
      Return the n-th number that is both a Fibonacci number and a prime number.
    </td>
  </tr>
  <tr>
    <td>HumanEval/40</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/40.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/40.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/40.md">100%</a>
    </td>
    <td>
      Check if there are three distinct elements in a list that sum to zero.
    </td>
  </tr>
  <tr>
    <td>HumanEval/41</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/41.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/41.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/41.md">60%</a>
    </td>
    <td>
      Count the number of collisions between cars moving in opposite directions
      on an infinitely long road.
    </td>
  </tr>
  <tr>
    <td>HumanEval/42</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/42.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/42.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/42.md">100%</a>
    </td>
    <td>
      The function should return a list with all elements incremented by 1.
    </td>
  </tr>
  <tr>
    <td>HumanEval/43</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/43.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/43.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/43.md">100%</a>
    </td>
    <td>
      Check if there are two distinct elements in a list that sum to zero.
    </td>
  </tr>
  <tr>
    <td>HumanEval/44</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/44.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/44.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/44.md">100%</a>
    </td>
    <td>
      Convert a given number from its current base to a specified base and
      return the string representation of the converted number.
    </td>
  </tr>
  <tr>
    <td>HumanEval/45</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/45.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/45.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/45.md">100%</a>
    </td>
    <td>
      Calculate and return the area of a triangle given the length of one side
      and the height.
    </td>
  </tr>
  <tr>
    <td>HumanEval/46</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/46.md">40%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/46.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/46.md">100%</a>
    </td>
    <td>
      Compute the n-th element of the Fib4 number sequence efficiently without
      using recursion.
    </td>
  </tr>
  <tr>
    <td>HumanEval/47</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/47.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/47.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/47.md">100%</a>
    </td>
    <td>Calculate and return the median of the elements in the given list.</td>
  </tr>
  <tr>
    <td>HumanEval/48</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/48.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/48.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/48.md">100%</a>
    </td>
    <td>Check if the given string is a palindrome.</td>
  </tr>
  <tr>
    <td>HumanEval/49</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/49.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/49.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/49.md">100%</a>
    </td>
    <td>Calculate the value of 2 raised to the power of n modulo p.</td>
  </tr>
  <tr>
    <td>HumanEval/50</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/50.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/50.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/50.md">100%</a>
    </td>
    <td>
      The function above should decode a string that has been encoded using the
      encode_shift function.
    </td>
  </tr>
  <tr>
    <td>HumanEval/51</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/51.md">20%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/51.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/51.md">100%</a>
    </td>
    <td>The function should remove all vowels from a given string.</td>
  </tr>
  <tr>
    <td>HumanEval/52</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/52.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/52.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/52.md">100%</a>
    </td>
    <td>Return True if all numbers in the list l are below the threshold t.</td>
  </tr>
  <tr>
    <td>HumanEval/53</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/53.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/53.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/53.md">100%</a>
    </td>
    <td>The function should add two numbers together.</td>
  </tr>
  <tr>
    <td>HumanEval/54</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/54.md">20%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/54.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/54.md">100%</a>
    </td>
    <td>Check if two words have the same characters.</td>
  </tr>
  <tr>
    <td>HumanEval/55</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/55.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/55.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-4/55.md">0%</a>
    </td>
    <td>Return the n-th Fibonacci number.</td>
  </tr>
  <tr>
    <td>HumanEval/56</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/56.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/56.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/56.md">100%</a>
    </td>
    <td>
      Check if every opening bracket in the given string has a corresponding
      closing bracket.
    </td>
  </tr>
  <tr>
    <td>HumanEval/57</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/57.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/57.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/57.md">100%</a>
    </td>
    <td>
      Return True if the elements in the given list are monotonically increasing
      or decreasing.
    </td>
  </tr>
  <tr>
    <td>HumanEval/58</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/58.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/58.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/58.md">100%</a>
    </td>
    <td>
      Return a sorted list of unique common elements between two input lists.
    </td>
  </tr>
  <tr>
    <td>HumanEval/59</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/59.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/59.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/59.md">100%</a>
    </td>
    <td>Return the largest prime factor of a given number.</td>
  </tr>
  <tr>
    <td>HumanEval/60</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/60.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/60.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/60.md">100%</a>
    </td>
    <td>
      The function `sum_to_n` should calculate the sum of numbers from 1 to n.
    </td>
  </tr>
  <tr>
    <td>HumanEval/61</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/61.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/61.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/61.md">100%</a>
    </td>
    <td>
      Check if every opening bracket in the given string has a corresponding
      closing bracket.
    </td>
  </tr>
  <tr>
    <td>HumanEval/62</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/62.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/62.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/62.md">100%</a>
    </td>
    <td>
      Calculate the derivative of a polynomial represented by a list of
      coefficients.
    </td>
  </tr>
  <tr>
    <td>HumanEval/63</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/63.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/63.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/63.md">100%</a>
    </td>
    <td>Compute the n-th element of the FibFib number sequence efficiently.</td>
  </tr>
  <tr>
    <td>HumanEval/64</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/64.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/64.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/64.md">90%</a>
    </td>
    <td>
      Count the number of vowels in a given word, considering 'y' as a vowel
      only when it is at the end of the word.
    </td>
  </tr>
  <tr>
    <td>HumanEval/65</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/65.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/65.md">60%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/65.md">100%</a>
    </td>
    <td>
      Shift the digits of the integer x to the right by shift positions and
      return the result as a string, or reverse the digits if shift is greater
      than the number of digits.
    </td>
  </tr>
  <tr>
    <td>HumanEval/66</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/66.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/66.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/66.md">100%</a>
    </td>
    <td>
      The function should calculate the sum of the ASCII codes of the uppercase
      characters in a given string.
    </td>
  </tr>
  <tr>
    <td>HumanEval/67</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/67.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/67.md">80%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/67.md">100%</a>
    </td>
    <td>
      Return the number of mango fruits in the basket given the total number of
      fruits and the number of apples and oranges.
    </td>
  </tr>
  <tr>
    <td>HumanEval/68</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/68.md">90%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/68.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/68.md">100%</a>
    </td>
    <td>
      The function `pluck` should find the smallest even value in an array
      representing a branch of a tree and return it along with its index.
    </td>
  </tr>
  <tr>
    <td>HumanEval/69</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/69.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/69.md">60%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/69.md">100%</a>
    </td>
    <td>
      Return the greatest integer that has a frequency greater than or equal to
      the value of the integer itself, or -1 if no such integer exists.
    </td>
  </tr>
  <tr>
    <td>HumanEval/70</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/70.md">40%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/70.md">70%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/70.md">100%</a>
    </td>
    <td>Sort a given list of integers in a specific order.</td>
  </tr>
  <tr>
    <td>HumanEval/71</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/71.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/71.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/71.md">100%</a>
    </td>
    <td>
      Calculate the area of a triangle if the given side lengths form a valid
      triangle, otherwise return -1.
    </td>
  </tr>
  <tr>
    <td>HumanEval/72</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/72.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/72.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/72.md">100%</a>
    </td>
    <td>
      Return True if the object q is balanced and the sum of its elements is
      less than or equal to the maximum weight w, otherwise return False.
    </td>
  </tr>
  <tr>
    <td>HumanEval/73</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/73.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/73.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/73.md">100%</a>
    </td>
    <td>
      Find the minimum number of elements that need to be changed to make the
      array palindromic.
    </td>
  </tr>
  <tr>
    <td>HumanEval/74</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/74.md">10%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/74.md">20%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/74.md">80%</a>
    </td>
    <td>
      Return the list with the total number of characters in all strings less
      than the other list, or the first list if they have the same number of
      characters.
    </td>
  </tr>
  <tr>
    <td>HumanEval/75</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/75.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/75.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/75.md">100%</a>
    </td>
    <td>Check if the given number is the product of three prime numbers.</td>
  </tr>
  <tr>
    <td>HumanEval/76</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/76.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/76.md">70%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/76.md">80%</a>
    </td>
    <td>
      The function should determine whether a given number is a simple power of
      another given number.
    </td>
  </tr>
  <tr>
    <td>HumanEval/77</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/77.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/77.md">50%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/77.md">50%</a>
    </td>
    <td>Check if the given integer is a cube of some integer number.</td>
  </tr>
  <tr>
    <td>HumanEval/78</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/78.md">10%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/78.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/78.md">100%</a>
    </td>
    <td>
      Count the number of prime hexadecimal digits in a given hexadecimal
      number.
    </td>
  </tr>
  <tr>
    <td>HumanEval/79</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/79.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/79.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/79.md">100%</a>
    </td>
    <td>
      Convert a decimal number to binary format and return it as a string with
      'db' at the beginning and end.
    </td>
  </tr>
  <tr>
    <td>HumanEval/80</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/80.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/80.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/80.md">100%</a>
    </td>
    <td>
      Check if a given string is ""happy"" by determining if its length is at
      least 3 and every 3 consecutive letters are distinct.
    </td>
  </tr>
  <tr>
    <td>HumanEval/81</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/81.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/81.md">80%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/81.md">100%</a>
    </td>
    <td>
      The function should convert a list of GPAs into a list of corresponding
      letter grades.
    </td>
  </tr>
  <tr>
    <td>HumanEval/82</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/82.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/82.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/82.md">100%</a>
    </td>
    <td>
      Return True if the length of the input string is a prime number, and False
      otherwise.
    </td>
  </tr>
  <tr>
    <td>HumanEval/83</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/83.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/83.md">40%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-4/83.md">0%</a>
    </td>
    <td>
      Count the number of n-digit positive integers that start or end with 1.
    </td>
  </tr>
  <tr>
    <td>HumanEval/84</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/84.md">20%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/84.md">70%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-4/84.md">0%</a>
    </td>
    <td>
      Return the total sum of the digits of a positive integer in binary form.
    </td>
  </tr>
  <tr>
    <td>HumanEval/85</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/85.md">60%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/85.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/85.md">100%</a>
    </td>
    <td>
      Add the even elements that are at odd indices in a given non-empty list of
      integers.
    </td>
  </tr>
  <tr>
    <td>HumanEval/86</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/86.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/86.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/86.md">100%</a>
    </td>
    <td>
      The function should return a string where all the words are replaced by a
      new word with their characters arranged in ascending order based on ascii
      value, while keeping the order of words and blank spaces in the sentence.
    </td>
  </tr>
  <tr>
    <td>HumanEval/87</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/87.md">60%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/87.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-4/87.md">0%</a>
    </td>
    <td>
      The function should return a list of tuples representing the coordinates
      of the integer x in the given 2-dimensional list, sorted by rows in
      ascending order and by columns in descending order.
    </td>
  </tr>
  <tr>
    <td>HumanEval/88</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/88.md">10%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/88.md">90%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/88.md">100%</a>
    </td>
    <td>
      Sort the given array in ascending order if the sum of the first and last
      index values is odd, or sort it in descending order if the sum is even,
      and return a copy of the sorted array.
    </td>
  </tr>
  <tr>
    <td>HumanEval/89</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/89.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/89.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/89.md">100%</a>
    </td>
    <td>
      Encrypt a given string by shifting each letter down the alphabet by two
      multiplied to two places.
    </td>
  </tr>
  <tr>
    <td>HumanEval/90</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/90.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/90.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/90.md">100%</a>
    </td>
    <td>
      The function should return the second smallest element in a given list of
      integers, or None if there is no such element.
    </td>
  </tr>
  <tr>
    <td>HumanEval/91</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/91.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/91.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-4/91.md">0%</a>
    </td>
    <td>
      Count the number of sentences that start with the word ""I"" in a given
      string.
    </td>
  </tr>
  <tr>
    <td>HumanEval/92</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/92.md">70%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/92.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/92.md">100%</a>
    </td>
    <td>
      Return true if one of the numbers is equal to the sum of the other two,
      and all numbers are integers; otherwise, return false.
    </td>
  </tr>
  <tr>
    <td>HumanEval/93</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/93.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/93.md">10%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-4/93.md">0%</a>
    </td>
    <td>
      Encode a given message by swapping the case of all letters and replacing
      vowels with the letter that appears 2 places ahead in the English
      alphabet.
    </td>
  </tr>
  <tr>
    <td>HumanEval/94</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/94.md">20%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/94.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/94.md">100%</a>
    </td>
    <td>
      The function should find the largest prime value in a given list of
      integers and return the sum of its digits.
    </td>
  </tr>
  <tr>
    <td>HumanEval/95</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/95.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/95.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/95.md">100%</a>
    </td>
    <td>
      Check if all keys in a dictionary are either all lowercase or all
      uppercase strings, and return True if they are, otherwise return False.
    </td>
  </tr>
  <tr>
    <td>HumanEval/96</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/96.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/96.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/96.md">100%</a>
    </td>
    <td>Return an array of the first n prime numbers that are less than n.</td>
  </tr>
  <tr>
    <td>HumanEval/97</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/97.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/97.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/97.md">100%</a>
    </td>
    <td>Return the product of the unit digits of two given integers.</td>
  </tr>
  <tr>
    <td>HumanEval/98</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/98.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/98.md">70%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/98.md">100%</a>
    </td>
    <td>
      Count the number of uppercase vowels in even indices of a given string.
    </td>
  </tr>
  <tr>
    <td>HumanEval/99</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/99.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/99.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/99.md">100%</a>
    </td>
    <td>
      Return the closest integer to a given number, rounding away from zero if
      the number is equidistant from two integers.
    </td>
  </tr>
  <tr>
    <td>HumanEval/100</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/100.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/100.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/100.md">100%</a>
    </td>
    <td>
      Create a pile of stones with a specific number of levels, where each level
      has a specific number of stones.
    </td>
  </tr>
  <tr>
    <td>HumanEval/101</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/101.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/101.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/101.md">100%</a>
    </td>
    <td>
      Split a string of words separated by commas or spaces into an array of
      individual words.
    </td>
  </tr>
  <tr>
    <td>HumanEval/102</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/102.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/102.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/102.md">100%</a>
    </td>
    <td>
      Return the largest even integer within the range [x, y] inclusive, or -1
      if there is no such number.
    </td>
  </tr>
  <tr>
    <td>HumanEval/103</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/103.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/103.md">20%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/103.md">100%</a>
    </td>
    <td>
      Calculate the average of a range of integers, round it to the nearest
      integer, and convert it to binary.
    </td>
  </tr>
  <tr>
    <td>HumanEval/104</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/104.md">70%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/104.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/104.md">100%</a>
    </td>
    <td>
      Return a sorted list of positive integers from the input list that do not
      contain any even digits.
    </td>
  </tr>
  <tr>
    <td>HumanEval/105</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/105.md">50%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/105.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/105.md">90%</a>
    </td>
    <td>
      Sort an array of integers between 1 and 9 inclusive, reverse the array,
      and replace each digit with its corresponding name.
    </td>
  </tr>
  <tr>
    <td>HumanEval/106</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/106.md">80%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/106.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/106.md">30%</a>
    </td>
    <td>
      Calculate and return a list of size n, where each element at index i is
      the factorial of i if i is even, or the sum of numbers from 1 to i
      otherwise.
    </td>
  </tr>
  <tr>
    <td>HumanEval/107</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/107.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/107.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/107.md">100%</a>
    </td>
    <td>
      The function should return a tuple containing the number of even and odd
      integer palindromes within the range (1, n).
    </td>
  </tr>
  <tr>
    <td>HumanEval/108</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/108.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/108.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/108.md">10%</a>
    </td>
    <td>
      Count the number of elements in the array that have a sum of digits
      greater than 0.
    </td>
  </tr>
  <tr>
    <td>HumanEval/109</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/109.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/109.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/109.md">100%</a>
    </td>
    <td>
      Determine if it is possible to obtain a sorted array by performing right
      shift operations on the given array.
    </td>
  </tr>
  <tr>
    <td>HumanEval/110</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/110.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/110.md">10%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/110.md">100%</a>
    </td>
    <td>
      Determine whether it is possible to exchange elements between two lists to
      make the first list contain only even numbers.
    </td>
  </tr>
  <tr>
    <td>HumanEval/111</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/111.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/111.md">90%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/111.md">100%</a>
    </td>
    <td>
      Return a dictionary containing the letter(s) with the highest occurrence
      and their corresponding count from a given string.
    </td>
  </tr>
  <tr>
    <td>HumanEval/112</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/112.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/112.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/112.md">100%</a>
    </td>
    <td>
      The function should delete characters from string `s` that are equal to
      any character in string `c`, and then check if the resulting string is a
      palindrome.
    </td>
  </tr>
  <tr>
    <td>HumanEval/113</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/113.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/113.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/113.md">100%</a>
    </td>
    <td>
      Count the number of odd digits in each string of a given list and return a
      list of strings describing the count for each string.
    </td>
  </tr>
  <tr>
    <td>HumanEval/114</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/114.md">40%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/114.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/114.md">100%</a>
    </td>
    <td>
      Calculate the minimum sum of any non-empty sub-array in the given array of
      integers.
    </td>
  </tr>
  <tr>
    <td>HumanEval/115</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/115.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/115.md">20%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-4/115.md">0%</a>
    </td>
    <td>
      The function `max_fill` should calculate the number of times the buckets
      need to be lowered in order to empty the wells in the given grid.
    </td>
  </tr>
  <tr>
    <td>HumanEval/116</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/116.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/116.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/116.md">100%</a>
    </td>
    <td>
      Sort an array of non-negative integers based on the number of ones in
      their binary representation in ascending order, and for numbers with the
      same number of ones, sort based on decimal value.
    </td>
  </tr>
  <tr>
    <td>HumanEval/117</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/117.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/117.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/117.md">100%</a>
    </td>
    <td>
      Return a list of words from the input string that contain exactly n
      consonants.
    </td>
  </tr>
  <tr>
    <td>HumanEval/118</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/118.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/118.md">20%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/118.md">10%</a>
    </td>
    <td>
      Find the closest vowel that stands between two consonants from the right
      side of the word.
    </td>
  </tr>
  <tr>
    <td>HumanEval/119</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/119.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/119.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/119.md">40%</a>
    </td>
    <td>
      Check if it is possible to concatenate two strings of parentheses in some
      order to create a balanced string.
    </td>
  </tr>
  <tr>
    <td>HumanEval/120</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/120.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/120.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-4/120.md">0%</a>
    </td>
    <td>Return a sorted list of the maximum k numbers in the given array.</td>
  </tr>
  <tr>
    <td>HumanEval/121</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/121.md">80%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/121.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/121.md">100%</a>
    </td>
    <td>
      Return the sum of all odd elements in even positions in a given list of
      integers.
    </td>
  </tr>
  <tr>
    <td>HumanEval/122</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/122.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/122.md">10%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/122.md">100%</a>
    </td>
    <td>
      The function should return the sum of the elements with at most two digits
      from the first k elements of the given array.
    </td>
  </tr>
  <tr>
    <td>HumanEval/123</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/123.md">10%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/123.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/123.md">100%</a>
    </td>
    <td>
      Return a sorted list of the odd numbers in the Collatz sequence for a
      given positive integer.
    </td>
  </tr>
  <tr>
    <td>HumanEval/124</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/124.md">90%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/124.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/124.md">100%</a>
    </td>
    <td>
      Validate a given date string and return True if the date is valid
      according to the specified rules, otherwise return False.
    </td>
  </tr>
  <tr>
    <td>HumanEval/125</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/125.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/125.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/125.md">100%</a>
    </td>
    <td>
      The function should split a string of words on whitespace or commas, and
      if neither exists, it should return the number of lowercase letters with
      odd order in the alphabet.
    </td>
  </tr>
  <tr>
    <td>HumanEval/126</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/126.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/126.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/126.md">50%</a>
    </td>
    <td>
      Check if a given list of numbers is sorted in ascending order and does not
      contain more than one duplicate of the same number.
    </td>
  </tr>
  <tr>
    <td>HumanEval/127</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/127.md">90%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/127.md">10%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/127.md">80%</a>
    </td>
    <td>
      Determine whether the length of the intersection of two intervals is a
      prime number.
    </td>
  </tr>
  <tr>
    <td>HumanEval/128</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/128.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/128.md">80%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/128.md">60%</a>
    </td>
    <td>
      The function `prod_signs` should calculate the sum of the magnitudes of
      integers in the input array, multiplied by the product of the signs of
      each number.
    </td>
  </tr>
  <tr>
    <td>HumanEval/129</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/129.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/129.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/129.md">20%</a>
    </td>
    <td>
      Find the minimum path of length k in a grid, where each cell contains a
      unique value, and return the ordered list of values on the cells that the
      minimum path goes through.
    </td>
  </tr>
  <tr>
    <td>HumanEval/130</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/130.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/130.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-4/130.md">0%</a>
    </td>
    <td>
      Return a list of the first n + 1 numbers of the Tribonacci sequence.
    </td>
  </tr>
  <tr>
    <td>HumanEval/131</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/131.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/131.md">10%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/131.md">100%</a>
    </td>
    <td>
      Return the product of the odd digits in a given positive integer, or 0 if
      all digits are even.
    </td>
  </tr>
  <tr>
    <td>HumanEval/132</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/132.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/132.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-4/132.md">0%</a>
    </td>
    <td>
      Check if a given string contains a valid subsequence of square brackets
      where at least one bracket is nested.
    </td>
  </tr>
  <tr>
    <td>HumanEval/133</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/133.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/133.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/133.md">100%</a>
    </td>
    <td>
      The function should calculate the sum of the squared numbers in a given
      list, after rounding each element to the nearest upper integer.
    </td>
  </tr>
  <tr>
    <td>HumanEval/134</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/134.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/134.md">90%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-4/134.md">0%</a>
    </td>
    <td>
      Check if the last character of a given string is an alphabetical character
      and is not part of a word.
    </td>
  </tr>
  <tr>
    <td>HumanEval/135</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/135.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/135.md">80%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/135.md">100%</a>
    </td>
    <td>
      Return the largest index of an element that is not greater than or equal
      to the element immediately preceding it, or -1 if no such element exists.
    </td>
  </tr>
  <tr>
    <td>HumanEval/136</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/136.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/136.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/136.md">100%</a>
    </td>
    <td>
      Return a tuple containing the largest negative integer and the smallest
      positive integer from a given list, or None if there are no negative or
      positive integers.
    </td>
  </tr>
  <tr>
    <td>HumanEval/137</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/137.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/137.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/137.md">90%</a>
    </td>
    <td>
      Return the larger variable in its given variable type, or None if the
      values are equal.
    </td>
  </tr>
  <tr>
    <td>HumanEval/138</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/138.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/138.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/138.md">90%</a>
    </td>
    <td>
      Evaluate whether the given number n can be written as the sum of exactly 4
      positive even numbers.
    </td>
  </tr>
  <tr>
    <td>HumanEval/139</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/139.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/139.md">80%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/139.md">100%</a>
    </td>
    <td>Calculate the special factorial of a given integer.</td>
  </tr>
  <tr>
    <td>HumanEval/140</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/140.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/140.md">70%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/140.md">50%</a>
    </td>
    <td>
      Replace spaces in a given string with underscores, and if there are more
      than 2 consecutive spaces, replace them with a hyphen.
    </td>
  </tr>
  <tr>
    <td>HumanEval/141</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/141.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/141.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/141.md">90%</a>
    </td>
    <td>Validate whether a given file name meets certain criteria.</td>
  </tr>
  <tr>
    <td>HumanEval/142</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/142.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/142.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/142.md">100%</a>
    </td>
    <td>
      Calculate the sum of squared and cubed entries in a list based on their
      index.
    </td>
  </tr>
  <tr>
    <td>HumanEval/143</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/143.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/143.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/143.md">100%</a>
    </td>
    <td>
      Return a string containing the words from the original sentence whose
      lengths are prime numbers, in the same order as the original sentence.
    </td>
  </tr>
  <tr>
    <td>HumanEval/144</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/144.md">90%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/144.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/144.md">100%</a>
    </td>
    <td>
      The function should determine whether the product of two fractions is a
      whole number or not.
    </td>
  </tr>
  <tr>
    <td>HumanEval/145</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/145.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/145.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-4/145.md">0%</a>
    </td>
    <td>
      Sort the given list of integers in ascending order based on the sum of
      their digits, with ties broken by the index in the original list.
    </td>
  </tr>
  <tr>
    <td>HumanEval/146</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/146.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/146.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/146.md">100%</a>
    </td>
    <td>
      Count the number of elements in the input array that are greater than 10
      and have both the first and last digits as odd numbers.
    </td>
  </tr>
  <tr>
    <td>HumanEval/147</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/147.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/147.md">90%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-4/147.md">0%</a>
    </td>
    <td>
      Calculate the number of triples in an array where the sum of the elements
      is a multiple of 3.
    </td>
  </tr>
  <tr>
    <td>HumanEval/148</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/148.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/148.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/148.md">80%</a>
    </td>
    <td>
      Return a tuple of planets whose orbits are located between the orbit of
      planet1 and the orbit of planet2, sorted by proximity to the sun.
    </td>
  </tr>
  <tr>
    <td>HumanEval/149</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/149.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/149.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/149.md">100%</a>
    </td>
    <td>
      Delete strings with odd lengths from a list of strings and return the
      remaining strings in ascending order of length, with alphabetical sorting
      for strings of the same length.
    </td>
  </tr>
  <tr>
    <td>HumanEval/150</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/150.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/150.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/150.md">100%</a>
    </td>
    <td>
      Return the value of x if n is a prime number and return the value of y
      otherwise.
    </td>
  </tr>
  <tr>
    <td>HumanEval/151</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/151.md">50%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/151.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/151.md">90%</a>
    </td>
    <td>
      Calculate the sum of squares of the odd numbers in the given list,
      ignoring negative numbers and non-integers.
    </td>
  </tr>
  <tr>
    <td>HumanEval/152</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/152.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/152.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/152.md">100%</a>
    </td>
    <td>
      The function should compare the guesses of a person with the actual scores
      of a number of matches and return an array indicating how far off each
      guess was.
    </td>
  </tr>
  <tr>
    <td>HumanEval/153</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/153.md">10%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/153.md">70%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/153.md">50%</a>
    </td>
    <td>
      Return the strongest extension for a given class name and list of
      extensions.
    </td>
  </tr>
  <tr>
    <td>HumanEval/154</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/154.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/154.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/154.md">100%</a>
    </td>
    <td>
      Check if the second word or any of its rotations is a substring in the
      first word.
    </td>
  </tr>
  <tr>
    <td>HumanEval/155</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/155.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/155.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-4/155.md">0%</a>
    </td>
    <td>
      Return a tuple containing the count of even and odd digits in the given
      integer.
    </td>
  </tr>
  <tr>
    <td>HumanEval/156</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/156.md">40%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/156.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/156.md">100%</a>
    </td>
    <td>
      Convert a positive integer to its lowercase Roman numeral equivalent.
    </td>
  </tr>
  <tr>
    <td>HumanEval/157</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/157.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/157.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/157.md">100%</a>
    </td>
    <td>
      Check if the given lengths of the three sides of a triangle form a
      right-angled triangle.
    </td>
  </tr>
  <tr>
    <td>HumanEval/158</td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./codellama-34b-instruct/158.md">40%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/158.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/158.md">100%</a>
    </td>
    <td>
      Return the word with the maximum number of unique characters from a list
      of strings.
    </td>
  </tr>
  <tr>
    <td>HumanEval/159</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/159.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-3.5-turbo/159.md">50%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/159.md">100%</a>
    </td>
    <td>
      The function should calculate the total number of carrots eaten and the
      number of carrots remaining after a rabbit has eaten a certain number of
      carrots and still needs to eat more.
    </td>
  </tr>
  <tr>
    <td>HumanEval/160</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/160.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/160.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/160.md">50%</a>
    </td>
    <td>
      Evaluate an algebraic expression using the given operators and operands.
    </td>
  </tr>
  <tr>
    <td>HumanEval/161</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/161.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/161.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/161.md">100%</a>
    </td>
    <td>
      Reverse the case of letters in a string, and if the string contains no
      letters, reverse the string.
    </td>
  </tr>
  <tr>
    <td>HumanEval/162</td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./codellama-34b-instruct/162.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-3.5-turbo/162.md">100%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/00ff00/00ff00.png" />
      <a href="./gpt-4/162.md">100%</a>
    </td>
    <td>Convert a given string into its MD5 hash equivalent.</td>
  </tr>
  <tr>
    <td>HumanEval/163</td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./codellama-34b-instruct/163.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/f03c15/f03c15.png" />
      <a href="./gpt-3.5-turbo/163.md">0%</a>
    </td>
    <td>
      <img src="https://placehold.co/15x15/ffea00/ffea00.png" />
      <a href="./gpt-4/163.md">80%</a>
    </td>
    <td>
      Generate a list of even digits between two given positive integers, in
      ascending order.
    </td>
  </tr>
</table>
