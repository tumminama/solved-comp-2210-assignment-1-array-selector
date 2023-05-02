Download Link: https://assignmentchef.com/product/solved-comp-2210-assignment-1-array-selector
<br>
<h1></h1>

This assignment focuses on implementing the methods of a class much like java.util.Arrays. The Selector.java file defines a class with static methods designed to provide useful functionality on arrays. Each method of Selector is very clearly specified, is independent of the other methods in the class, and is designed to provide relatively simple functionality. So, this is a great context for practicing what we are discussing in lecture – systematic, disciplined development and test-based verification.

The Selector class

You must correctly implement all the method bodies of the provided Selector class. Your implementation must adhere <em>exactly </em>to the API of the Selector class, as described in the provided source code comments and as described below.

<strong>public final class </strong><strong>Selector </strong>{ <strong>public static </strong><strong>int </strong>min(<strong>int</strong>[] a) <strong>public static </strong><strong>int </strong>max(<strong>int</strong>[] a) <strong>public static </strong><strong>int </strong>kmin(<strong>int</strong>[] a, <strong>int </strong>k) <strong>public static </strong><strong>int </strong>kmax(<strong>int</strong>[] a, <strong>int </strong>k) <strong>public static </strong><strong>int</strong>[] range(<strong>int</strong>[] a, <strong>int </strong>low, <strong>int </strong>high) <strong>public static </strong><strong>int </strong>ceiling(<strong>int</strong>[] a, <strong>int </strong>key) <strong>public static </strong><strong>int </strong>floor(<strong>int</strong>[] a, <strong>int </strong>key)

}

<strong>The min method.</strong>

This method selects the minimum value from a given array. If the array is null or has zero length, this method throws an IllegalArgumentException. The array is not changed by this method.

<em>Examples:</em>

<table width="174">

 <tbody>

  <tr>

   <td width="126">a[ ]</td>

   <td width="47">min(a)</td>

  </tr>

  <tr>

   <td width="126">[2, 8, 7, 3, 4]</td>

   <td width="47">2</td>

  </tr>

  <tr>

   <td width="126">[5, 9, 1, 7, 3]</td>

   <td width="47">1</td>

  </tr>

  <tr>

   <td width="126">[8, 7, 6, 5, 4]</td>

   <td width="47">4</td>

  </tr>

  <tr>

   <td width="126">[2, 8, 8, 7, 3, 3, 4]</td>

   <td width="47">2</td>

  </tr>

 </tbody>

</table>

<strong>The max method.</strong>

This method selects the maximum value from a given array. If the array is null or has zero length, this method throws an IllegalArgumentException. The array is not changed by this method.

1

<em>COMP 2210 Assignment Examples:</em>

<table width="176">

 <tbody>

  <tr>

   <td width="126">a[ ]</td>

   <td width="50">max(a)</td>

  </tr>

  <tr>

   <td width="126">[2, 8, 7, 3, 4]</td>

   <td width="50">8</td>

  </tr>

  <tr>

   <td width="126">[5, 9, 1, 7, 3]</td>

   <td width="50">9</td>

  </tr>

  <tr>

   <td width="126">[8, 7, 6, 5, 4]</td>

   <td width="50">8</td>

  </tr>

  <tr>

   <td width="126">[2, 8, 8, 7, 3, 3, 4]</td>

   <td width="50">8</td>

  </tr>

 </tbody>

</table>

<strong>The kmin method.</strong>

This method selects the <em>k<sup>th </sup></em>minimum value from a given array. A value is the <em>k<sup>th </sup></em>minimum if there are exactly <em>k − </em>1 values less than it in the array. If the array is null, has zero length, or if there is no <em>k<sup>th </sup></em>minimum value, this method throws an IllegalArgumentException. Note that there is no <em>k<sup>th </sup></em>minimum value if <em>k </em>is less than 1, <em>k </em>is greater than the number of elements in the array, or if <em>k </em>is greater than the number of distinct values in the array. The array is not changed by this method.

<em>Examples:</em>

<table width="219">

 <tbody>

  <tr>

   <td width="126">a[ ]</td>

   <td width="23">k</td>

   <td width="69">kmin(a, k)</td>

  </tr>

  <tr>

   <td width="126">[2, 8, 7, 3, 4]</td>

   <td width="23">1</td>

   <td width="69">2</td>

  </tr>

  <tr>

   <td width="126">[5, 9, 1, 7, 3]</td>

   <td width="23">3</td>

   <td width="69">5</td>

  </tr>

  <tr>

   <td width="126">[8, 7, 6, 5, 4]</td>

   <td width="23">5</td>

   <td width="69">8</td>

  </tr>

  <tr>

   <td width="126">[2, 8, 8, 7, 3, 3, 4]</td>

   <td width="23">3</td>

   <td width="69">4</td>

  </tr>

 </tbody>

</table>

<strong>The kmax method.</strong>

This method selects the <em>k<sup>th </sup></em>maximum value from a given array. A value is the <em>k<sup>th </sup></em>maximum if there are exactly <em>k − </em>1 values greater than it in the array. If the array is null, has zero length, or if there is no <em>k<sup>th </sup></em>maximum value, this method throws an IllegalArgumentException. Note that there is no <em>k<sup>th </sup></em>maximum value if <em>k </em>is less than 1, <em>k </em>is greater than the number of elements in the array, or if <em>k </em>is greater than the number of distinct values in the array. The array is not changed by this method.

<em>Examples:</em>

<table width="221">

 <tbody>

  <tr>

   <td width="126">a[ ]</td>

   <td width="23">k</td>

   <td width="72">kmax(a, k)</td>

  </tr>

  <tr>

   <td width="126">[2, 8, 7, 3, 4]</td>

   <td width="23">1</td>

   <td width="72">8</td>

  </tr>

  <tr>

   <td width="126">[5, 9, 1, 7, 3]</td>

   <td width="23">3</td>

   <td width="72">5</td>

  </tr>

  <tr>

   <td width="126">[8, 7, 6, 5, 4]</td>

   <td width="23">5</td>

   <td width="72">4</td>

  </tr>

  <tr>

   <td width="126">[2, 8, 8, 7, 3, 3, 4]</td>

   <td width="23">3</td>

   <td width="72">4</td>

  </tr>

 </tbody>

</table>

<strong>The range method.</strong>

This method returns an array of all values <em>i </em>from a given array such that <em>low ≤ i ≤ high</em>, including duplicate values. (Note that <em>low </em>and <em>high </em>do not have to be actual values in the given array, and the order of the resulting values is irrelevant.) The length of the returned array is the same as the number of values <em>i </em>that meet the criterion. If there are no values <em>i </em>that meet the criterion, this method returns a zero-length array. If the given array is null or has zero length, this method throws an IllegalArgumentException. The given array is not changed by this method.

<em>Examples:</em>

<em>Page 2 of 3</em>

<em>COMP 2210 Assignment</em>

<table width="321">

 <tbody>

  <tr>

   <td width="126">a[ ]</td>

   <td width="35">low</td>

   <td width="41">high</td>

   <td width="118">range(a, low, high)</td>

  </tr>

  <tr>

   <td width="126">[2, 8, 7, 3, 4]</td>

   <td width="35">1</td>

   <td width="41">5</td>

   <td width="118">[2, 3, 4]</td>

  </tr>

  <tr>

   <td width="126">[5, 9, 1, 7, 3]</td>

   <td width="35">3</td>

   <td width="41">5</td>

   <td width="118">[3, 5]</td>

  </tr>

  <tr>

   <td width="126">[8, 7, 6, 5, 4]</td>

   <td width="35">4</td>

   <td width="41">8</td>

   <td width="118">[8, 7, 6, 5, 4]</td>

  </tr>

  <tr>

   <td width="126">[2, 8, 8, 7, 3, 3, 4]</td>

   <td width="35">3</td>

   <td width="41">7</td>

   <td width="118">[7, 3, 3, 4]</td>

  </tr>

 </tbody>

</table>

<strong>The ceiling method.</strong>

This method returns the smallest value <em>i </em>in a given array such that <em>i ≥ key</em>. (Note that <em>key </em>does not have to be an actual value in the given array.) If the given array is null or has zero length, or if there is no qualifying value <em>i</em>, this method returns an IllegalArgumentException. The given array is not changed by this method.

<em>Examples:</em>

<table width="252">

 <tbody>

  <tr>

   <td width="126">a[ ]</td>

   <td width="35">key</td>

   <td width="90">ceiling(a, key)</td>

  </tr>

  <tr>

   <td width="126">[2, 8, 7, 3, 4]</td>

   <td width="35">1</td>

   <td width="90">2</td>

  </tr>

  <tr>

   <td width="126">[5, 9, 1, 7, 3]</td>

   <td width="35">7</td>

   <td width="90">7</td>

  </tr>

  <tr>

   <td width="126">[8, 7, 6, 5, 4]</td>

   <td width="35">0</td>

   <td width="90">4</td>

  </tr>

  <tr>

   <td width="126">[2, 8, 8, 7, 3, 3, 4]</td>

   <td width="35">5</td>

   <td width="90">7</td>

  </tr>

 </tbody>

</table>

<strong>The floor method.</strong>

This method returns the largest value <em>i </em>in a given array such that <em>i ≤ key</em>. (Note that <em>key </em>does not have to be an actual value in the given array.) If the given array is null or has zero length, or if there is no qualifying value <em>i</em>, this method returns an IllegalArgumentException. The given array is not changed by this method.

<em>Examples:</em>

<table width="241">

 <tbody>

  <tr>

   <td width="126">a[ ]</td>

   <td width="35">key</td>

   <td width="79">floor(a, key)</td>

  </tr>

  <tr>

   <td width="126">[2, 8, 7, 3, 4]</td>

   <td width="35">6</td>

   <td width="79">4</td>

  </tr>

  <tr>

   <td width="126">[5, 9, 1, 7, 3]</td>

   <td width="35">1</td>

   <td width="79">1</td>

  </tr>

  <tr>

   <td width="126">[8, 7, 6, 5, 4]</td>

   <td width="35">9</td>

   <td width="79">8</td>

  </tr>

  <tr>

   <td width="126">[2, 8, 8, 7, 3, 3, 4]</td>

   <td width="35">5</td>

   <td width="79">4</td>

  </tr>

 </tbody>

</table>

<h1>Notes and other requirements</h1>

Here are more specific requirements, notes, and suggestions.

<ul>

 <li>Read this handout carefully. Read the provided source code carefully. Ask questions on Piazza. Start early and be proactive.</li>

 <li>The constructor has been completed for you and must not be changed in any way.</li>

 <li>You may add any number of private methods that you like, but you may not add any public method or constructor, nor may you change the signature of any public method or constructor.</li>

 <li>You must not add any fields, either public or private, to the Selector class.</li>

 <li>You are allowed to use sorting <strong>only </strong>as part of your solution to kmin and kmax. You are not required to use sorting, but you are allowed to do so for these two methods <strong>only</strong>. If you use sorting, I strongly recommend the use of the Arrays.sort method.</li>

 <li>You must not import anything other than java.util.Arrays. If you do not use java.util.Arrays, then delete its import statement.</li>

</ul>

<em>Page 3 of 3</em>