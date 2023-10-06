## More Divide & Conquer Examples
The following are more examples of well-known Divide & Conquer algorithms. Some of these examples were taught previousl at PSUT and are commonly taught in courses on algorithms.

- **Counting Inversions.**
This problem has many applications and can be solved efficiently with a slight modification of Mergesort. [[video1](https://www.youtube.com/watch?v=7_AJfusC6UQ&ab_channel=StanfordAlgorithms)][[video2](https://www.youtube.com/watch?v=PLkuid82dbc&ab_channel=FreeEngineeringLectures)]

- **Karatsuba's Algorithm for Integer Multiplication.**
This is a classic (and quite clever) algorithm for multiplying two integers. It is better than the algorithms discussed in the introductory lecture of this course ([slides from Spring 2023](https://drive.google.com/file/d/1dlXfadqUiaIL6k8WQFwVS8zwk6YBSt98/view?usp=drive_link), [video](https://www.youtube.com/watch?v=JCbZayFr9RE&list=PLXFMmlk03Dt7Q0xr1PIAriY5623cKiH7V&index=3&ab_channel=StanfordAlgorithms)).

- **Finding the closest pair of points in a 2D space.**
While the divide and conquer algorithm is not the fastest known algorithm for this problem, it is a classic example of divide and conquer that can be eye opening to learn! [[video](https://www.youtube.com/watch?v=6u_hWxbOc7E&ab_channel=LingQi)]

- **Strassen's Algorithm for Matrix Multiplication** ([wikipedia article](https://en.wikipedia.org/wiki/Strassen_algorithm))
- **The _MergeHull_ and _QuickHull_ algorithms for finding convex hulls.**

## Sorting Lower Bound

This is a very important result in computer science. Check [these slides](https://drive.google.com/file/d/1ihI42MveiRaLQ-NkrUSbpbMQ-u7yc4ay/view?usp=drive_link).

## Median Finding
* Quick Select has bad theoretical worst-case running time. How can we find the median in linear time? [Watch Turing Award winner Blum talk about his algorithm](https://www.youtube.com/watch?v=3NWz6PY-4-k&ab_channel=TuringAwardeeClips). [Watch this explanation of the algorithm](https://www.youtube.com/watch?v=n8cyxDtp9t4&ab_channel=EasyTheory).
* Given a continuously arriving stream of data, how can we efficiently, at any point, report the median? [Check these slides](https://drive.google.com/file/d/1I8vq5YKSKqk0QyhlMSgSFtVOvVV0FvV4).
