# Introductiong to Computer Science - Fall 2017

# Lab 9 - One way or another, you're going to pay

**Functions as abstractions:** this lab gives you a chance to practice defining and calling a function. In this lab, you will write a function that computes how much a payment is on a loan, given the term, interest rate, and initial loan amount. Much of the web page is already crafted for you and is attached to this repository.

**Discussion:** In what follows, notice how things are named so that we can use variables.

The formula for computing the monthly payments on a loan of P dollars at a given annual percentage rate(APR) for N months is:

![img/pmt.gif]

where `R = APR/1200`, the monthly interest rate in computational form. The monthly payment assumes that interest is compounded monthly on the unpaid balance. Consider the following example in which $1000 is borrowed at 5.1% annual interest rate for 12 months.

`P = 1000 APR`, `APR = 5.1`, `N = 12`

`R = APR / 1200 = 5.1 / 1200 = .00425`

![img/ex.gif]

which is $86.65 when rounded to the nearest penny. You can check the calculations by using a calculator. Your calculations may produce a number that is slightly different than 85.65 due to round-off error in the calculations.

**The Payment Function:** Code a JavaScript function named `payment()` that will calculate the monthly payment for a loan using the formula described above. The function must have 3 parameters: the principal amount of the loan, the annual percentage rate of interest, and the number of months payments will be made. The function must return the payment amount. All variables used in the function must be declared in the function using `var` statements.

Here are few hints. Look at the source code for the [diagonals program](http://itech190.erickuha.com/abstraction/diagonals.html) (courtesy Marty J. Wolf). This is a great opportunity to practice the problem solving technique of dividing the problem into subproblems. Look for ways to compute small parts of the formula above. To raise a number to a power, use the standard JavaScript function `Math.pow()`. For example, `Math.pow(2.5,8)` will calculate and return the value of 2.5<sup>8</sup> = 1525.87890625. In general, `Math.pow(x,k)` calculates and returns x<sup>k</sup> (x raised to the k<sup>th</sup> power).

Your `payment()` function should be inserted into the `loan.html` file at the place indicated by a JavaScript comment that appears in a heading script. Remove the comment and put your function in its place. You also need to un-comment the statements in the `CalculatePayment()` function that displays the payment amount and total interest. That is remove the "/*" and the "*/".

Once you have completed the assignment, push your edited copy of the repository back to your master branch.
