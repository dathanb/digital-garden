---
created: 2022-10-16T10:54:52-07:00
updated: 2022-10-16T11:04:29-07:00
---

Cosine similarity is one metric for calculating similarity of two vectors. It's probably the most commonly used metric for calculating [[Text similarity|similarity of two texts]].

It takes advantage of the fact that 
$$
A \cdot B = \|A\| \|B\| cos \Theta
$$

to let us calculate $cos \Theta$ as
$$
cos \Theta = \frac{A \cdot B}{\|A\| \|B\|} = \frac{\sum_{i=1}^{n} A_i B_i}{\sqrt{\sum_{i=1}^{n}A_i^2}\sqrt{\sum_{i=1}^{n}B_i^2}}
$$

Which in many cases can be calculated efficiently on modern hardware for very large corpora.


# Links
- [Academic overview of cosine similarity](https://www.sciencedirect.com/topics/computer-science/cosine-similarity)