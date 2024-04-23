[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/ppBU16qM)
# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

## Proof

Suppose graphs $A$ and $B$ are composed of just one node each. 

A = [$n_{1,1}$]

B = [$n_{2,1}$]

These graphs are already isomorphic because $n_{1,1} \rightarrow n_{2,1}$, that's the only mapping that exists here. 

Let's add a new node to each graph and connect it to the other node in that graph, so that the graphs remain completely connected. 

A = [$n_{1,1}$] - $E_{1,1}$ - [$n_{1,2}$]

B = [$n_{2,1}$] - $E_{2,1}$ - [$n_{2,2}$]

These graphs with edges are also isomporphic becasue they satisfy the definition. $f: n_1 \rightarrow n_2$ such that $(n_{1,1}, n_{1,2}) \in E_{1,1}$ iff $(f(n_{1,1}), f(n_{1,2})) \in E_{2,1}$

If I continute to add one node to each graph and connect it to every other node in the graphs to be completely connected, the new edges and nodes will be added to the bijection function and satisfy the definition of isomorphism, no matter where I add the node. And in general, if I keep doing this method, connecting every new node to all other nodes to be completely connected, they will continute to be isomorphic with each new $n-1$ edges and node. I can therefore reach two completely connected graphs of any size that are isomorphic. 

$\therefore$ Any graphs $A$ and $B$ that have the same number of nodes and are completely connected have to be isomorphic. 