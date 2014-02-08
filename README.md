rs
==

C++ Reed Solomon encoding library

Reed Solomon encoding algorithms use the concept of finite field Z/p. Since the number of elements in such finite fields have to be a prime number, most of algorithms has to construct Galois Fields with the help of Z/p, so that a byte can be represented by an elements in a GF of size 265.

Another way to attack the problem is to note that 257 is a prime number. So it is possible to use Z/257 to construct a field directly without a Galois Field. This will increase the required storage space for eraser code slightly (1/257), but with the simplified algorithm, it may well worth it.

