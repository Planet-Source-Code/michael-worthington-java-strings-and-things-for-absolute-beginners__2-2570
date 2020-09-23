<div align="center">

## JAVA \- 'Strings and Things' for absolute beginners


</div>

### Description

the purpose of this tutorial is to get beginner java programmers familiar with the variable type String, as well as with a couple String functions. it includes a simple program that beginners can make, and it covers a lot of basics to understanding strings and how one can use them.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[michael worthington](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/michael-worthington.md)
**Level**          |Beginner
**User Rating**    |4.5 (18 globes from 4 users)
**Compatibility**  |Java \(JDK 1\.2\)
**Category**       |[String Manipulation](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/string-manipulation__2-60.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/michael-worthington-java-strings-and-things-for-absolute-beginners__2-2570/archive/master.zip)





### Source Code

```
<blockquote>
 <p><font face="Verdana, Arial, Helvetica, sans-serif" size="1"><br>
 </font></p>
 <hr>
 <p><font face="Verdana, Arial, Helvetica, sans-serif" size="1"><u>INTRO TO JAVA (PART 3) -
 WRITTEN BY: M.WORTHINGTON [01.02.02]</u><br>
<? $path="http://mixednuts.8bit-religion.com/java/counter.php?id=tutorialthree.txt" ; if (!nofile) {print "Error Reading Counter. Sorry." ; } else include( "$path"); ?> <br>
 <br>
 ...after checking out the first two <a
 href="http://mixednuts.8bit-religion.com/java.php?=main">tutorials you should</a> you
 should now be able to make a running program as well as mess around with numbers. now it
 is time to endulge ourselves in the world of strings.<br>
 <br>
 in our class StringsAndThings we will be using the variable type: String. the 's' must
 always be capitalized in the word 'String'. a String is any type of text. it can be
 letters, symbols, and even numbers. however, if the variable is defined as a String and it
 has a value of a number, it will not functino like a number, it will not function like an
 int or double. to explain, look at the following:<br>
 &nbsp; String a = &quot;1&quot;; //correct<br>
 &nbsp; String a = 1; //incorrect<br>
 &nbsp; int a = &quot;1&quot;; //incorrect<br>
 &nbsp; int a = 1; //correct<br>
 &nbsp; String b = &quot;2&quot;;<br>
 &nbsp; String c = a + b;<br>
 &nbsp;&nbsp; if you print out c, you would get 12 (1 and 2 is 12 in string format). c
 would not be 3 (1 + 2 = 3).<br>
 <br>
 a key thing to know about Strings is that each letter or character of the string has an
 index. the indexes of a string go from 0 to the length of the string minus one. for
 example:<br>
 &nbsp; String k = &quot;Funky Town&quot;;<br>
 &nbsp;&nbsp; Funky Town<br>
 &nbsp;&nbsp; 0123456789<br>
 The index of F is 0<br>
 The index of u is 1<br>
 The index of n is 2<br>
 The index of k is 3<br>
 The index of y is 4<br>
 The index of&nbsp;&nbsp;&nbsp; is 5<br>
 The index of T is 6<br>
 The index of o is 7<br>
 The index of w is 8<br>
 The index of n is 9<br>
 <br>
 The length of this string is 10, but as you can see, the last index is 9 (the length minus
 one). Always remember that the index starts at 0.<br>
 <br>
 in this program, StringsAndThings we will be using string variables and some of their
 functions. they are as follows:<br>
 .length() &lt;--- produces an integer of the length of the string<br>
 .substring(beginning position, ending position) &lt;---prints out a specified part of the
 string<br>
 .toUpperCase() &lt;---PUTS ALL OF THE CHARACTERS IN THE STRING TO UPPER CASE<br>
 .toLowerCase() &lt;---puts all of the characters in the string to lower case<br>
 <br>
 <u>OBJECTIVE</u> <br>
 to create, use, and manipulate Strings. this tutorial doesn't contain all of the useful
 functions that come along with Strings, but it does have the basics. i figured i'd get
 these out first for you to soak up, and i'll introduce others in another tutorial. <br>
 <br>
 <u>PROGRAM</u><br>
 <br>
 public class StringsAndThings<br>
 {<br>
 &nbsp; public static void main(String[] args)<br>
 &nbsp; {<br>
 &nbsp;&nbsp; String first = &quot;John&quot;;<br>
 &nbsp;&nbsp; String last = &quot;Doe&quot;;<br>
 &nbsp;&nbsp; String full = (first + &quot; &quot; + last);<br>
 &nbsp;&nbsp; System.out.println(&quot;first name: &quot; + first); // Line 1<br>
 &nbsp;&nbsp; System.out.println(&quot;last name: &quot; + last); // Line 2<br>
 &nbsp;&nbsp; System.out.println(&quot;full name: &quot; + full); // Line 3<br>
 &nbsp;&nbsp; //length<br>
 &nbsp;&nbsp; System.out.println(&quot;first name has &quot; + first.length() + &quot;
 characters&quot;); // Line 4<br>
 &nbsp;&nbsp; System.out.println(&quot;last name has &quot; + last.length() + &quot;
 characters&quot;); // Line 5<br>
 &nbsp;&nbsp; //substring<br>
 &nbsp;&nbsp; System.out.println(&quot;last, first: &quot; + full.substring(4,8) + &quot;,
 &quot; + full.substring(0,5)); //Line 6<br>
 &nbsp;&nbsp; System.out.println(&quot;last, first: &quot; + full.substring(4) + &quot;,
 &quot; + full.substring(0,5)); // Line 7<br>
 &nbsp;&nbsp; //upper, lower cases<br>
 &nbsp;&nbsp; System.out.println(&quot;first name: &quot; + first.toUpperCase()); // Line 8<br>
 &nbsp;&nbsp; System.out.println(&quot;first name: &quot; + first); // Line 9<br>
 &nbsp;&nbsp; first = first.toUpperCase();<br>
 &nbsp;&nbsp; System.out.println(&quot;first name: &quot; + first); // Line 10<br>
 &nbsp;&nbsp; System.out.println(&quot;first name: &quot; + first.toLowerCase()); // Line
 11<br>
 &nbsp;&nbsp; System.out.println(&quot;first name: &quot; + first); // Line 12<br>
 &nbsp;&nbsp; first = first.toLowerCase();<br>
 &nbsp;&nbsp; System.out.println(&quot;first name: &quot; + first); // Line 13<br>
 &nbsp; } //main<br>
 } //class</p>
 <p><font face="Verdana, Arial, Helvetica, sans-serif" size="1"><u>ABOUT THE PROGRAM</u><br>
 on each line of coding that is going to print something out is a comment that has an
 assigned number line. this is just so referring to each line will be easier to understand.<br>
 <br>
 <u>OUTPUT</u><br>
 be sure to compile the program and then run it. refer back to the <a
 href="http://mixednuts.8bit-religion.com/java.php?id=tutorial1">first tutorial</a> for
 instructions.</font></p>
 <p>the following is output from each line(minus the line reference) as you should have
 when you run the program:<br>
 <br>
 Line 1:&nbsp; first name: John<br>
 Line 2:&nbsp; last name: Doe<br>
 Line 3:&nbsp; full name: John Doe<br>
 Line 4:&nbsp; first name has 4 characters<br>
 Line 5:&nbsp; last name has 3 characters<br>
 Line 6:&nbsp; last, first: Doe, John<br>
 Line 7:&nbsp; last, first: Doe, John<br>
 Line 8:&nbsp; first name: JOHN<br>
 Line 9:&nbsp; first name: John<br>
 Line 10:&nbsp; first name: JOHN<br>
 Line 11:&nbsp; first name: john<br>
 Line 12:&nbsp; first name: JOHN<br>
 Line 13:&nbsp; first name: john<br>
 <br>
 <br>
 <u>EXPLANATION</u><br>
 first, i want to jump straight to the upper and lower case section. while lines 8 and 11
 printed out the first name in Upper and Lower Cases, respectively, they did not change
 what the variable itself contained. the contents of the variable do not change until after
 lines 9 and 12. lines 1 through 3 simply print out the contents of the variables. lines 4
 and 5 simply print out the length of the strings. lines 6 and 7 print out substrings. line
 6 prints out the characters at the 4th, 5th, 6th, and 7th indexes in the string, but not
 the 8th. the substring ends at the 8th index but does not include it. it then prints out the comma and the characters from 0 to 4, but not including the character with the index of 4. the only difference between lines 6 and 7 is that the first substring only has one number in the parenthesis. putting only one number in the substring parenthesis means 'print from this spot to the end of the string.' it is as simple as that. i suggest messing around with substrings until you completely have a grasp on them. they're not difficult,
 but simple mistakes with them will annoy you later down the road.<br>
 <br>
 if you're still having trouble with the program and understanding it, your best bet is
 to just mess around with it. change up the variables, variable types (include ints and
 doubles in the program), values, and functions; before running the program, try to
 predict what is going to be printed out.<br>
 <br>
 any other questions, hit up the <a href="http://mixednuts.8bit-religion.com/forum.php">message
 boards</a>. if you chat there you can easily go ahead of tutorials and learn more
 programming.<br>
 <br>
 please let me know what you think of this tutorial by going to the <a
 href="http://mixednuts.8bit-religion.com/forum.php">message boards</a> or the <a
 href="http://mixednuts.8bit-religion.com/contactpage.php">contact page</a> to submit your
 comments. thank you.<br>
 </font>
 <hr>
 <p>&nbsp;</p>
</blockquote>
```

