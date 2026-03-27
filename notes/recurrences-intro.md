# Recurrence Equations

A _recurrence equation_ defines a function in terms of its value on smaller inputs. Such equations are useful for describing the behavior of _recursive_ algorithms. 

Given a recursive algorithm and a certain aspect of its behavior that we want to analyze (e.g., the number of operations it performs, or the amount of memory it uses), we can often express that using a recurrence equation. Solving the recurrence equation then gives us insight into the behavior of the algorithm (e.g., its time complexity or space complexity).

## Example 1

Consider the following recursive implementation of binary search:

```C++
bool search(int a[], int k, int lo, int hi) {
    if (lo > hi)
        return false;

    int mid = (lo + hi) / 2;
    if (a[mid] == k)
        return true;
    else if (a[mid] < k) {
        return search(a, k, mid + 1, hi);
    else 
        return search(a, k, lo, mid - 1);
}
```

If we are interested in analyzing the running time of this algorithm, we notice that the following:
- If the search interval is **empty** (i.e., `lo > hi`), then we perform _constant_ amount of work.
- If the search interval is **not empty**, we make 1-2 comparisons and then a new call to `search` on an interval that is half the size of the original.

Therefore, we can express the time needed to search an array of size $n$ using the following recurrence equation:

$$T(n) = \begin{cases}
c & \text{if } n = 0 \\
c + T(n/2) & \text{if } n > 0
\end{cases}$$

> 💡 The recurrence equation tells us that the time needed to search an array of size $n$ is equal to the time needed to search an array of size $n/2$ plus a constant.

But what is the time needed to search an array of size $n/2$? We can express that using the same recurrence equation: $T(n/2) = c + T(n/4)$, which makes the original equation look like this:

$$T(n) = c + (c + T(n/4))$$

We can apply the same reasoning again to get:

$$T(n) = c + (c + (c + T(n/8)))$$

If we keep applying the same reasoning, we will notice that we will get the constant $c$ repeated $\sim \log_2 n$ times, because we can only divide $n$ by 2 a logarithmic number of times before we get to the base case. This means that the solution to the recurrence equation is $T(n) = \Theta(\log n)$, which matches our intuition about the running time of binary search.
