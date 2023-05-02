Download Link: https://assignmentchef.com/product/solved-cop3502-lab-10-recursion
<br>
<strong>Overview</strong>

This lab is designed to illustrate concepts and characteristics of recursion, including the difference between “regular recursion” and “tail recursion,” the use of base cases, the concept of the call stack, and arithmetic in return statements. You will write three different public methods and a private helper method in this lab. <strong>You must strictly follow the given method signatures and specifications.</strong>

<strong>Specification </strong>

You create a <strong>Factorial</strong> class which will implement several versions of a factorial calculation. The recursive definition for factorial is as follows:




Base Case:                               <strong>factorial(1) = 1</strong>

Recurrence Relation:              <strong>factorial(n) = n * factorial(n – 1)</strong>




<u>The factorial function is undefined for non-positive numbers (including zero)</u>; if a non-positive number is passed in, the function should throw an <strong>IllegalArgumentException</strong>.




The <strong>Factorial</strong> class should have the following methods:




<em>public static </em><em>long</em> <strong>pureRecursive</strong>(int n)

A purely recursive function that calculates the factorial of <strong>n</strong>. This function should call <u>only itself</u>.




<em>public static </em><em>long</em> <strong>tailRecursive</strong>(int n)

A kickoff method for tail recursion; it should call only the <strong>tail</strong>() method (see below).




<em>private static </em><em>long</em> <strong>tail</strong>(…)

A private method called by the tail recursion kickoff method. Students may select the parameters for this method, but it must be present and used. This method should only call itself, and only via tail recursion – i.e., <u>it</u> <u>should call itself on the last line with no other computation after the function call</u>.




<em>public static </em><em>long</em> <strong>iterative</strong>(int n)

An iterative version of the factorial calculation. This method should be an “unwound” version of the <strong>tailRecursive</strong>() method outlined above. It should not call itself or any other method but should instead using a looping structure to calculate the factorial.







<strong>Submissions </strong>

<strong>NOTE</strong>: Your output must match the example output *exactly*. If it does not, <strong><em>you will not receive full credit for your submission</em></strong>!







Files:                Factorial.java

Method:           Submit on Canvas

<strong>Sample Results (Public Methods) </strong>




<table width="338">

 <tbody>

  <tr>

   <td width="66"><strong>Param.</strong></td>

   <td width="272"><strong>Returns</strong></td>

  </tr>

  <tr>

   <td width="66">0</td>

   <td width="272"><em>throws </em><em>IllegalArgumentException</em></td>

  </tr>

  <tr>

   <td width="66">1</td>

   <td width="272">1</td>

  </tr>

  <tr>

   <td width="66">2</td>

   <td width="272">2</td>

  </tr>

  <tr>

   <td width="66">3</td>

   <td width="272">6</td>

  </tr>

  <tr>

   <td width="66">4</td>

   <td width="272">24</td>

  </tr>

  <tr>

   <td width="66">5</td>

   <td width="272">120</td>

  </tr>

  <tr>

   <td width="66">6</td>

   <td width="272">720</td>

  </tr>

  <tr>

   <td width="66">7</td>

   <td width="272">5,040</td>

  </tr>

  <tr>

   <td width="66">8</td>

   <td width="272">40,320</td>

  </tr>

  <tr>

   <td width="66">9</td>

   <td width="272">362,880</td>

  </tr>

  <tr>

   <td width="66">10</td>

   <td width="272">3,628,800</td>

  </tr>

  <tr>

   <td width="66">11</td>

   <td width="272">39,916,800</td>

  </tr>

  <tr>

   <td width="66">12</td>

   <td width="272">479,001,600</td>

  </tr>

  <tr>

   <td width="66">13</td>

   <td width="272">6,227,020,800</td>

  </tr>

  <tr>

   <td width="66">14</td>

   <td width="272">87,178,291,200</td>

  </tr>

  <tr>

   <td width="66">15</td>

   <td width="272">1,307,674,368,000</td>

  </tr>

 </tbody>

</table>





