---
aliases:
  - simplicial set
  - ensemble simplicial
summary: 函子 Δ^op → Set；同伦论与 ∞-范畴（Kan 复形、拟范畴、dg nerve）的组合模型
---
# Definition

Let $\Delta$ be the **simplex category**: objects $[n]=\{0<1<\dots<n\}$ for $n\geq 0$, morphisms the weakly order-preserving maps. A **simplicial set** (单纯集) is a functor $X:\Delta^{\mathrm{op}}\to\mathbf{Set}$, and a morphism is a natural transformation. They form the presheaf topos $\mathbf{sSet}$. Write $X_n=X([n])$ for the set of $n$-simplices.

Concretely, $X$ is given by sets $X_n$ with **face maps** $d_i:X_n\to X_{n-1}$ and **degeneracy maps** $s_i:X_n\to X_{n+1}$ ($0\le i\le n$), induced by the coface $\delta^i$ (skip $i$) and codegeneracy $\sigma^i$ (repeat $i$), subject to the **simplicial identities**
$$d_id_j=d_{j-1}d_i\ (i<j),\qquad s_is_j=s_{j+1}s_i\ (i\le j),$$
$$d_is_j=\begin{cases}s_{j-1}d_i & i<j\\ \mathrm{id} & i=j,\,j+1\\ s_jd_{i-1} & i>j+1.\end{cases}$$
A simplex is **degenerate** if it lies in the image of some $s_i$. Every simplex $x\in X_n$ is uniquely of the form $x=\sigma^*y$ with $\sigma:[n]\twoheadrightarrow[m]$ a surjection and $y\in X_m$ nondegenerate (Eilenberg–Zilber lemma).

# Examples

- **Standard simplex** $\Delta^n=\mathrm{Hom}_\Delta(-,[n])$. By Yoneda, $X_n\cong\mathrm{Hom}(\Delta^n,X)$. Its sub-objects are the boundary $\partial\Delta^n$ and the **horns** $\Lambda^n_k$ ($0\le k\le n$), the union of all faces except the $k$-th.
- **Singular complex** $\mathrm{Sing}\,X$ of a space: $(\mathrm{Sing}\,X)_n=\mathrm{Hom}_{\mathbf{Top}}(|\Delta^n|,X)$.
- **Nerve** $N\mathcal{C}$ of a small category: $N\mathcal{C}_n=$ composable strings $c_0\to\cdots\to c_n$, with $d_i$ composing (or dropping an end) and $s_i$ inserting identities. $BG=|NG|$ for a group $G$.
- **Ordered simplicial complexes** give simplicial sets whose nondegenerate simplices are the faces. See [[Simplicial complex 单纯复形 complexe simplicial|simplicial complex]]. The nerve of a poset recovers the order complex.
- **Simplicial abelian groups / modules**, e.g. the free simplicial abelian group $\mathbb{Z}[X]$, whose normalized chain complex computes $H_*(|X|;\mathbb{Z})$.
- **dg nerve** $N_{\mathrm{dg}}(\mathcal{A})$ of a dg category $\mathcal{A}$ (Lurie, *HA* 1.3.1). Its $n$-simplices are objects $x_0,\dots,x_n$ together with $f_I\in\mathcal{A}^{1-k}(x_{i_0},x_{i_k})$ for each $I=\{i_0<\cdots<i_k\}$ with $k\geq1$. These satisfy identities expressing $d f_I$ through the $f_{I\setminus\{i_j\}}$ and the composites $f_{\{i_j<\cdots<i_k\}}\circ f_{\{i_0<\cdots<i_j\}}$. In particular, edges are closed degree-$0$ morphisms and $2$-simplices are homotopies $f_{02}\simeq f_{12}f_{01}$. It is a quasi-category, and it models the $\infty$-category underlying a pretriangulated dg category such as a dg Higgs category.

# Key results

- **Geometric realization** $|-|:\mathbf{sSet}\rightleftarrows\mathbf{Top}:\mathrm{Sing}$ is an adjunction, with $|X|=\int^{[n]}X_n\times|\Delta^n|$, a CW complex with one $n$-cell per nondegenerate $n$-simplex. $|X\times Y|\cong|X|\times|Y|$ in compactly generated spaces. $|\mathrm{Sing}\,T|\to T$ is a weak equivalence (Milnor).
- **Kan–Quillen model structure.** In it cofibrations are monomorphisms, weak equivalences are maps inducing weak equivalences on realizations, and fibrant objects are **Kan complexes**, which have fillers for all horns $\Lambda^n_k\to X$. $|-|\dashv\mathrm{Sing}$ is a Quillen equivalence, so $\mathrm{Ho}(\mathbf{sSet})\simeq\mathrm{Ho}(\mathbf{Top})$.
- **Nerves and $\infty$-categories.** $N$ is fully faithful. A simplicial set is a nerve iff every inner horn ($0<k<n$) has a *unique* filler. $N\mathcal{C}$ is Kan iff $\mathcal{C}$ is a groupoid. Dropping uniqueness gives **quasi-categories** (Boardman–Vogt, Joyal, Lurie), the fibrant objects of the Joyal model structure.
- **Dold–Kan correspondence.** Normalized chains give an equivalence $\mathbf{sAb}\simeq\mathrm{Ch}_{\geq0}(\mathbf{Ab})$, and more generally for any abelian category. Homotopy groups correspond to homology. This is the bridge between simplicial and dg (connective) homological algebra.
- Simplicial homotopy groups of a Kan complex agree with those of its realization.

# Related

- [[Combinatorics 组合数学 combinatoire|Combinatorics hub]]
- [[Simplicial complex 单纯复形 complexe simplicial|Simplicial complex]]
- [[Building 建筑 immeuble|Building]]: realizations of buildings as spaces.
- [[Quiver 箭图 carquois|Quiver]]: the path category of $Q$ has a nerve. For the dg categories of quivers with potential (Ginzburg, Higgs) one uses the dg nerve.

# References

- P. G. Goerss, J. F. Jardine, *Simplicial Homotopy Theory*, Progr. Math. 174, Birkhäuser 1999.
- J. P. May, *Simplicial Objects in Algebraic Topology*, Van Nostrand 1967 (Univ. Chicago Press 1992).
- E. Riehl, *Categorical Homotopy Theory*, CUP 2014; E. Riehl, A leisurely introduction to simplicial sets (notes).
- J. Lurie, *Higher Topos Theory*, Ann. of Math. Stud. 170, 2009; *Higher Algebra*, §1.3.1 (dg nerve).
- D. Quillen, *Homotopical Algebra*, LNM 43, Springer 1967.
