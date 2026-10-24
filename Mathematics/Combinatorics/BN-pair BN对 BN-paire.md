---
aliases:
  - bn-pair
  - BN-paire
  - Tits system
  - système de Tits
summary: 群中满足 Bruhat 型公理的子群对 (B,N)，给出 Bruhat 分解与 building
---
# Definition

A **BN-pair** (BN对), or **Tits system** (système de Tits), in a group $G$ is a quadruple $(G,B,N,S)$ where $B,N\leq G$ are subgroups and $S\subseteq W:=N/T$ with $T:=B\cap N$, such that

- (BN1) $G=\langle B,N\rangle$ and $T\trianglelefteq N$;
- (BN2) $S$ generates $W$ and consists of involutions;
- (BN3) $sBw\subseteq BwB\cup BswB$ for all $s\in S$, $w\in W$;
- (BN4) $sBs\neq B$ for all $s\in S$.

Since $T\subseteq B$, double cosets $BwB:=B\dot wB$ are independent of the lift $\dot w\in N$. $W$ is the **Weyl group** and $|S|$ is the **rank**. A subgroup conjugate to some $P_J$ below is called **parabolic**.

# Examples

- $G=GL_n(k)$ for a field $k$: $B$ is the upper triangular matrices, $N$ the monomial matrices, $T$ the diagonal matrices, $W\cong S_n$, and $S$ the adjacent transpositions. Then $BwB$ consists of the invertible matrices whose "pivot pattern" is the permutation $w$ (Gaussian elimination).
- More generally $G=\mathbf{G}(k)$ for a connected reductive $k$-group: $B=\mathbf{P}(k)$ a minimal parabolic $k$-subgroup, $N=N_{\mathbf{G}}(\mathbf{S})(k)$ for a maximal $k$-split torus $\mathbf{S}\subseteq\mathbf{P}$, and $W={}_kW$ the relative Weyl group (Borel–Tits). Finite groups of Lie type, twisted ones included, are of this kind. This is the input for the classification of finite simple groups.
- **Affine BN-pair.** $G=SL_n(K)$ with $K$ non-archimedean local, $\mathcal{O}\subseteq K$ its valuation ring, $\varpi$ a uniformizer. $B$ is the **Iwahori subgroup**, the preimage under $SL_n(\mathcal{O})\to SL_n(\mathcal{O}/\varpi)$ of the upper triangular matrices. $N$ is the monomial matrices in $G$, and $W=N/T\cong\mathbb{Z}^{n-1}\rtimes S_n$ is the affine Weyl group of type $\widetilde{A}_{n-1}$. (For $GL_n(K)$ one gets the *extended* affine Weyl group, which is not a Coxeter group. One then uses a "generalized" Tits system.)
- Kac–Moody groups carry two BN-pairs $(B_+,N)$, $(B_-,N)$ forming a **twin BN-pair**.

# Key results

- **$(W,S)$ is a [[Coxeter system 考克斯特系统 système de Coxeter|Coxeter system]]** (Bourbaki IV §2.4).
- **Bruhat decomposition.** $G=\bigsqcup_{w\in W}BwB$, and $BsB\cdot BwB=BswB$ if $\ell(sw)=\ell(w)+1$.
- **Parabolic subgroups.** For $J\subseteq S$, $P_J:=BW_JB$ is a subgroup. $J\mapsto P_J$ is an inclusion-preserving bijection from subsets of $S$ to subgroups of $G$ containing $B$. The $P_J$ are self-normalizing and pairwise non-conjugate. $P_I\cap P_J=P_{I\cap J}$.
- **The building.** Let $\Delta(G,B)$ be the poset of cosets $gP_J$ ($g\in G$, $J\subsetneq S$) under reverse inclusion. It is a thick [[Building 建筑 immeuble|building]] of type $(W,S)$. Its chambers are $G/B$ and its standard apartment is $\{nP_J\}_{n\in N}\cong\Sigma(W,S)$. $G$ acts **strongly transitively**, i.e. transitively on pairs (apartment, chamber in it). Conversely, a strongly transitive type-preserving action on a thick building gives a BN-pair, with $B$ the stabilizer of a chamber $C$ and $N$ the stabilizer of an apartment $\Sigma\ni C$. So BN-pairs and strongly transitive actions on buildings are essentially the same thing. Here $W$-distance is $\delta(gB,hB)=w\iff g^{-1}h\in BwB$.
- **Tits' simplicity theorem.** Suppose $(W,S)$ is irreducible, $G$ is perfect, and $B=U\rtimes T$ with $U$ solvable and $\bigcup_g gUg^{-1}$ generating $G$. Then every normal subgroup of $G$ is either contained in $Z:=\bigcap_g gBg^{-1}$ or equal to $G$, so $G/Z$ is simple when $G/Z$ is nontrivial. This applies to $PSL_n(k)$ and to Chevalley groups.
- **Double Bruhat cells.** With an opposite Borel $B_-$, $G^{u,v}:=BuB\cap B_-vB_-$. These cells carry (upper) cluster algebra structures (Berenstein–Fomin–Zelevinsky). Cluster algebras from double Bruhat cells are among the examples where the dg Higgs category is not concentrated in degree $0$ (cf. [[ICRA 2026 Abstract]]).

# Related

- [[Combinatorics 组合数学 combinatoire|Combinatorics hub]]
- [[Coxeter system 考克斯特系统 système de Coxeter|Coxeter system]]
- [[Building 建筑 immeuble|Building]]
- [[Quotient root system 商根系 système de racines quotient|Quotient root system]]: Levi decompositions of $P_J$.
- [[Quiver 箭图 carquois|Quiver]]

# References

- N. Bourbaki, *Groupes et algèbres de Lie*, Ch. IV §2 (Systèmes de Tits).
- P. Abramenko, K. S. Brown, *Buildings: Theory and Applications*, GTM 248, Springer 2008, Ch. 6.
- J. Tits, *Buildings of Spherical Type and Finite BN-Pairs*, LNM 386, Springer 1974.
- M. Ronan, *Lectures on Buildings*, Academic Press 1989 (updated ed. Univ. Chicago Press 2009).
- R. W. Carter, *Simple Groups of Lie Type*, Wiley 1972.
- A. Berenstein, S. Fomin, A. Zelevinsky, Cluster algebras III: Upper bounds and double Bruhat cells, *Duke Math. J.* 126 (2005).
