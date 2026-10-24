---
aliases:
  - simplicial complex
  - complexe simplicial
summary: 对子集封闭的有限顶点集族；Coxeter 复形、building、cluster 复形的组合载体
---
# Definition

An **(abstract) simplicial complex** (单纯复形) is a pair $(V,\Delta)$ of a set $V$ of vertices and a set $\Delta$ of finite nonempty subsets of $V$ (the **simplices** or faces) such that

- $\{v\}\in\Delta$ for every $v\in V$;
- if $\sigma\in\Delta$ and $\emptyset\neq\tau\subseteq\sigma$, then $\tau\in\Delta$.

A simplex $\sigma$ with $|\sigma|=n+1$ has **dimension** $n$, and $\dim\Delta=\sup_\sigma\dim\sigma$. Some authors (e.g. Abramenko–Brown) also include $\emptyset$ as the $(-1)$-simplex. A **simplicial map** $f:(V,\Delta)\to(V',\Delta')$ is a map $f:V\to V'$ with $f(\sigma)\in\Delta'$ for all $\sigma\in\Delta$. $\Delta$ is **pure** if all maximal simplices have the same dimension.

The **geometric realization** $|\Delta|$ is the subspace of $\mathbb{R}^{(V)}$ consisting of the convex combinations $\sum_{v\in\sigma}t_v e_v$ ($t_v\ge0$, $\sum t_v=1$, $\sigma\in\Delta$), with the weak (colimit) topology.

Equivalently (cf. Abramenko–Brown, Appendix A), with $\emptyset$ adjoined as a bottom element, a poset is the face poset of a simplicial complex iff any two elements have a greatest lower bound and every lower interval $\{\tau\le\sigma\}$ is isomorphic to the Boolean lattice of subsets of a finite set. Posets satisfying only the second condition are *simplicial posets*. This is how the Coxeter complex and $\Delta(G,B)$, defined as posets of cosets, are seen to be simplicial complexes.

# Examples

- The $n$-simplex $2^{[n]}\setminus\{\emptyset\}$ and its boundary $\partial\Delta^n$, with $|\partial\Delta^n|\cong S^{n-1}$.
- **Order complex** $\Delta(P)$ of a poset $P$: its simplices are the finite nonempty chains. $|\Delta(P)|$ is the classifying space of $P$ viewed as a category, i.e. the realization of its nerve.
- **Flag (clique) complex** of a graph: its simplices are the finite cliques.
- **Nerve** of a cover $\mathcal{U}=\{U_i\}$: its simplices are the finite $I$ with $\bigcap_{i\in I}U_i\neq\emptyset$. Nerve theorem: if all nonempty finite intersections are contractible (open cover of a paracompact space), the nerve is homotopy equivalent to $X$.
- **Coxeter complex** $\Sigma(W,S)$: cosets $wW_J$ ($J\subsetneq S$) under reverse inclusion. Its vertices are the cosets of the maximal standard parabolics $W_{S\setminus\{s\}}$ and its chambers are the elements of $W$. For finite $W$ it is a triangulation of the sphere $S^{|S|-1}$ cut out by the reflecting hyperplanes. See [[Coxeter system 考克斯特系统 système de Coxeter|Coxeter system]].
- **Buildings** are simplicial complexes glued from Coxeter complexes. See [[Building 建筑 immeuble|Building]].
- **Cluster complex** (Fomin–Zelevinsky). For a cluster algebra of finite type, its vertices are the cluster variables and its simplices are the sets of pairwise compatible ones. The maximal simplices are the clusters. It is a pure $(n-1)$-dimensional complex, homeomorphic to $S^{n-1}$, and it is the dual complex of the generalized associahedron. Its vertices can be indexed by the almost positive roots $\Phi_{\geq -1}$. Categorically, simplices correspond to basic rigid objects of the cluster category (and clusters to cluster-tilting objects); see [[Quiver 箭图 carquois|quiver]].

# Key results

- **Chamber complexes.** A finite-dimensional pure complex is a chamber complex if any two maximal simplices are joined by a gallery. Coxeter complexes and buildings are thin, resp. thick, chamber complexes. Coxeter complexes and buildings are shellable (Björner 1984). For spherical ones this recovers the Solomon–Tits theorem.
- **Simplicial approximation.** Every continuous map $|K|\to|L|$ with $K$ finite is homotopic to the realization of a simplicial map $\mathrm{sd}^n K\to L$ for some barycentric subdivision.
- **Homology.** Simplicial homology of $\Delta$ (ordered or oriented chains) agrees with singular homology of $|\Delta|$.
- **Stanley–Reisner.** $\Delta$ on finite $V$ corresponds to the squarefree monomial ideal $I_\Delta\subseteq k[x_v]$. Cohen–Macaulayness of $k[\Delta]$ is detected by links (Reisner).
- **Relation to [[Simplicial set 单纯集 ensemble simplicial|simplicial sets]].** A simplicial complex with a total order on each simplex, e.g. one induced by a total order on $V$, determines a simplicial set whose nondegenerate $n$-simplices are the $n$-faces, with the same realization. Simplicial sets are the homotopically well-behaved generalization: they are closed under colimits and products, and they allow multiple faces and degenerate simplices.

# Related

- [[Combinatorics 组合数学 combinatoire|Combinatorics hub]]
- [[Simplicial set 单纯集 ensemble simplicial|Simplicial set]]
- [[Coxeter system 考克斯特系统 système de Coxeter|Coxeter system]]
- [[Building 建筑 immeuble|Building]]
- [[Quiver 箭图 carquois|Quiver]]

# References

- P. Abramenko, K. S. Brown, *Buildings: Theory and Applications*, GTM 248, Springer 2008, Appendix A (simplicial complexes and posets).
- J. R. Munkres, *Elements of Algebraic Topology*, Addison-Wesley 1984.
- A. Björner, Topological methods, in *Handbook of Combinatorics*, Elsevier 1995; Some combinatorial and algebraic properties of Coxeter complexes and Tits buildings, *Adv. Math.* 52 (1984).
- S. Fomin, A. Zelevinsky, Y-systems and generalized associahedra, *Ann. of Math.* 158 (2003).
- R. P. Stanley, *Combinatorics and Commutative Algebra*, 2nd ed., Birkhäuser 1996.
