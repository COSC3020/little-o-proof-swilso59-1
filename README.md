# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

Definition of little $o$:
$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

Definition of Big $O$:
$f(n)\in O(g(n)) \iff \exists c > 0,\exists n_0, \forall n\ge n_0: f(n) \leq c\cdot g(n)$

## Proof 
In our proof we want to show that $if$ $f(n)\in o(g(n))$, $then$ $f(n)\in O(g(n))$ 

Starting with the definiton of little $o$. We can see that for all positive constant $c$, There exists a point $n_0$ which all $n > n_0$ $f(n) < c\cdot g(n)$

In the definition of Big $O$ we can see that there exists a constant $c$ that for all $n \ge n_0$ $f(n) \leq c \cdot g(n)$

Since in little $o$ the condition for the constant $c$ is true for all. for Big $O$ there only needs to be one that exists. If all are ture for the little $o$ condition this means that there is always one constant $c$ that is true for the Big $O$ condition. 

In little $o$ $f(n) < c \cdot g(n)$ this implies that $f(n) \leq g(n)$ 

So we can conclude that $f(n) \in o(g(n)) \implies f(n) \in O(g(n))$. 

## Plagiarism Acknowledgement
- I started this by taking a look at https://github.com/COSC3020/little-o-proof-swilso59.git
- I also looked online for definitions of Big O simply with a google search. I found these websites helpful.
  https://xlinux.nist.gov/dads/HTML/bigOnotation.html#:~:text=Definition%3A%20A%20theoretical%20measure%20of,multiple%20of%20g(n).
  https://web.mit.edu/16.070/www/lecture/big_o.pdf
- I reviewed my previous repository and tried to explain it in a more clear manner.
- I was curous about how other classmates were wording there proof so I had a look at a few. 
  https://github.com/COSC3020/little-o-proof-ZachRenz.git
  https://github.com/COSC3020/little-o-proof-egkallas.git
  https://github.com/COSC3020/little-o-proof-ZachRenz.git

“I certify that I have listed all sources used to complete this exercise, including the use
of any Large Language Models. All of the work is my own, except where stated
otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is
suspected, charges may be filed against me without prior notice.”

