===================
Python data storage types
===================

Python has five standard data types −

- Numbers
- String
- List
- Tuple
- Dictionary

We already used numbers(ints and floats), string and tuples. Now it is time to learn about Lists and Dictionaries.


Cute Wabbit
===================

A little girl goes into a pet show and asks for a wabbit. The shop keeper looks down at her, smiles and says:

"Would you like a lovely fluffy little white rabbit, or a cutesy wootesly little brown rabbit?"

"Actually", says the little girl, "I don't think my python would notice."

Now lest get back to learning :)

List
===================

Still we haven’t said anything about lists, as they do not differ much from the intuitive concept of
lists in the everyday life. We can easily think of lists in Python as we think of any other list (a
shopping list, a guest list, exam results etc.) written on a paper and numbered.

Let's start with a blank page by starting a new python interpreter:

    >>> L = []
    >>> L
    []

At any time we can check how many items we have saved on our list by using the function :func:`len`.

    >>> len(L)
    0

Let's make another list (which can have the same name or a different one):

    >>> L = ["Ala", "Ola", "Jacek"]
    >>> len(L)
    3

As in the case of tuples, consecutive elements of the list are separated by commas. Unlike tuples,
brackets ``[`` and ``]`` are obligatory.

To preview a particular position of an element on the list (remember that we count the positions from 0 ):

    >>> L[0]
    'Ala'
    >>> L[1]
    'Ola'
    >>> L[2]
    'Jacek'
    >>> L[3]
    Traceback (most recent call last):
     File "<stdin>", line 1, in <module>
    IndexError: list index out of range

We can also use the loop :keyword:`for`,to execute instructions for every element of the list:

    >>> for name in L:
    ...     print("Name:", name)
    ...
    Name: Ala
    Name: Ola
    Name: Jacek

In the same way, we can print the first part of our half of the Christmas tree:

    >>> lst = [1, 2, 3]
    >>> for n in lst:
    ...     print("*"*n)
    ...
    *
    **
    ***

Well, unfortunately we still have to type the entire contents of the list. This problem can be solved
by the function :func:`range`. Check ``help(range)``
for the full story, or check these quick examples:


    >>> list(range(2, 5, 1))
    [2, 3, 4]
    >>> list(range(1, 11, 2))
    [1, 3, 5, 7, 9]
    >>> list(range(1, 11))
    [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
    >>> list(range(1, 2))
    [1]
    >>> list(range(2))
    [0, 1]

Dictionary
===================
