This tutorial assumes a basic understanding of the following -

- HTML, CSS and JS
- Some basic C based programming knowledge regarding if/else, variables, loops, operators (`+, -, *, /, !=, ==`), functions etc

## Purpose of this document

- This document serves as a guideline and is not intended to be a tutorial.
- The points mentioned in the guidelines are starting points to begin your exploration.

## Task 1 - Understanding how browsers and a server communicate via  Web Browser.

The web is distributed, one system sitting on one part of the globe connects to another via the Internet. 
 The **client** sends a request to the **server**. The server processes the request and sends a  response back to the client. Read more about it here - 

http://abhinavsingh.com/blog/2008/11/what-happens-before-you-finally-viewed-this-page/

##### By the end of this task you should be able to -

1. Understand the request-response cycle 
2. Understand the purpose of a server
3. Understand the purpose of a browser.

## Task 2 - Installing the LAMP/WAMP stack on your machine.

- If you are a Microsoft Windows user, please access this URL to learn how to install WAMP on your machine. - http://youtu.be/3j5lxcV_320
- If you are a Linux user, the installation process might defer based on the distribution you use. Any article that you find on digitalocean.com should be a good place to start on how to install the LAMP stack on Linux.
- Ensure that you are install PHP version 5.4 or above.

##### By the end of this task you should be able to -

1. Install LAMP stack on Windows or Linux based PC's.

## Task 3 - Understanding the LAMP/WAMP Stack.

You should be familiar with the following -

#### L - Linux, W - Windows
Operating System, purpose is to run other application software.

#### A - Apache 
- What's a web server?
- What are some other web servers?
- Apache's root directory (You'll be putting your PHP files here)

#### M - MySQL
- What's a database system?
- What are some other database software?

#### P - PHP
- Full form for PHP
- A brief history. 
- What's a dynamic programming language?
- What's the difference between a static language like C and a dynamic programming language like PHP?
- Examples of some other dynamic languages.
- PHP is an interpreted programming language.
- The PHP configuration file - `php.ini`. Location of this varies based on the OS.
- Extension of a PHP file.
- Understanding the REQUEST - RESPONSE cycle on Apache/PHP based webserver - http://abhinavsingh.com/blog/2008/11/how-does-php-echos-a-hello-world-behind-the-scene/
- PHP has a very good documentation @ http://php.net/docs.php
- Whenever you go through the documentation, ensure that you glance through the comments at the bottom too.

##### By the end of this task you should be able to -

1. Familiar with basics of Apache and MySQL
2. Difference between a dynamic and static programming language.
3. An interpreted programming language.
4. Familiarity with the PHP documentation website.

## Task 4 - Setting up your Workspace

- What's an IDE?
- Installing **NetBeans** with PHP - https://netbeans.org/kb/trails/php.html, https://netbeans.org/downloads/index.html
- What's debugging? 
- What are breakpoints while debugging?
- Pardon the poor music - https://www.youtube.com/watch?v=HbJOP0YcSjs 
- Setting up **MySQLWorkbench** for connecting to MySQL - http://www.mysql.com/products/workbench/

##### By the end of this task you should be able to -

1. Familiar with the various preferences in Netbeans.
2. Familiarity with debugging code and breakpoints.
3. Familiarity with the **MySQLWorkbench**


## Task 5 - [Quick Crash Course] Tutorials on the PHP.NET website

The best place to continue now would be to complete the following tuts - 

1. http://php.net/manual/en/tutorial.firstpage.php
2. http://php.net/manual/en/tutorial.useful.php
3. http://php.net/manual/en/tutorial.forms.php

##### By the end of this task you should be able to understand -

1. The `<?php ?>` tags
2. The `echo` statement 
3. `strpos()`, `strupper()` library **functions**
4. If/Else in PHP
5. HTML  forms (action, method attributes) - [When to use GET or POST](http://stackoverflow.com/questions/46585/when-do-you-use-post-and-when-do-you-use-get)
6. Super globals in PHP
7. Handling data from form on the server based on the method/action attribute. (REQUEST)
8. `htmlspecialchars()` librabry function.
8. Sending a response back to the client.

## Task 6 - Data Types in PHP

Best place to start on Data Types would be to go through - http://php.net/manual/en/language.types.php

Our recommendation would be to cover atleast till the `NULL` data type and then to go through Type Juggling - http://php.net/manual/en/language.types.type-juggling.php

##### By the end of this task you should be able to understand -

1. Identify the various data types allowed by PHP.

## Task 7 - Variables in PHP

Read up on variables from here - http://php.net/manual/en/language.variables.basics.php  

You can skip the section **Vairable Variable**
For **Variables From External Sources** cover only the GET and POST section.

##### By the end of it, you should be familiar with - 

- Declaring variables and assigning them values.
- How scoping of variables works in PHP

## Task 8 - Constants in PHP 

Read here - http://php.net/manual/en/language.constants.php

##### By the end of it, you should be familiar with - 

- How to declare, access a constant
- Knowledge of some magic constants such as `__FILE__`, `__DIR__`, `__LINE__` etc.

## Task 9 - Let's build a shopping cart for a Supermarket.

The supermarket will currently have a predefined list of items, to which there is no possibility (for now) to add things.

You'll create a form with the following controls/labels - 

| Label | Control (For Quantity) | Price (As Label) |
|-------|------------------------|---------------------|
| Tooth Brush | Textbox | 40 |
| Tooth Paste | Textbox | 60 |
| Hand wash | Textbox | 55 |
| Cocunut Hair Oil | Textbox | 60 |
| Bathing Soap | Textbox | 25 |

Put a heading on top of your form, with a name for your supermarket. At the bottom of the form add a submit (text should be **Buy**) button. Ensure that the `action` and `method` attribute are set correctly. (Method should be POST)

Now in your PHP page, you've to calculate the total price (price * quantity) for each item and display it to the end user.

At the bottom you will also display a Total column that will be the sum of all the prices.

Your output should be a table of the following type - 

| Item | Quantity | Price | Total |
|----------------|------|------|-------|
| Tooth Brush | 3 | 40 | 120 |
| Bathing Soap | 3 | 25 | 75 |
| **Total** | | | 195 |

**Further Tips/Hints** -
- Ensure your text-boxes have the html `name` attribute. It's a common mistake to forget these.
- Ensure your form's method is `POST`
- Access form variables in PHP using `$_POST`
- Use constants to define the prices of various objects.
- Generate each row of the table (except for the header row) in a `for` loop
- Ideally your code to calculate and generate the table should be a function.

##### By the end of it, you should be familiar with - 

1. Access values from textboxes in an HTML page.
2. The `$_POST` variable
3. Writing specific focused functions.


## Task  10 : A slightly improved shopping cart.

OK, so we are comfortable working with text-boxes, it's time to move onto some other HTML controls.

1. We'll add a check-box at the bottom of our form (but above the submit button). The label of the check-box will be **Want a paper-bag?**
2. The price column will now become a drop-down that will contain different prices for different products. For example Tooth Paste might have three prices - 60, 55, 50. The user can select which **type** of toothpaste he wants. These values will be predefined and populated in the HTML.

##### By the end of it, you should be familiar with - 

1. Access values from checkboxes
2. Access values from dropdowns

## Task 11 : Saving the purchase details in the database for future use. (In progress)

Now what we want to do is save every purchase made into the database so that we can have an idea of what has been purchased since the beginning of time.



