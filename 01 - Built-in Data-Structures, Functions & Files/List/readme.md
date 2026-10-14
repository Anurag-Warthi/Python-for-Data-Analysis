<h1>List</h1>

<pr>
Lists are used to store multiple items in a single variable.

Lists are one of 4 built-in data types in Python used to store collections of data, the other 3 are Tuple, Set, and Dictionary, all with different qualities and usage.

Lists are created using square brackets:
</pr>

<pre><code>
thislist = ["apple", "banana", "cherry"]
print(thislist)
</code></pre>

<p><strong>Output</strong><p>
<pre><code>
["apple", "banana", "cherry"]
</code></pre>

<hr>

<h2>List Items</h2>

<pr>
List items are ordered, changeable, and allow duplicate values.

List items are indexed, the first item has index [0], the second item has index [1] etc.
</pr>

<hr>

<h2>Ordered</h2>

<pr>
When we say that lists are ordered, it means that the items have a defined order, and that order will not change.

If you add new items to a list, the new items will be placed at the end of the list.
</pr>

<hr>

<h2>Changeable</h2>

<pr>
The list is changeable, meaning that we can change, add, and remove items in a list after it has been created.
</pr>

<hr>

<h2>Allow Duplicates</h2>

<pr>
Since lists are indexed, lists can have items with the same value.
</pr>

<pre><code>
thislist = ["apple", "banana", "cherry", "apple", "cherry"]
print(thislist)
</code></pre>

<p><strong>Output</strong><p>
<pre><code>
["apple", "banana", "cherry", "apple", "cherry"]
</code></pre>

<hr>

<h2>List Length</h2>

<pr>
To determine how many items a list has, use the len() function:
</pr>

<pre><code>
thislist = ["apple", "banana", "cherry"]
print(len(thislist))
</code></pre>

<p><strong>Output</strong><p>
<pre><code>
3
</code></pre>

<hr>

<h2>List Items - Data Types</h2>

