Below are two videos you might want to watch as you are having lunch or on a Friday night (instead of scrolling down pointlessly on Instagram or ~~TikTok~~)

## Donald Knuth

[Don Knuth](https://en.wikipedia.org/wiki/Donald_Knuth) coined the term "algorithm analysis" and played an important role in popularizing the use of asymptotic notation in computer science. 
Thus he is known as the **father of algorithm analysis**. He is still a faculty member at Stanford.

Watch the following lecture in which Knuth recreates a 1969 lecture he gave at Stanford in which he introduced to the faculty there what he means by "algorithm analysis".

[![Watch the video](https://img.youtube.com/vi/vkUNH9r6UCI/hqdefault.jpg)](https://www.youtube.com/embed/vkUNH9r6UCI?si=KA9QoRN_SQ8_SwYa)

You might find it difficult to watch the whole lecture, but it is interesting to watch at least its beginning in which he talks about how and when he came up with the name "algorithm analysis" and demos the first example he used to explain what he means by the term.


## Asymptotic Notation

Knuth's analysis focused mostly on the **average case**. He was interested in making mathematical statements about the performance of algorithms that are **useful in practice**, i.e. statements that are useful for comparing actual running times and for predicting performance. However, this has drawbacks:

- The assumptions made in average case analysis might not be realistic.
- The math can be too detailed and difficult!

 To address these drawbacks, other computer scientists like [Aho, Ullman & Hopcroft](https://www.amazon.com/Design-Analysis-Computer-Algorithms/dp/0201000296) and [CLRS](https://en.wikipedia.org/wiki/Introduction_to_Algorithms) popularized the use of **worst-case** analysis and the **Big-O** notation in particular, which simplified algorithm analysis greatly and led to an era where algorithm designers compete for reducing upper-bounds on algorithm performance. However, this has drawbacks also:

- Worst-case input is at many times not representative of input typically encountered in practice.
- Using Asymptotic notation hides constants that are very important for comparing between algorithms and for predicting actual running times.

Watch the video below by [Bob Sedgwick](https://en.wikipedia.org/wiki/Robert_Sedgewick_(computer_scientist)) (a student of Knuth and a pioneer in the field of algorithm analysis) in which he argues for a scientific method for algorithm analysis that involves both experimental and theoretical analysis as well-as the use of the [tilde (∼) notation](https://en.wikipedia.org/wiki/Asymptotic_analysis#Definition) instead of Big-O and Big-Theta.
(Tilde notation does not drop the coefficient of the highest order term but drops lower order terms).

[![Watch the video](https://img.youtube.com/vi/j_sHSf5Cr4A/hqdefault.jpg)](https://www.youtube.com/watch?v=j_sHSf5Cr4A)

