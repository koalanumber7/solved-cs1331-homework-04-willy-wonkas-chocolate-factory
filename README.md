Download Link: https://assignmentchef.com/product/solved-cs1331-homework-04-willy-wonkas-chocolate-factory
<br>



<strong> </strong>

<h1>Problem Description</h1>

It is 1970 in Munich, Germany and you just found a golden ticket in a Wonka Bar. Elated for a chocolatey change of pace from your usual vocation as a chimney sweep, you grab your chaperone and head to Willy Wonka’s Chocolate Factory. You and and the four other winners sign contracts before heading into the fabled factory. Unfortunately for you, 10 minutes in you get sucked into a chocolate whirlpool and eventually you find yourself unceremoniously fished out by some oompa loompas. When you regain consciousness you realize you’re chained to a metal desk with only a laptop, a copy of <em>Head First Java Edition 2 </em>and a pile of stale saltine crackers. Turns out that in the fine print of your contract, font size 2 to be exact, it stated that any failure to complete the tour would result in your immediate and mandatory employment in the Wonka IT department for the fair wage of 6 saltines an hour.

Your first task will be to create a class that represents a simple rectuangular chocolate bar.

<h1>Solution Description</h1>

Your solution will consist of one Java class: Bar.java.

This Bar class should be flexible and will be used to represent Wonka Bars of various flavors (even those that haven’t been created yet) and sizes. It will also provide important methods that will print specifications of the bar to be used by other programmers and oompa loompas.

The Bar class should contain of the following fields:

<ul>

 <li>private String chocolateType. This will contain a String of any case that describes the chocolate bar’s flavor. <em>Some </em>possible values include: <strong>“milk”, “Dark”, “toffee”, or “Cookies’n’Cream”</strong>.</li>

 <li>private int barLength. This will contain the length of the bar as an integer.</li>

 <li>private int barWidth. This will contain the width of the bar as an integer.</li>

</ul>

The Bar class should contain the following methods:

<ul>

 <li>public int getPerimeter() that returns the the perimeter of the bar as an integer.</li>

 <li>public int getArea() that returns the area of the bar as an integer.</li>

 <li>public boolean isSquare() that returns True only if the bar of chocolate is a square.</li>

 <li>public double calculateCost(double chocolateCost, double trimCost) This method returns the cost of making this bar given the cost per unit area of chocolate and the cost of the trim that will go around the bar’s perimeter.</li>

</ul>

To be specific, this method should calculate and return the following: <strong>area * chocolateCost + perimeter</strong>

<strong>* trimCost</strong>

<ul>

 <li>public String getDetails() This method should return a String that describes the bar in the following format: <strong>“</strong><strong>Length by </strong><strong>Width bar of </strong><strong>chocolateType chocolate”</strong>. However, if the chocolate bar is a square, this method should return the following instead: <strong>“Square </strong><strong>getArea() piece bar of </strong><strong>chocolateType chocolate”</strong></li>

 <li>public void drawBar() This should print out a text drawing of the chocolate bar with the correct dimensions using the capitalized first letter of the chocolateType. For example, the following should be the console output if called on a 6 (length) by 4 (width) “milk” chocolate bar:</li>

</ul>

MMMM

MMMM

MMMM

MMMM

MMMM

MMMM

Note: The x-dimension is the width, and the y-dimension is the length.

Finally, create the following <strong>constructor </strong>that initializes fields chocolateType, barLength, and barWidth respectively:

<ul>

 <li>public Bar(String chocolateType, int barLength, int barWidth)</li>

</ul>

You are <strong>required </strong>to use the “this” keyword when referencing instance variables in your constructor.

<h1>Testing</h1>

We encourage you to write your own tests for Bar.java. Create a seperate Test class with a main() method and instantiate and inspect various instances of the Bar class.

<h1>Rubric</h1>

<ul>

 <li>[18] <strong>Fields</strong>

  <ul>

   <li>[18] chocolateType, barLength, barWidth</li>

  </ul></li>

</ul>

∗ [6] Return types

∗ [6] Access modifiers

∗ [6] Names

<ul>

 <li>[82] <strong>Methods</strong>

  <ul>

   <li>[30] getPerimeter, getArea, isSquare</li>

  </ul></li>

</ul>

∗ [6] Method signatures

∗ [6] Return types

∗ [6] Access modifiers

∗ [12] Correct output

<ul>

 <li>[13] calculateCost</li>

</ul>

∗ [4] Method signature

∗ [2] Return type

∗ [2] Access modifier

∗ [5] Correct output

<ul>

 <li>[14] getDetails</li>

</ul>

∗ [2] Method signature

∗ [2] Return type

∗ [2] Access modifier

∗ [8] Correct output

<ul>

 <li>[14] drawBar</li>

</ul>

∗ [2] Method signatures

∗ [2] Return types

∗ [2] Access modifier

∗ [8] Correct output

<ul>

 <li>[11] <strong>constructor</strong></li>

</ul>

∗ [6] Constructor signature, access modifier

∗ [2] Uses “this” keyword

∗ [3] Correctly initializes fields




<h1>Javadocs</h1>

For this assignment, you will be commenting your code with Javadocs. Javadocs are a clean and useful way to document your code’s functionality. For more information on what Javadocs are and why they are awesome, the <a href="http://www.oracle.com/technetwork/java/javase/documentation/index-137868.html">online overview</a> for them is extremely detailed and helpful.

You can generate the javadocs for your code using the command below, which will put all the files into a folder called javadoc:

$ javadoc *.java -d javadoc

The relevant tags that you need to include are @author, @version, @param, and @return. Here is an example of a properly Javadoc’d class:

<table width="632">

 <tbody>

  <tr>

   <td width="632"><strong>import </strong>java.util.Scanner;<em>/**</em>* This class represents a Dog object<em>.</em>* <strong>@author </strong>George P<em>. </em>Burdell* <strong>@version </strong><em>1.0</em><em>*/ </em><strong>public class </strong>Dog {<em>/**</em>* Creates an awesome dog <em>(</em>NOT a dawg<em>!)</em><em>*/ </em><strong>public </strong>Dog() { …}<em>/**</em>* This method takes in two ints and returns their sum* <strong>@param a </strong>first number* <strong>@param b </strong>second number <em>* </em><strong>@return </strong>sum of a and b<em>*/ </em><strong>public </strong>int add(int a, int b) {…}}</td>

  </tr>

 </tbody>

</table>

A more thorough tutorial for Javadocs can be found <a href="https://cs1331.gitlab.io/cs1331-style-guide.html">here</a>.

Take note of a few things:

<ol>

 <li>Javadocs are begun with /** and ended with */.</li>

 <li>Every class you write must be Javadoc’d and the @author and @verion tag included. The comments for a class should start with a brief description of the role of the class in your program.</li>

 <li>Every non-private method you write must be Javadoc’d and the @param tag included for every method parameter. The format for an @param tag is @param &lt;name of parameter as written in method header&gt; &lt;description of parameter&gt;. If the method has a non-void return type, include the @return tag which should have a simple description of what the method returns, semantically.</li>

</ol>

<ul>

 <li></li>

</ul>