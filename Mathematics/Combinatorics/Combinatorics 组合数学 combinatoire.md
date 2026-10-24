---
aliases:
  - combinatorics
  - combinatoire
summary: Combinatorics 文件夹的 hub：Coxeter 群、BN-pair、building、根系、单纯结构与箭图
---
# Overview

Combinatorics (组合数学) here means the discrete structures underlying Lie theory and representation theory, not enumerative combinatorics per se. The pages in this folder fit into three lines.

1. **Reflection groups and their geometry.** A Coxeter system $(W,S)$ is the combinatorial shadow of a root system. A group with a BN-pair has $(W,S)$ as its Weyl group. Its geometry is a building, glued from copies of the Coxeter complex $\Sigma(W,S)$.
2. **Simplicial structures.** Coxeter complexes, buildings and cluster complexes are simplicial complexes. Simplicial sets are their homotopy-theoretic generalization, and they are the language of nerves, $\infty$-categories and dg nerves.
3. **Quivers.** Dynkin and Coxeter diagrams reappear as quivers. Gabriel's theorem identifies indecomposables over Dynkin quivers with positive roots, and quivers with potential feed into cluster categories and Higgs categories.

Schematically:
$$\text{root system }\Phi\ \leadsto\ (W,S)\ \leadsto\ \Sigma(W,S)\ \subseteq\ \text{building }\Delta(G,B)\ \longleftarrow\ (G,B,N,S).$$

# Pages

## Coxeter groups and root systems
- [[Coxeter system 考克斯特系统 système de Coxeter|Coxeter system]]: presentation by involutions and braid relations. It covers the classification of finite types ($A$–$I_2(m)$), parabolic subgroups $W_J$, and the link to Dynkin quivers.
- [[Quotient root system 商根系 système de racines quotient|Quotient root system]]: the image $\Phi/J$ of a root system modulo a parabolic subsystem $\Phi_J$. It gives the grading of $\mathfrak{g}$ attached to a parabolic $\mathfrak{p}_J$, and relative root systems. It is in general not itself a root system.

## Groups and geometries
- [[BN-pair BN对 BN-paire|BN-pair]] (Tits system): axioms on $(G,B,N,S)$. They give the Bruhat decomposition $G=\bigsqcup_w BwB$, the parabolic subgroups $P_J$, and Tits' simplicity theorem. Its Weyl group is a Coxeter system.
- [[Building 建筑 immeuble|Building]]: a simplicial complex covered by apartments that are Coxeter complexes (simplicial or $W$-metric definition). BN-pairs are the same as strongly transitive actions on buildings. Spherical, affine (Bruhat–Tits) and rank-2 (generalized polygons) cases.

## Simplicial structures
- [[Simplicial complex 单纯复形 complexe simplicial|Simplicial complex]]: an abstract simplicial complex and its geometric realization. Examples are order complexes, nerves, Coxeter complexes and the Fomin–Zelevinsky cluster complex.
- [[Simplicial set 单纯集 ensemble simplicial|Simplicial set]]: a functor $\Delta^{\mathrm{op}}\to\mathbf{Set}$. Topics are nerves, Kan complexes, quasi-categories, Dold–Kan and the dg nerve of a dg category.

## Quivers
- [[Quiver 箭图 carquois|Quiver]]: the user's notes on quivers with extra structure (valued, translation, ice quivers), relative preprojective and relative Ginzburg dg algebras, and Higgs categories. Its underlying graphs connect to Coxeter/Dynkin diagrams via Gabriel's theorem and reflection functors.

# Related

- [[Metamathematics 元数学 métamathématique|Metamathematics]]

# References

- N. Bourbaki, *Groupes et algèbres de Lie*, Ch. IV–VI.
- J. E. Humphreys, *Reflection Groups and Coxeter Groups*, CUP 1990.
- P. Abramenko, K. S. Brown, *Buildings: Theory and Applications*, GTM 248, Springer 2008.
- P. G. Goerss, J. F. Jardine, *Simplicial Homotopy Theory*, Birkhäuser 1999.
