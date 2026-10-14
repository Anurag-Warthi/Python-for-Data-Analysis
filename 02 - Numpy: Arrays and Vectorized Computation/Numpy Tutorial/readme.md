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

