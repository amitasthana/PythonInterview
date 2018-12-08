# PythonInterview
Common and Advanced Python Interview Questions and Answers

### Topic:- Mutable / Immutable 

Objects of built-in types like (int, float, bool, str, tuple, unicode) are immutable
Objects of built-in types like (list, set, dict) are mutable. Custom classes are generally mutable

### Question:- Numbers as key in dictionary python? 

Dictionaries are indexed by keys, which can be any immutable type; strings and numbers can always be keys. Tuples can be used as keys if they contain only strings, numbers, or tuples; if a tuple contains any mutable object either directly or indirectly, it cannot be used as a key. You can’t use lists as keys, since lists can be modified in place using index assignments, slice assignments, or methods like append() and extend().

`python

dict = {1:0, 2:1}
>>> dict[1]
0
`

### Topic:- Class based views

Class-based views provide an alternative way to implement views as Python objects instead of functions. They do not replace function-based views, but have certain differences and advantages when compared to function-based views:

Organization of code related to specific HTTP methods (GET, POST, etc.) can be addressed by separate methods instead of conditional branching.
Object oriented techniques such as mixins (multiple inheritance) can be used to factor code into reusable components.

