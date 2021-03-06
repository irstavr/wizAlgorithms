# Symbol Table

This is an implementation of a symbol table data structure. It is designed as a 'Spaghetti stack' and depends on a generic hash
table, in which keys are strings and values can be of whatever value, elements of the same hashing value are stored into collision lists on every table's element. <br>

### Structures:
- Hash Table
- Collision List

### Spaghetti Stack:

A spaghetti stack is an N-ary tree data structure in which child nodes <br>
have pointers to the parent nodes (but not vice-versa)

Spaghetti stack structure is used in situations when records are dynamically <br>
pushed and popped onto a stack as execution progresses, but references to the <br>
popped records remain in use. Following are some applications of Spaghetti Stack. <br>

Compilers, for languages such as C, create a spaghetti stack as it opens and <br>
closes symbol tables representing block scopes. When a new block scope is opened, <br>
a symbol table is pushed onto a stack. <br>
When the closing curly brace is encountered, the scope is closed and the symbol table <br>
is popped. But that symbol table is remembered, rather than destroyed. <br>
And of course it remembers its higher level “parent” symbol table and so on. <br>
