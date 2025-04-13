# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

$G=(V, E)$ is completely connected iff $\forall u, v \in V, u \neq v 
\implies (u,v) \in E$.

A function $f: V_1 \rightarrow V_2$ is onto iff $\forall v_2, \exists v_1, (v_2 \in V_2 \implies v_2 = f(v_1))$

A function $f: V_1 \rightarrow V_2$ is one-to-one iff $(f(v_1) = f(v_2) \implies v_1 = v_2))$

Let $A=(V_1 , E_1)$ and $G_2=(V_2, E_2)$ such that $|V_1| = |V_2|$ and $G_1$ and $B$
are both completely connected. 

### Proof

Because $|V_1| = |V_2|$, there must exists a bijection $f: V_1 \rightarrow V_2$ because 
each element in $V_1$ can be mapped to a unique element in $V_2$ and in doing so, every
element in $V_2$ will be mapped onto by some element in $V_1$. 

Since both graphs are completely connected, every pair of distinct vertices in each
graph will have an edge between them. For any bijection $f: V_1 \rightarrow V_2$, any
pair of vertices $(u,v) \in E_1$, where $,u,v \in V_1$, can be mapped to a pair of vertices 
such that $f(u) \in V_2$ and $f(v) \in V_2$. Because both graphs include every set of possible 
vertex pairs that are distinct from one another, $(u,v) \in E_1 \implies (f(u),f(v)) \in E_2$.
Likewise, because f is a bijection and each vertex in $V_2$, is mapped onto by some vertex 
in $V_2$, the same logic can be applied to conclude that $(f(u),f(v)) \in E_2 \implies (u,v) 
\in E_1$

Therefore, since $A$ and $B$ have the same number of nodes and are completely connected, they 
must be isomorphic.

##Extra Help

All of the work done here was my own, but I had to consult some of my notes from COSC 2300 
to recall the definition of one-to-one and onto. 

"I certify that I have listed all sources used to complete this exercise, 
including the use of any Large Language Models. All of the work is my own, 
except where stated otherwise. I am aware that plagiarism carries severe 
penalties and that if plagiarism is suspected, charges may be filed against 
me without prior notice."
