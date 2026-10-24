---
aliases:
  - quotient root system
  - système de racines quotient
summary: 根系模去一个抛物子根系 Φ_J 后在商空间中的像，对应 Levi 分解下的 grading
---
# Definition

Let $\Phi$ be a finite crystallographic root system in a Euclidean space $(V,(-,-))$ with base $\Delta$, positive roots $\Phi^+$ and Weyl group $W$. For $J\subseteq\Delta$ put $V_J:=\mathbb{R}J$ and $\Phi_J:=\Phi\cap V_J$. $\Phi_J$ is the parabolic subsystem with base $J$ and Weyl group $W_J$. Let $\pi:V\to V/V_J$ be the projection. The **quotient root system** (商根系) of $\Phi$ by $J$ is
$$\Phi/J:=\pi(\Phi\setminus\Phi_J)\subseteq V/V_J,\qquad (\Phi/J)^+:=\pi(\Phi^+\setminus\Phi_J^+).$$
Identifying $V/V_J\cong V_J^{\perp}$, $\pi$ becomes orthogonal projection, which gives $\Phi/J$ an inner product. Elements of $\Phi/J$ are also called **$\mathfrak{t}$-roots** (Kostant) or **restricted roots** in the situations below. The fibre $\pi^{-1}(\lambda)\cap\Phi$ has cardinality the **multiplicity** of $\lambda$.

> [!note] Terminology
> "Quotient root system" is not used uniformly in the literature. The definition here, the image of a root system modulo a parabolic subsystem, is the one compatible with Levi decompositions and relative root systems. Dimitrov–Fioresi axiomatize such images as *generalized root systems*.

# Examples

- **$B_2$**, base $\{\alpha,\beta\}$ with $\alpha$ long, $\Phi^+=\{\beta,\alpha,\alpha+\beta,\alpha+2\beta\}$.
  - $J=\{\beta\}$: all of $\alpha,\alpha+\beta,\alpha+2\beta$ map to $\bar\alpha$, so $\Phi/J=\{\pm\bar\alpha\}$ ($A_1$, multiplicity $3$).
  - $J=\{\alpha\}$: $\beta,\alpha+\beta\mapsto\bar\beta$ and $\alpha+2\beta\mapsto 2\bar\beta$, so $\Phi/J=\{\pm\bar\beta,\pm2\bar\beta\}$, the **non-reduced** system $BC_1$.
- **$A_3$**, $J=\{\alpha_2\}$: $(\Phi/J)^+=\{\bar\alpha_1,\bar\alpha_3,\bar\alpha_1+\bar\alpha_3\}$ with multiplicities $2,2,1$. Combinatorially this is $A_2$, but metrically it is not. With $(\alpha_i,\alpha_i)=2$ the projections onto $\alpha_2^\perp$ are $\alpha_1+\tfrac12\alpha_2$ and $\alpha_3+\tfrac12\alpha_2$, each of squared length $\tfrac32$, with inner product $-\tfrac12$. The angle is $\arccos(-\tfrac13)\neq\tfrac{2\pi}{3}$, so $\Phi/J$ is **not a root system** in $V_J^\perp$.
- **$J=\emptyset$** gives $\Phi$. **$J=\Delta\setminus\{\alpha_i\}$** gives $\Phi/J\subseteq\{\pm\bar\alpha_i,\pm2\bar\alpha_i,\dots\}$, which records the grading of $\mathfrak{g}$ by the coefficient of $\alpha_i$ (e.g. $\{\pm\bar\alpha_i\}$ for cominuscule $\alpha_i$).

# Properties

- $\Phi/J$ is finite, $\Phi/J=-\Phi/J$, $\Phi/J=(\Phi/J)^+\sqcup-(\Phi/J)^+$, and $\pi(\Delta\setminus J)$ is a basis of $V/V_J$ such that every element of $(\Phi/J)^+$ is a nonnegative integer combination of it. So $\Phi/J$ has a "base". In general, however, it is neither reduced nor stable under the reflections it defines. The reflection-stability fails in the $A_3$ example.
- **Lie-theoretic meaning.** Let $\mathfrak{g}$ be semisimple with Cartan $\mathfrak{h}$, $\mathfrak{l}_J=\mathfrak{h}\oplus\bigoplus_{\alpha\in\Phi_J}\mathfrak{g}_\alpha$ the Levi, and $\mathfrak{t}=\mathfrak{z}(\mathfrak{l}_J)$. Then $\mathfrak{t}^*\cong V/V_J$ (over $\mathbb{R}$, on the real span), and
$$\mathfrak{g}=\mathfrak{l}_J\oplus\bigoplus_{\lambda\in\Phi/J}\mathfrak{g}_\lambda,\qquad \mathfrak{g}_\lambda=\bigoplus_{\pi(\alpha)=\lambda}\mathfrak{g}_\alpha .$$
Each $\mathfrak{g}_\lambda$ is an **irreducible** $\mathfrak{l}_J$-module (Kostant), of dimension the multiplicity of $\lambda$. Also $[\mathfrak{g}_\lambda,\mathfrak{g}_\mu]=\mathfrak{g}_{\lambda+\mu}$ when $\lambda,\mu,\lambda+\mu\in\Phi/J$. The nilradical of the parabolic $\mathfrak{p}_J$ is $\mathfrak{u}_J=\bigoplus_{\lambda\in(\Phi/J)^+}\mathfrak{g}_\lambda$.
- **Relative root systems.** Let $\mathbf{G}$ be a reductive group over $k$ that is an inner form of a split group (trivial $*$-action on the Tits index), and let $J$ be the set of anisotropic (black) simple roots. Then $\Phi/J$ is the relative root system ${}_k\Phi$ with respect to a maximal split torus, and by Borel–Tits it **is** a root system, possibly non-reduced (e.g. $BC_q$ for $Sp(p,q)$, $p>q$, an inner form of type $C_{p+q}$). The same holds for restricted roots of real forms via Satake diagrams. For outer forms one must also fold by the $*$-action. Its Weyl group ${}_kW$ is the Weyl group of the BN-pair in $\mathbf{G}(k)$ (see [[BN-pair BN对 BN-paire|BN-pair]]).
- **Weyl group.** $N_W(W_J)$ preserves $\Phi_J$ and $V_J$, hence acts on $\Phi/J$, and $W_J$ acts trivially. Howlett: $N_W(W_J)=W_J\rtimes N_J$ with $N_J=\{w\in W: wJ=J\}$. In general $N_J$ is not a reflection group (Howlett; Brink–Howlett).
- On the Coxeter side, the corresponding quotient is the set $W^J$ of minimal coset representatives (see [[Coxeter system 考克斯特系统 système de Coxeter|Coxeter system]]). For $w\in W^J$ one has $w(\Phi_J^+)\subseteq\Phi^+$, so all inversions $\{\alpha\in\Phi^+: w\alpha\in\Phi^-\}$ of $w$ lie in $\Phi^+\setminus\Phi_J^+$.

# Related

- [[Combinatorics 组合数学 combinatoire|Combinatorics hub]]
- [[Coxeter system 考克斯特系统 système de Coxeter|Coxeter system]]
- [[BN-pair BN对 BN-paire|BN-pair]]: parabolic subgroups $P_J$ and Levi decomposition.
- [[Building 建筑 immeuble|Building]]: links of type $J$ simplices.
- [[Quiver 箭图 carquois|Quiver]]: dimension vectors of indecomposables over Dynkin quivers are the positive roots (Gabriel).

# References

- N. Bourbaki, *Groupes et algèbres de Lie*, Ch. VI (systèmes de racines).
- J. E. Humphreys, *Reflection Groups and Coxeter Groups*, CUP 1990, Ch. 1, 5.
- A. Borel, J. Tits, Groupes réductifs, *Publ. Math. IHÉS* 27 (1965), §5–6 (relative root systems).
- B. Kostant, Root systems for Levi factors and Borel–de Siebenthal theory, in *Symmetry and Spaces*, Progr. Math. 278, Birkhäuser 2010.
- R. B. Howlett, Normalizers of parabolic subgroups of reflection groups, *J. London Math. Soc.* (2) 21 (1980).
- I. Dimitrov, R. Fioresi, Generalized root systems, preprint (2023), arXiv.
