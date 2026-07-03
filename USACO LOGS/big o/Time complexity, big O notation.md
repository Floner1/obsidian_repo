**Complexity:** the amount of computational resources an algorithm uses, execution time and memory space, as the input grows. 

**Big O:** classifies how an algorithm's running time or memory usage scales as the input size becomes very large, focusing only on the dominant growth categories (linear, quadratic, cubic, etc. )and ignoring constants and lower-order terms.

O(n): n tells u how much input, O tells u how much the amount of work scales

![[big o example.png]]
![[different n relative to big o.png]]
# LOOPS:
The time complexity of loops is the number of iterations that the loop runs

CALCULATE nest loop time complexity:  multiply only when the inner loop performs ~ the same amount of work for every iteration of the outer loop. Otherwise, count or sum how many times the inner loop actually runs.

**constant terms**: are things such as 5 or 67

**lower order terms:** are things such as +57 in n+57 or n in n^2+n, bv they eventually get insignificant as n increases.

If an algorithm contains multiple blocks, then its time complexity is the worst time complexity out of any block.

a block is just a group of statements that are treated as 1

if 2 or more blocks run sequentially, u take the time complexity of each and add it to find total big o

if 2 or more blocks run parallel, u just take the max big O of all of the blocks that ran parallel

**CONSTANT FACTOR:**
different operations with same complexity take different amounts of time to run
usually ignored by big o, unless u receive a time limt exceeded warning
