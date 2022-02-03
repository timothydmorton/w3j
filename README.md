# w3j


Installation:  `python setup.py install`

This will install the `w3j` package.  To access the SLATEC function
`drc3jm`, just do `from w3j import drc3jm`.  Example usage is as follows:

    >>> from w3j import drc3jm
    >>> import numpy as np
    >>> result = np.empty(5, dtype=float)
    >>> drc3jm(2,2,2,0,-2,2, result, 0)
    >>> result
    	array([ 0.23904572,  0.11952286, -0.23904572,  0.11952286,  0.23904572])

The first four arguments `(l1, l2, l3, m1)` are really the only optional
ones; the fifth and sixth are always `-l2` and `l2`.  The last argument
just needs to be any integer; doesn't matter what.
