Download Link: https://assignmentchef.com/product/solved-p3-cs373
<br>



Construct a PDA that accepts { x#y#z | x, y, z in {0, 1}<sup>+</sup> with x ≈ y, or x ≈ z, or y ≈ z }.

Define x ≈ y as follows: Let x = x<sub>1</sub>x<sub>2</sub> … x<sub>n</sub> and y = y<sub>1</sub>y<sub>2</sub> … y<sub>m</sub>, and let n’ and m’ be the largest odd values less than or equal to n and m respectively. Let x’ = x<sub>1</sub>x<sub>3</sub> … x<sub>n’</sub> and y’ = y<sub>1</sub>y<sub>3</sub> … y<sub>m’</sub>. Then x ≈ y if x’ ≠ y’ (that is, x<sub>1</sub>x<sub>3</sub> … x<sub>n’</sub> ≠ y<sub>1</sub>y<sub>3</sub> … y<sub>m’</sub>).

For your PDA to work correctly it will need to be non-deterministic. You can assume that you will always be given a valid string – that is, the input will always contain two #s, and x, y, and z will be strings over {0, 1} of length greater than 0.

My PDA accepts x#y#z under any of the following conditions: |x’| ≠ |y’| or |x’| ≠ |z’| or |y’| ≠ |z’| or there exists odd value i with x<sub>i</sub> ≠ y<sub>i</sub> or x<sub>i</sub> ≠ z<sub>i</sub> or y<sub>i</sub> ≠ z<sub>i</sub>.

If you are having memory issues, try starting JFLAP from the command line allocating more memory. As an example, from the directory that JFLAP is in, enter “java -Xmx500m -classpath JFLAP.jar JFLAP”. The -Xmx500m tells java to allocate 500MB of memory to the heap. By default, java only allocates 64MB to the heap.

For this programming assignment, and the remainder of them for the semester, you need to follow my submission directions – filename (lower case last name followed by “_p3.jff”) and e-mail subject (“CS 373 program 3”).

You may use JFLAP version 8 if you have problems with epsilon transitions with version 7.1.3