This small project implements a simple Bloom Filter.

1. Build with javac
   (1) cd to project home directory.
   (2) $ mkdir -p build/classes
   (2) $ javac -cp lib/junit-4.10.jar -d build/classes src/java/org/schubert/bloom/*.java src/test/org/schubert/bloom/*.java

2. Build with ant
   (1) cd to project home directory, here is a build.xml
   (2) to build jar package
       $ ant or ant package
   (3) to build java docs
       $ ant javadoc
   (4) clean all build outputs
       $ ant cleanall

3. Run unit test
   (1) cd to build/classes
       $ java -cp .:../../lib/junit-4.10.jar org.junit.runner.JUnitCore org.schubert.bloom.SimpleBloomFilterTest
   (2) or, if you have built jar, and stay in home
       $ java -cp bloomfilter-simple-1.0.0.jar:lib/junit-4.10.jar org.junit.runner.JUnitCore org.schubert.bloom.SimpleBloomFilterTest
   (3) or, use ant to do unit test
       $ ant unittest
       
That's easy!
