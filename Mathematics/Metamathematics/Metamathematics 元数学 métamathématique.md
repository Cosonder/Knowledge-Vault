---
aliases:
  - metamathematics
  - métamathématique
summary: 以数学方法研究数学理论本身：证明论、模型论、可计算性、集合论基础
---
# Definition

**Metamathematics** (元数学) is the mathematical study of mathematical theories themselves. Formal theories $T$ (a language, axioms and a deductive calculus) become objects of study, and one proves theorems *about* $T$: consistency, completeness, decidability, independence, and the strength of $T$ relative to other theories. The term goes back to Hilbert. Today it is distributed over **proof theory**, **model theory**, **computability theory** and **set theory**, which together make up mathematical logic.

# Overview

## Hilbert's programme
Around 1920 Hilbert proposed to formalize mathematics (e.g. analysis, set theory) in a formal system $T$. The goal was to prove the **consistency** of $T$ by **finitary** means, i.e. combinatorial reasoning about finite strings of symbols. This would secure "ideal" infinitary mathematics by "real" finitary mathematics. In its original form the programme was refuted by Gödel's second incompleteness theorem. Relativized versions survive in proof theory and reverse mathematics.

## Gödel
- **Completeness theorem** (1929). For a first-order theory $T$, $T\vdash\varphi$ iff $T\models\varphi$, i.e. $\varphi$ holds in every model of $T$. Syntax and semantics agree.
- **First incompleteness theorem** (1931; Rosser 1936 for simple consistency). If $T$ is consistent, recursively axiomatizable and interprets enough arithmetic (e.g. Robinson's $Q$), then there is a sentence $G_T$ with $T\nvdash G_T$ and $T\nvdash\neg G_T$.
- **Second incompleteness theorem.** For such $T$ (extending e.g. $\mathrm{PA}$, with a standard provability predicate), $T\nvdash\mathrm{Con}(T)$.
- Related: **Tarski's undefinability of truth**, and the **Church–Turing** negative solution of the *Entscheidungsproblem* (1936). First-order validity is semi-decidable but not decidable.

## Proof theory
Proof theory studies formal derivations as combinatorial objects. **Gentzen** introduced natural deduction and sequent calculus and proved **cut elimination**. In 1936 he proved $\mathrm{Con}(\mathrm{PA})$ using transfinite induction up to $\varepsilon_0$ for quantifier-free predicates. This starts **ordinal analysis**, where the proof-theoretic ordinal of $\mathrm{PA}$ is $\varepsilon_0$. Other branches are reverse mathematics (the systems $\mathrm{RCA}_0$, $\mathrm{WKL}_0$, $\mathrm{ACA}_0$, …), and the Curry–Howard correspondence between proofs and programs, which underlies type theories and proof assistants (Lean, Coq/Rocq).

## Model theory
Model theory studies the relation between theories and their models. Its basic results are **compactness** and **Löwenheim–Skolem**: a countable theory with an infinite model has models of every infinite cardinality, so first-order theories cannot pin down infinite structures up to isomorphism. Further topics are quantifier elimination (Tarski: real closed fields; algebraically closed fields), Morley's categoricity theorem, and stability theory (Shelah). Applications in algebra and geometry include Ax–Grothendieck and Hrushovski's proof of the function-field Mordell–Lang conjecture.

## Set-theoretic foundations
$\mathrm{ZFC}$ is the standard foundation. **Gödel** (1938) showed with the constructible universe $L$ that $\mathrm{Con}(\mathrm{ZF})\Rightarrow\mathrm{Con}(\mathrm{ZFC}+\mathrm{GCH})$. **Cohen** (1963) showed with **forcing** that $\mathrm{Con}(\mathrm{ZF})\Rightarrow\mathrm{Con}(\mathrm{ZFC}+\neg\mathrm{CH})$ and $\mathrm{Con}(\mathrm{ZF}+\neg\mathrm{AC})$. Hence CH and AC are independent. Large cardinal axioms measure consistency strength. By the second incompleteness theorem, ZFC (if consistent) cannot prove that an inaccessible cardinal exists, since $V_\kappa\models\mathrm{ZFC}$ for inaccessible $\kappa$.

For working mathematicians the relevant point is **size**. Categories such as $\mathcal{D}(A)$, or "the category of all small dg categories", need a convention: classes (NBG/MK), or **Grothendieck universes**, which are equivalent to inaccessible cardinals and lie beyond ZFC. Localizations of non-small categories need not have small Hom-sets. This is the reason for the standing hypothesis "small dg category" in derived Morita theory. Alternative foundations are Lawvere's ETCS, homotopy type theory (univalent foundations), and Feferman's and Shulman's set-theoretic treatments of category theory.

# Remarks

The user's remark on writing mathematics in Obsidian (kept verbatim):

> Since in Obsidian we use markdown, it's not very wieldy to write latex code here (at least at present). So I will mainly focus on describing using natural languages. 

(The vault now renders LaTeX via `$…$` / `$$…$$`, see `CLAUDE.md`.)

# Related

- [[Combinatorics 组合数学 combinatoire|Combinatorics hub]]
- [[Simplicial set 单纯集 ensemble simplicial|Simplicial set]]: homotopy type theory has simplicial-set models (Voevodsky's Kan simplicial set model).

# References

- K. Gödel, Über formal unentscheidbare Sätze der *Principia Mathematica* und verwandter Systeme I, *Monatsh. Math. Phys.* 38 (1931).
- S. C. Kleene, *Introduction to Metamathematics*, North-Holland 1952.
- J.-Y. Girard, *Proof Theory and Logical Complexity*, Bibliopolis 1987; G. Takeuti, *Proof Theory*, 2nd ed., North-Holland 1987.
- D. Marker, *Model Theory: An Introduction*, GTM 217, Springer 2002.
- K. Kunen, *Set Theory*, College Publications 2011; T. Jech, *Set Theory*, 3rd millennium ed., Springer 2003.
- P. Smith, *An Introduction to Gödel's Theorems*, 2nd ed., CUP 2013.
- M. Shulman, Set theory for category theory, arXiv:0810.1279.
