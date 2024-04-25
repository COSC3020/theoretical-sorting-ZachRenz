[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/9YUeXH71)
# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.

## Testing for $O(n)$

If we only have a blackbox algorithm, then we'll have to test it and graph it. I would test it with different cases, like being sorted, slightly sorted, randomly shuffled, completely reversed for the worst case, and lists of the same number, and make about 30 different versions of each case, going from 1 to 30 length. I would also test empty lists. Then we can graph the time it took to sort over the change in length and find a linear regression line for the data. If the correlation coefficient $r$ is significantly close to 1, then we do truly have a linear algorithm, otherwise the algorithm does not have a $O(n)$ complexity. 

## Theoretical Analysis

This Computer Science researcher says that his alrogithm sorts in $O(n)$ time using comparisions of two elements of a time. But we know from class it is proven that the best time for a comparison of two elements sorting algorithm can only be $\Omega(nlogn)$. So theoretically this algorithm can not be correct. 
