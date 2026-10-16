<h1>NumPy Introduction</h1>

<h2>What is NumPy?</h2>

<pr>
NumPy is a Python library used for working with arrays.

NumPy was created in 2005 by Travis Oliphant. It is an open source project and you can use it freely.

NumPy, short for Numerical Python, is one of the most important foundational pack‐
ages for numerical computing in Python. Many computational packages providing
scientific functionality use NumPy’s array objects as one of the standard interface
lingua francas for data exchange.

</pr>

<p>Here are some of the things you will find in NumPy:</p>

<ul>
    <li>ndarray, an efficient multidimensional array providing fast array-oriented arithmetic operations and flexible broadcasting capabilities.</li>
    <li>Mathematical functions for fast operations on entire arrays of data without having to write loops</li>
    <li>Tools for reading/writing array data to disk and working with memory-mapped files</li>
    <li>Linear algebra, random number generation, and Fourier transform capabilities</li>
</ul>

<hr>

<h2>Why use NumPy?</h2>

<pr>
In Python we have lists that serve the purpose of arrays, but they are slow to process.

NumPy aims to provide an array object that is up to 50x faster than traditional Python lists.

The array object in NumPy is called ndarray, it provides a lot of supporting functions that make working with ndarray very easy.

Arrays are very frequently used in data science, where speed and resources are very important.
</pr>

<hr>

<h2>Why is NumPy Faster Than Lists?</h2>

<pr>
NumPy arrays are stored at one continuous place in memory unlike lists, so processes can access and manipulate them very efficiently.

This behavior is called locality of reference in computer science.

This is the main reason why NumPy is faster than lists. Also it is optimized to work with latest CPU architectures.
</pr>

<hr>

<h2>Which Language is NumPy written in?</h2>

<pr>
NumPy is a Python library and is written partially in Python, but most of the parts that require fast computation are written in C or C++.
</pr>

<hr>

<h1>NumPy Getting Started</h1>

<h2>Installation of NumPy</h2>

<pr>
If you have Python and PIP installed on a system, then installation of NumPy is very easy.
</pr>


<p>Install it using this command:<p>

<pre><code>
C:\Users\Your Name>pip install numpy
</code></pre>

<hr>

<h2>Import Numpy</h2>

<pr>
Once NumPy is installed, import it in your applications by adding the import keyword:
</pr>

<pre><code>
import numpy
</code></pre>

<p>Now NumPy is imported and ready to use.</p>

<p>Example:</p>

<pre><code>
import numpy

arr = numpy.array([1, 2, 3, 4, 5])

print(arr)
</code></pre>

<p><strong>Output</strong></p>
<pre><code>
[1  2  3  4  5]
</code></pre>

<hr>

<h2>NumPy as np</h2>

<pr>
NumPy is usually imported under the np alias.
</pr>

<p><strong>alias: In Python alias are an alternate name for referring to the same thing.</strong></p>

<pr>
Create an alias with the as keyword while importing:
</pr>

<pre><code>
import numpy as np
</code></pre>

<p>Now the NumPy package can be referred to as np instead of numpy.</p>

<p>Example:</p>

<pre><code>
import numpy as np

arr = np.array([1, 2, 3, 4, 5])

print(arr)
</code></pre>

<p><strong>Output</strong></p>
<pre><code>
[1  2  3  4  5]
</code></pre>

<hr>

<h2>Checking Numpy Version</h2>

<p>The version string is stored under __version__ attribute.</p>

<pre><code>
import numpy as np
print(np.__version__)
</code></pre>

<p><strong>Output</strong></p>
<pre><code>
2.4.6
</code></pre>

<hr>

<h1>NumPy Creating Arrays</h1>

<h2>Create a NumPy ndarray Object</h2>

<pr>
NumPy is used to work with arrays. The array object in NumPy is called ndarray.

We can create a NumPy ndarray object by using the array() function.
</pr>

<pre><code>
import numpy as np
arr = np.array([1, 2, 3, 4, 5])
print(arr)
print(type(arr))
</code></pre>

<p><strong>Output</strong><p>
<pre><code>
[1 2 3 4 5]
< class 'numpy.ndarray'>
</code></pre>


<pr>
To create an ndarray, we can pass a list, tuple or any array-like object into the array() method, and it will be converted into an ndarray:
</pr>

<p>Using a tuple to create a numpy array:</p>

<pre><code>
import numpy as np

arr = np.array((1, 2, 3, 4, 5))

print(arr)
</code></pre>

<p><strong>Output</strong></p>
<pre><code>
[1  2  3  4  5]
</code></pre>

<hr>

<h2>Dimensions in Arrays</h2>

<p>A dimension in arrays is one level of array depth (nested arrays).</p>

<p><strong>nested array: are arrays that have arrays as their elements.</strong></p>

<hr>

<h2>0-D Array</h2>

<pr>
0-D arrays, or Scalars, are the elements in an array. Each value in an array is a 0-D array.
</pr>

<pre><code>
arr = np.array(42)
print(arr)
</code></pre>

<p><strong>Output</strong></p>
<pre><code>
42
</code></pre>

<hr>

<h2>1-D Arrays</h2>

<pr>
An array that has 0-D arrays as its elements is called uni-dimensional or 1-D array.

These are the most common and basic arrays.
</pr>

<p>Creating a 1-D array containing the values 1,2,3,4,5:</p>

<pre><code>
arr = np.array([1, 2, 3, 4, 5])
print(arr)
</code></pre>

<hr>

<h2>2-D Arrays</h2>

<pr>
An array that has 1-D arrays as its elements is called a 2-D array.

These are often used to represent matrix or 2nd order tensors.
</pr>

<p>Create a 2-D array containing two arrays with values 1,2,3 and 4,5,6</p>

<pre><code>
arr = np.array([[1, 2, 3], [4, 5, 6]])
print(arr)
</code></pre>

<p><strong>Output</strong></p>
<pre><code>
[[1 2 3]
 [4 5 6]]
</code></pre>

<hr>

<h2>3-D Arrays</h2>

<pr>
An array that has 2-D arrays (matrices) as its elements is called 3-D array.

These are often used to represent a 3rd order tensor.
</pr>

<p>Create a 3-D array with two 2-D arrays, both containing two arrays with the values 1,2,3 and 4,5,6:</p>

<pre><code>
arr = np.array([[[1, 2, 3], [4, 5, 6]], [[1, 2, 3], [4, 5, 6]]])

print(arr)
</code></pre>

<p><strong>Output</strong></p>
<pre><code>
[[[1 2 3]
  [4 5 6]]

 [[1 2 3]
  [4 5 6]]]
</code></pre>

<hr>

<h2>Check Number of Dimensions?</h2>

<pr>
NumPy Arrays provides the ndim attribute that returns an integer that tells us how many dimensions the array have.
</pr>

<pre><code>
a = np.array(42)
b = np.array([1, 2, 3, 4, 5])
c = np.array([[1, 2, 3], [4, 5, 6]])
d = np.array([[[1, 2, 3], [4, 5, 6]], [[1, 2, 3], [4, 5, 6]]])

print(a.ndim)
print(b.ndim)
print(c.ndim)
print(d.ndim)
</code></pre>

<p><strong>Output</strong></p>
<pre><code>
0
1
2
3
</code></pre>

<hr>

<h2>Higher Dimension Arrays</h2>

<pr>
An array can have any number of dimensions.

When the array is created, you can define the number of dimensions by using the ndmin argument.
</pr>

<pre><code>
arr = np.array([1, 2, 3, 4], ndmin=5)

print(arr)
print('number of dimensions :', arr.ndim)
</code></pre>

<p><strong>Output</strong></p>
<pre><code>
[[[[[1 2 3 4]]]]]
number of dimensions : 5
</code></pre>

<hr>

<h1>NumPy Array Indexing</h1>

<h2>Access Array Elements</h2>

<pr>
Array indexing is the same as accessing an array element.

You can access an array element by referring to its index number.

The indexes in NumPy arrays start with 0, meaning that the first element has index 0, and the second has index 1 etc.
</pr>

<pre><code>
arr = np.array([1, 2, 3, 4])

print(arr[0])
print(arr[1])
print(arr[2])
print(arr[3])
</code></pre>

<p><strong>Output</strong></p>
<pre><code>
1
2
3
4
</code></pre>


<p><strong>Example:</strong></p>

<p>Get third and fourth elements from the following array and add them.</p>

<pre><code>
arr = np.array([1, 2, 3, 4])

print(arr[2] + arr[3])
</code></pre>

<p><strong>Output</strong></p>
<pre><code>
7
</code></pre>

<hr>

<h2>Access 2-D Arrays</h2>

<pr>
To access elements from 2-D arrays we can use comma separated integers representing the dimension and the index of the element.

Think of 2-D arrays like a table with rows and columns, where the dimension represents the row and the index represents the column.
</pr>

<p><strong>Example</strong></p>

<p>Access the element on the first row, second column:</p>

<pre><code>
arr = np.array([[1,2,3,4,5], [6,7,8,9,10]])

print('2nd element on 1st row: ', arr[0, 1])
</code></pre>

<p><strong>Output</strong></p>
<pre><code>
2
</code></pre>

<hr>

<p><strong>Example 2</strong></p>

<p>Access the element on the 2nd row, 5th column:</p>

<pre><code>
arr = np.array([[1,2,3,4,5], [6,7,8,9,10]])

print('5th element on 2nd row: ', arr[1, 4])
</code></pre>

<p><strong>Output</strong></p>
<pre><code>
10
</code></pre>

<hr>

<h2>Access 3-D Arrays</h2>

<pr>
To access elements from 3-D arrays we can use comma separated integers representing the dimensions and the index of the element.
</pr>

<p><strong>Example</strong></p>

<p>Access the third element of the second array of the first array:</p>

<pre><code>
arr = np.array([[[1, 2, 3], [4, 5, 6]], [[7, 8, 9], [10, 11, 12]]])

print(arr)
print(arr[0, 1, 2])
</code></pre>

<p><strong>Output</strong></p>
<pre><code>
[[[ 1  2  3]
  [ 4  5  6]]

 [[ 7  8  9]
  [10 11 12]]]
6
</code></pre>

<p><strong>Example Explained</strong></p>

<pre>
arr[0, 1, 2] prints the value 6.

And this is why:

The first number represents the first dimension, which contains two arrays:
[[1, 2, 3], [4, 5, 6]]
and:
[[7, 8, 9], [10, 11, 12]]
Since we selected 0, we are left with the first array:
[[1, 2, 3], [4, 5, 6]]

The second number represents the second dimension, which also contains two arrays:
[1, 2, 3]
and:
[4, 5, 6]
Since we selected 1, we are left with the second array:
[4, 5, 6]

The third number represents the third dimension, which contains three values:
4
5
6
Since we selected 2, we end up with the third value:
6
</pre>

<hr>

<h2>Negative Indexing</h2>

<pr>
Use negative indexing to access an array from the end.
</pr>

<p><strong>Example</strong></p>
<p>Print the last element from the 2nd dim.</p>

<pre><code>
arr = np.array([[1,2,3,4,5], [6,7,8,9,10]])

print('Last element from 2nd dim: ', arr[1, -1])
</code></pre>

<p><strong>Output</strong></p>
<pre><code>
Last element from 2nd dim:  10
</code></pre>

<hr>