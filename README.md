# Skein 512-512

## Java

Here are two Java implementations of the Skein 512-512 hash algorithm. Both implementations are relatively small, and compatible with the revised (version 1.3) test vectors and reference implementation.

[Skein512.java](http://www.h2database.com/skein/Skein512.java) is optimize for speed. 151 MB/s on a MacBook Pro, 2.53 GHz Intel Core 2 Duo; Java 1.6, server mode.

[Skein512Small.java](http://www.h2database.com/skein/Skein512Small.java) is optimize for size (32 lines).

[Test.java](http://www.h2database.com/skein/Test.java) and [testVectors.txt](http://www.h2database.com/skein/testVectors.txt) (3 MB) tests for both implementations.

## Scala

The Scala implementation is based on the small Java implementation.

[Test.scala](http://www.h2database.com/skein/Test.scala) and [Skein512.scala](http://www.h2database.com/skein/Skein512.scala).

## Javascript

Here is a Javascript implementations of the Skein 1.3 512-512 hash algorithm. It is quite small, but slow, because Javascript does not directly support 64 bit integer operations. This implementation should be compatible with the revised (version 1.3) test vectors and reference implementation (warning: only a subset of the tests have been run). The message size must be a multiple of 8 bits.

## Public Domain
This algorithm and source code is released to the public domain.

## Feedback
For questions, improvements, or remarks, send an email to "db support" (one word) at "h2 database" (one word) dot com.

## Changelog

* 2010-12-11: The implementations are now compatible with the revised reference implementation (1.3).
* 2010-01-18: Slight speedup (from 141 MB to 151 MB) due to early array bounds checking in getLong.
* 2009-09-16: The implementations are now compatible with the revised reference implementation (1.2).
* 2009-05-09: Skein512.java: The method hash(..) is now static. Thanks to Greg Ewing!
* 2009-03-10: The Scala implementation is ready.
* 2008-12-08: The Javascript implementation is ready.
* 2008-12-05: The implementation is now compatible with the revised reference implementation (1.1).
* 2008-11-05: The Java implementation is ready.