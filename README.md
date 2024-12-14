<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<header>
  <h1>Customer Sorting by Lessons Program 📊</h1>
  <p>
    The program reads customer data from a CSV file, sorts the customers by the number of lessons using the quick sort algorithm, and writes the sorted data to a new CSV file.
  </p>
</header>

<hr>

<details>
  <summary>Table of Contents 📖</summary>
  <ul>
    <li><a href="#task">Task</a></li>
    <li><a href="#input-and-output">Input and Output</a></li>
    <li><a href="#examples">Examples</a></li>
    <li><a href="#requirements">Requirements</a></li>
    <li><a href="#usage">Usage</a></li>
  </ul>
</details>

<hr>

<section id="task">
  <h2>Task 🛠️</h2>
  <p>
    Modify the program from Project 7 to use quick sort to sort the customers by the number of lessons. Use the quick sort library function and implement a custom comparison function.
  </p>
</section>

<hr>

<section id="input-and-output">
  <h2>Input and Output 🖥️</h2>
  <h3>Input</h3>
  <ul>
    <li>The input file is named <code>customers.csv</code> and contains customer information formatted as email address (string), number of lessons (int), and name (string), with each customer on a separate line.</li>
    <li>The program reads the file using <code>fscanf</code> with the format specifier <code>%[^,],%d,%[^\n]\n</code>.</li>
  </ul>

  <h3>Output</h3>
  <ul>
    <li>The program outputs the sorted data to a file named <code>results.csv</code>.</li>
    <li>The format of the output file must be the same as the input: email, number of lessons, and name, with each customer on a separate line.</li>
  </ul>
</section>

<hr>

<section id="examples">
  <h2>Examples 📋</h2>
  <h3>Example Input (customers.csv)</h3>
  <div class="code-block">
    email1@example.com,5,John Doe<br>
    email2@example.com,10,Jane Smith<br>
    email3@example.com,3,Bob Johnson
  </div>
  
  <h3>Example Output (results.csv)</h3>
  <div class="code-block">
    email3@example.com,3,Bob Johnson<br>
    email1@example.com,5,John Doe<br>
    email2@example.com,10,Jane Smith
  </div>
  <p><strong>Explanation:</strong></p>
  <ul>
    <li>The program reads the customer data from <code>customers.csv</code>, sorts the customers by the number of lessons in ascending order, and writes the sorted data to <code>results.csv</code>.</li>
  </ul>
</section>

<hr>

<section id="requirements">
  <h2>Requirements ✔️</h2>
  <ol>
    <li>The program must use quick sort to sort the customers by the number of lessons.</li>
    <li>Implement a custom comparison function for <code>qsort</code>.</li>
    <li>The program should read data from an input file named <code>customers.csv</code>.</li>
    <li>Use <code>fscanf</code> with the format specifier <code>%[^,],%d,%[^\n]\n</code> to read the data into customer structures.</li>
    <li>The program must sort the customers by the number of lessons using quick sort.</li>
    <li>The program must output the sorted data to a file named <code>results.csv</code> in the same format as the input.</li>
    <li>Assume that the file will contain no more than 200 customers and that name and email are no longer than 100 characters.</li>
  </ol>
</section>

<hr>

<section id="usage">
  <h2>Usage 🚀</h2>
  <p><strong>1. Compile the Program:</strong></p>
  <div class="code-block">gcc -o customer_sort customer_sort.c</div>
  
  <p><strong>2. Run the Program:</strong></p>
  <div class="code-block">./customer_sort</div>
  
  <p><strong>3. Input File:</strong></p>
  <ul>
    <li>The input file <code>customers.csv</code> should be in the same directory as the program.</li>
  </ul>

  <p><strong>4. Output File:</strong></p>
  <ul>
    <li>The program will create an output file named <code>results.csv</code> with the sorted customer data.</li>
  </ul>
</section>

</body>
</html>
