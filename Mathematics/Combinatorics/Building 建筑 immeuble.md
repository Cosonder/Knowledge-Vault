---
aliases:
  - building
  - immeuble
  - Tits building
summary: 由 Coxeter 复形（apartment）粘合而成的单纯复形，是带 BN-pair 的群的几何
---
# Definition

Fix a [[Coxeter system 考克斯特系统 système de Coxeter|Coxeter system]] $(W,S)$, and let $\Sigma=\Sigma(W,S)$ be its **Coxeter complex**: the poset of cosets $wW_J$ ($w\in W$, $J\subsetneq S$) under reverse inclusion. It is a [[Simplicial complex 单纯复形 complexe simplicial|simplicial complex]] whose chambers (maximal simplices) are the elements of $W$.

**Simplicial definition** (Abramenko–Brown, Def. 4.1). A **building** (immeuble) of type $(W,S)$ is a simplicial complex $\Delta$ together with a family $\mathcal{A}$ of subcomplexes, called **apartments**, such that

- (B0) each $\Sigma\in\mathcal{A}$ is isomorphic to the Coxeter complex $\Sigma(W,S)$;
- (B1) any two simplices of $\Delta$ lie in a common apartment;
- (B2) if $\Sigma,\Sigma'\in\mathcal{A}$ both contain a chamber $C$, there is an isomorphism $\Sigma\xrightarrow{\sim}\Sigma'$ fixing $\Sigma\cap\Sigma'$ pointwise.

$\mathcal{A}$ is a **system of apartments**. The union of all systems of apartments is again one, the **complete** system $\mathcal{A}(\Delta)$. So one often writes "a building $(\Delta,\mathcal{A})$" or simply speaks of the apartment system $\mathcal{A}$. Codimension-1 simplices are **panels**. $\Delta$ is **thick** if every panel is a face of at least three chambers, and **thin** if exactly two; thin buildings are Coxeter complexes. $\Delta$ is **spherical** if $W$ is finite, and **affine** (Euclidean) if $W$ is an affine Coxeter group.

**$W$-metric definition** (Tits). A building of type $(W,S)$ is a set $\mathcal{C}$ (of chambers) with a map $\delta:\mathcal{C}\times\mathcal{C}\to W$ such that, for $\delta(C,D)=w$,

- (WD1) $w=1\iff C=D$;
- (WD2) if $\delta(C',C)=s\in S$, then $\delta(C',D)\in\{sw,w\}$, and $\delta(C',D)=sw$ when $\ell(sw)=\ell(w)+1$;
- (WD3) for every $s\in S$ there is $C'$ with $\delta(C',C)=s$ and $\delta(C',D)=sw$.

The two definitions are equivalent: chambers of the simplicial building with $\delta$ read off in a common apartment, and conversely the simplicial complex of residues.

# Examples

- **Coxeter complexes** are the thin buildings. For $W=S_3$ it is a hexagon; for $W$ the infinite dihedral group it is the real line subdivided at the integers.
- **Spherical building of a vector space.** Let $V$ be an $n$-dimensional vector space over $k$. $\Delta(V)$ is the flag complex of proper nonzero subspaces (simplices are chains $0\subsetneq V_1\subsetneq\cdots\subsetneq V_r\subsetneq V$). Apartments correspond to frames $V=L_1\oplus\cdots\oplus L_n$ of lines. It has type $A_{n-1}$ and equals $\Delta(GL_n(k),B)$ for the [[BN-pair BN对 BN-paire|BN-pair]] of $GL_n(k)$. For $n=3$ it is the incidence graph of the projective plane $\mathbb{P}^2(k)$.
- **Rank 2.** Spherical buildings of type $I_2(m)$ are exactly the **generalized $m$-gons**: bipartite graphs of diameter $m$ and girth $2m$. Projective planes are the generalized $3$-gons. Feit–Higman: finite thick generalized $m$-gons exist only for $m\in\{2,3,4,6,8\}$.
- **Trees.** A tree without leaves is a building of type $\widetilde{A}_1$, whose apartments are the bi-infinite geodesics. The Bruhat–Tits tree of $SL_2(\mathbb{Q}_p)$ is the $(p+1)$-regular tree. Its vertices are homothety classes of $\mathbb{Z}_p$-lattices in $\mathbb{Q}_p^2$.
- **Bruhat–Tits buildings** of reductive groups over non-archimedean local fields are affine, e.g. lattice classes for $SL_n(K)$, of type $\widetilde{A}_{n-1}$.

# Key results

- **Strongly transitive actions ↔ BN-pairs.** If $G$ has a BN-pair, $\Delta(G,B)$ is a thick building with strongly transitive $G$-action. Conversely, such an action yields a BN-pair. See [[BN-pair BN对 BN-paire|BN-pair]].
- **Retractions.** For an apartment $\Sigma\ni C$, the retraction $\rho_{\Sigma,C}:\Delta\to\Sigma$ is a distance-nonincreasing simplicial map. It is the basic tool for (B1)–(B2) arguments and for the Iwasawa/Cartan decompositions in the affine case.
- **Solomon–Tits theorem.** A spherical building of rank $n$ has the homotopy type of a wedge of $(n-1)$-spheres, with one sphere for each chamber opposite a fixed chamber $C$ (equivalently, for each apartment containing $C$). For finite groups of Lie type, $G$ acts on $\tilde H_{n-1}(\Delta)$ by the Steinberg representation.
- **Geometric realization.** Affine buildings are CAT(0) (Bruhat–Tits). The Davis realization of any building is CAT(0) (Davis), hence contractible. Contractibility and Solomon–Tits drive cohomological applications, e.g. Borel–Serre duality for arithmetic and $S$-arithmetic groups.
- **Classification.** Thick irreducible spherical buildings of rank $\geq 3$ are Moufang. They are classified by Tits: they come from simple algebraic groups, classical groups and their analogues. Thick irreducible affine buildings of rank $\geq 4$ come from algebraic groups over complete discretely valued fields (Tits 1986). In rank $2$, and in rank $3$ for affine buildings, there are "exotic" examples.

# Related

- [[Combinatorics 组合数学 combinatoire|Combinatorics hub]]
- [[Coxeter system 考克斯特系统 système de Coxeter|Coxeter system]]: apartments are Coxeter complexes.
- [[BN-pair BN对 BN-paire|BN-pair]]
- [[Simplicial complex 单纯复形 complexe simplicial|Simplicial complex]]
- [[Simplicial set 单纯集 ensemble simplicial|Simplicial set]]

# References

Recommendations collected in the MathOverflow question *Any good reference for Tits Building?* (MathOverflow 74117):

- P. Abramenko, K. S. Brown, *Buildings: Theory and Applications*, GTM 248, Springer 2008. The standard reference; the first edition is K. S. Brown, *Buildings*, Springer 1989.
- J. Tits, Reductive groups over local fields, in *Automorphic Forms, Representations and L-Functions* (Corvallis 1977), Proc. Symp. Pure Math. 33, Part 1, AMS 1979. (The clipping calls this "Corvallis 1979".)
- I. G. Macdonald, *Spherical Functions on a Group of $p$-adic Type*, Ramanujan Institute, Madras 1971.
- J. Rabinoff, *The Bruhat–Tits building of a $p$-adic Chevalley group and an application to representation theory*, senior thesis, Harvard 2003. A very readable exposition.
- B. Everitt, A (very short) introduction to buildings, arXiv:1207.2266. Has many pictures and pointers to the literature.
- J. Tits, *Buildings of Spherical Type and Finite BN-Pairs*, LNM 386, Springer 1974. Essentially combinatorial, so it can be read without algebraic groups.
- R. M. Weiss, *The Structure of Spherical Buildings*, Princeton 2003; *The Structure of Affine Buildings*, Ann. of Math. Stud. 168, Princeton 2009.
- M. Ronan, *Lectures on Buildings*, Academic Press 1989; updated ed. Univ. Chicago Press 2009. Suited to beginners.

Further: M. W. Davis, *The Geometry and Topology of Coxeter Groups*, Princeton 2008 (Ch. 18, buildings).
