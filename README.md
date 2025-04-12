# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

$G=(V, E)$ is completely connected iff $\forall u \in V,\forall v \in V, u \neq v 
\implies (u,v) \in E$.

Let $G_1=(V_1 , E_1)$ and $G_2=(V_2, E_2)$ such that $|V_1| = |V_2|$ and $G_1$ and $G_2$
are both completely connected. 

A function $f: A \rightarrow B is onto iff $\forall b \in B, \exists a \in A$ 
such that $f(a) = b$. 

A function $f: A \rightarrow B is one-to-one iff $\forall a_1, a_1 \in A , f(a_1) = f(a_2) 
\implies a_1 = a_2$.

$|V_1| = |V_2|$ and both graphs are completely connected, meaning every vertex $v_1 \in V_1$
has an edge to each other distinct vertex in that graph. Likewise, every vertex $v_2 \in V_2$
has an edge to each other distinct vertex in that graph. Therefore, $|E_1| = |E_2|$ and there
exists an onto function $f: V_1 \rightarrow V_2$ such that $\forall (u_2,v_2) \in E_2, \exists (u_1,v_1)
\in E_1$ such that $(f(u_1), f(v_1)) = (u_2,v_2)$. 

Since $|V_1| = |V_2|$ and f is onto, f must also be one-to-one. If all $v_2 \in V_2$ are 
mapped to by some $v_1 \in V_1$, then each $v_1$ must map to a unique vertex in $V_2$. This 
means that f is a bijection between $G_1$ and $G_2$. 

By the definition of a bijection, $f: V_1 \rightarrow V_2$ is also function such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.
