---
date: 2026-04-29
aliases:
  - quiver
tags:
---
# Basic construction

## path algebra


\subsection{Quiver with structures}

One should pense on the question that which type of a new concept lies in, a new property, an extra structure or an extra stuff. For example, on first thought, graded quiver, valued quiver, quiver with translation, valued quiver with translation, quiver with potential should be quiver with extra structure, while ice quiver should be quiver with extra stuff, and ice qiuver with potential should be a hybrid.

\subsubsection{Valued quiver}

\begin{definition}

A valued quiver is a triple $Q=(Q_0,d,d')$ consisting of

\begin{compactitem}

\item $Q_0$: a set of vertices,

\item $d,d':Q_0\times Q_0\rightarrow\N$.

\end{compactitem}

Denote by $d_{ij}=d(i,j),d'_{ij}=d'(i,j)$ for $i,j\in Q_0$.

  

A morphism $f:Q\rightarrow\Gamma$ between value quivers is a morphism of quivers which preserves the valuation, i.e.,

  

The valued quivers and morphisms between them forms a category $\cate{vQui}$

\end{definition}

\begin{remark}

To draw the diagram of a valued quiver we use a labeled arrow between each pair of vertices $(i,j)\in Q_0^2$ s.t. $d_{ij},d'_{ij}>0$,

$$i\xrightarrow{(d_{ij},d'_{ij})} j$$.

\end{remark}

  

\begin{construction}

The underlying quiver of a valued quiver. As we can see, there is no set of arrow a priori in the definition of a valued quiver.

\end{construction}

  
  

\begin{definition}

A value quiver $Q$ is called

\begin{compactitem}

\item locally finite if $\forall i\in Q_0, \sum_{j\in Q_0}d_{ji}<\infty,\sum_{j\in Q_0}d'_{ij}<\infty$,

\item symmetrizable if $\exists c:Q_0\rightarrow\N_+$ called a symmetrizer s.t. $\forall i,j\in Q_0, c_id_{ij}=d'_{ij}c_j$.

\end{compactitem}

\end{definition}

  

\begin{construction}(the Auslander-Reiten quiver of a Krull-Schmidt additive category)

  

Let $\mathcal{C}$: Krull-Schmidt additive category, $\ind\mathcal{C}$: isomorphism classes of indecomposable objects.

  

For $X,Y\in\ind\mathcal{C}$,

  

$D_X:=(\mathcal{C}/\rad\mathcal{C})(X,Y)$ is a division ring,

  
  

\end{construction}

  

\subsubsection{Translation quiver}

\begin{definition}

A translation quiver $\Gamma=(\Gamma_0,\Gamma_1,s,t,\sigma,\tau,\Gamma_0')$ consists of

\begin{compactitem}

\item $(\Gamma_0,\Gamma_1,s,t)$ is a locally finite quiver without loops,

\item $\Gamma_0'\subseteq\Gamma_0$, $\Gamma_0':=t^{-1}(\Gamma_0')$,

\item $\tau: \Gamma_0'\rightarrow\Gamma_0$ is an injective map s.t. $\forall x\in\Gamma_0, y\in\Gamma_0'$ we have $|\Gamma_1(x,y)|=|\Gamma_1(\tau(y),x)|$,

\item $\sigma:\Gamma_1'\rightarrow\Gamma_1$ is an injective map s.t. $\forall x\in\Gamma_0, y\in\Gamma_0',\alpha\in\Gamma_1(x,y)$ we have $\sigma(\alpha)\in\Gamma_1(\tau(y),x)$.

\end{compactitem}

The map $\tau$ is called the translation of $\Gamma$,

  

$\sigma$ is called the polarization (or semitranslation) of $\Gamma$,

  

elements in $\Gamma_0\backslash\Gamma_0'$ are called the projective vertices, and

  

elements in $\Gamma_0\backslash\tau(\Gamma_0')$ are called the injective vertices.

  

$\Gamma$ is called stable if $\Gamma_0=\Gamma_0'=\tau(\Gamma_0)$.

  

\end{definition}

\begin{remark}

\begin{compactenum}

\item The translation should be considered as a bijective map $\tau:\Gamma_0'\rightarrow\tau(\Gamma_0')=:\Gamma_0''$ from the set of non-projective vertices to the set of non-injective vertices with inverse $\tau^{-1}:\Gamma_0''\rightarrow\Gamma_0'$.

\item If $\Gamma$ has no multiple arrows, then the polarization is uniquely determined by the translation.

\end{compactenum}

\end{remark}

  

\begin{proposition}

Let $Q$ be a quiver. Then the repetition quiver $\Z Q$ is a stable translation quiver.

\end{proposition}

\subsubsection{Valued translation quiver}

  
  
  

\subsubsection{Ice quiver}

\begin{definition}

An ice quiver is a pair $(Q,F)$ where

\begin{compactitem}

\item $Q$ is a quiver,

\item $F\subseteq Q$ is a subquiver, called the frozen subquiver.

\end{compactitem}

Elements of $F_0$ (resp. $F_1$) are called the frozen vertices (resp. frozen arrows). Elements of $Q_0\backslash F_0$ (resp. $Q_1\backslash F_1$) are called the unfrozen (or mutable) vertices (resp. unfrozen arrows).

  

The unfrozen part $\underline{Q}$ is the full subquiver of $Q$ on the unfrozen vertices, i.e., obtained by removing all the frozen vertices and arrows with frozen source or target.

\end{definition}

\begin{remark}

$F$ is not necessarily a full subquiver.

\end{remark}

  
  
  

\begin{construction}(the relative preprojective algebra,\cite{kellerRelativeCalabiYauStructures2023})

  

Let $(Q,F)$ be a (finite) ice quiver, $k$ a field.

Define a quiver $\widetilde{Q_F}$ as follows:

\begin{compactenum}

\item the vertices: $\widetilde{Q}_0:=Q_0$,

\item the arrows $\widetilde{Q}_1$ consists of 2 disjoint part:

\begin{compactenum}

\item the arrows of $Q$,

\item an arrow $a^*:j\rightarrow i$ for each arrow $a:i\rightarrow j$,

\end{compactenum}

\end{compactenum}

Define the relative preprojective algebra associated with $(Q,F)$, as the quotient of the complete graded path algebra $\widehat{k\widetilde{Q_F}}$ by

the closure of the ideal generated by the

$$e_i(\sum_{a\in Q_1}[a,a^*])e_i,$$

where $i$ runs through the unfrozen vertices.

\end{construction}

\begin{remark}

The notation $\Pi_2(Q)$ might not be standard.

\end{remark}

  
  

\begin{construction}(the relative derived preprojective algebra)

  

Let $(Q,F)$ be a (finite) ice quiver, $k$ a field.

Define a graded quiver $\widetilde{Q_F}$ as follows:

\begin{compactenum}

\item the vertices: $\widetilde{Q}_0:=Q_0$,

\item the arrows $\widetilde{Q}_1$ consists of three disjoint part:

\begin{compactenum}

\item the arrows of $Q$ (of degree 0),

\item an arrow $a^*:j\rightarrow i$ of degree $0$ for each unfrozen arrow $a:i\rightarrow j$,

\item a loop $t_i: i\rightarrow i$ of degree $-1$ for each vertex $i$.

\end{compactenum}

\end{compactenum}

Define the relative derived preprojective algebra as the dg $k$-algebra with underlying graded algebra the complete graded path algebra $\widehat{k\widetilde{Q_F}}$ and with differential given as the unique $k$-linear continuous endomorphism of degree $1$ which satisfies the graded Leibniz rule

$$d(uv)=d(u)v+(-1)^{|u|}ud(v)$$

for all homogeneous $u,v$, and takes the following values on the arrows of $\widetilde{Q}$:

\begin{compactitem}

\item $d(a)=0$ for each $a\in Q_1$,

\item $d(a^*)=0$ for each unfrozen $a\in Q_1$,

\item $d(t_i)=e_i(\sum_{a\in Q_1}[a,a^*])e_i$ for each vertex $i$.

\end{compactitem}

\end{construction}

\begin{remark}

This lacks a reference.

\end{remark}

  
  

\subsubsection{Quiver with potential}

See \cite{derksenQuiversPotentialsTheir2008,derksenQuiversPotentialsTheir2010,presslandMutationFrozenJacobian2020}

\begin{definition}

  

Let $Q$ be a finite quiver, $k$ a field. A potential on $Q$ is an element $W\in \HH_0(\widehat{kQ})$ expressible as a (possibly infinite) linear combination of homogeneous elements of degree at least 2, such that any term involving a loop has degree at least 3.

  

A quiver with potential is a pair $(Q,W)$ where

\begin{compactitem}

\item $Q$ is a finite quiver,

\item $W\in \HH_0(\widehat{kQ})$ is a potential on $Q$.

\end{compactitem}

\end{definition}

\begin{remark}

A potential can be thought of as a formal linear combination of cyclic paths in $Q$ (of length at least 2), considered up to the equivalence relation on such cycles induced by

$$\alpha_n\cdots\alpha_1\sim\alpha_{n-1}\cdots\alpha_1\alpha_n.$$

\end{remark}

  

\begin{construction}(the cyclic derivative, the Jacobian algebra)

  

Fix $\alpha\in Q_1$. Let $p=\alpha_n\cdots\alpha_1$ be a cyclic path, where each $\alpha_i\in Q_1$. Then the cyclic derivative of $p$ w.r.t. $\alpha$ is

$$\partial_\alpha p:=\sum_{\alpha_i=\alpha}\alpha_{i-1}\cdots\alpha_1\cdots\alpha_{i+1}.$$

We extended $\partial_\alpha$ by linearity and continuity and get a well-defined map

$$\partial_\alpha:\HH_0(\widehat{kQ})\rightarrow\widehat{kQ}.$$

Given a quiver with potential $(Q,W)$, define the Jacobian ideal of $\widehat{kQ}$ as

$$\overline{\langle\partial_\alpha W|\alpha\in Q_1\rangle}$$

and the Jacobian algebra as

$$J(Q,W):=\widehat{kQ}/ \overline{\langle\partial_\alpha W|\alpha\in Q_1\rangle}.$$

\end{construction}

\begin{example}

Let $Q$ be the quiver with one vertex and three loops labeled $X,Y$ and $Z$:

\[\begin{tikzcd}

\bullet

\arrow["Y"{description}, from=1-1, to=1-1, loop, in=55, out=125, distance=10mm]

\arrow["X"{description}, from=1-1, to=1-1, loop, in=60, out=120, distance=5mm]

\arrow["Z"{description}, from=1-1, to=1-1, loop, in=50, out=130, distance=15mm]

\end{tikzcd}\]

Let $W=XYZ-XZY$ (technically the equivalence class corresponding to this) be a potential. Then we compute as

\begin{align*}

\partial_X(XYZ)&=YZ,\partial_Y(XYZ)=ZX,\partial_Z(XYZ)=XY,\\

\partial_X(XZY)&=ZY,\partial_Y(XZY)=XZ,\partial_Z(XZY)=YX,\\

\partial_X(W)&=[Y,Z],\partial_Y(W)=[Z,X],\partial_Z(W)=[X,Y],

\end{align*}

hence the cyclic derivatives of $W$ yield th ecommutativity relations between $X,Y$ and $Z$, and $J(Q,W)\cong k[[X,Y,Z]]$, the algebra of power series in three variable.

  

Question: try to generalize to the case of power series in $n$ variables.

\end{example}

  

\begin{construction}(the complete Ginzburg dg algebra)

  

Let $(Q,W)$ be a (finite) quiver with potential.

Define a graded quiver $\widetilde{Q}$ as follows:

\begin{compactenum}

\item the vertices: $\widetilde{Q}_0:=Q_0$,

\item the arrows $\widetilde{Q}_1$ consists of three disjoint part:

\begin{compactenum}

\item the arrows of $Q$ (of degree 0),

\item an arrow $a^*:j\rightarrow i$ of degree $-1$ for each arrow $a:i\rightarrow j$,

\item a loop $t_i: i\rightarrow i$ of degree $-2$ for each vertex $i$.

\end{compactenum}

\end{compactenum}

Define the complete Ginzburg dg algebra $\mathbf{\Gamma}(Q,W)$ as the dg $k$-algebra with underlying graded algebra the complete graded path algebra $\widehat{k\widetilde{Q}}$ and with differential given as the unique $k$-linear continuous endomorphism of degree $1$ which satisfies the graded Leibniz rule

$$d(uv)=d(u)v+(-1)^{|u|}ud(v)$$

for all homogeneous $u,v$, and takes the following values on the arrows of $\widetilde{Q}$:

\begin{compactitem}

\item $d(a)=0$ for each $a\in Q_1$,

\item $d(a^*)=\partial_a W$ for each $a\in Q_1$,

\item $d(t_i)=e_i(\sum_{a\in Q_1}[a,a^*])e_i$ for each vertex $i$.

\end{compactitem}

\end{construction}

  

\begin{question}

Is there a quiver-free definition of the (complete) Ginzburg algebra?

\end{question}

  

\begin{example}

Let $Q$ be the following quiver with potential $W=abc$

\[\begin{tikzcd}

& 2 \\

1 && 3

\arrow["a", from=1-2, to=2-3]

\arrow["b", from=2-1, to=1-2]

\arrow["c", from=2-3, to=2-1]

\end{tikzcd}\]

Then $\widetilde{Q}$ is the following graded quiver: (I don't know how to indicate the grading)

\[\begin{tikzcd}

& 2 \\

1 && 3

\arrow["{t_2}", from=1-2, to=1-2, loop, in=55, out=125, distance=10mm]

\arrow["{b^*}"', shift right, from=1-2, to=2-1]

\arrow["a"', shift right, from=1-2, to=2-3]

\arrow["b"', shift right, from=2-1, to=1-2]

\arrow["{t_1}", from=2-1, to=2-1, loop, in=145, out=215, distance=10mm]

\arrow["{c^*}"', shift right, from=2-1, to=2-3]

\arrow["{a^*}"', shift right, from=2-3, to=1-2]

\arrow["c"', shift right, from=2-3, to=2-1]

\arrow["{t_3}", from=2-3, to=2-3, loop, in=325, out=35, distance=10mm]

\end{tikzcd}\]

The differential on $\Gamma:=\mathbf{\Gamma}(Q,W)$ is given by

$$d(a^*)=bc, d(b^*)=ca, d(c^*)=ab,$$

$$d(t_1)=cc^*-b^*b,d(t_2)=bb^*-a^*a,d(t_3)=aa^*-c^*c.$$

\end{example}

  

\subsubsection{Ice quiver with potential}

See \cite{presslandMutationFrozenJacobian2020}

\begin{definition}

An ice quiver with potential is a tuple $(Q,F,W)$ where

\begin{compactitem}

\item $(Q,F)$ is a finite ice quiver,

\item $W\in \HH_0(\widehat{kQ})$ is a potential on $Q$.

\end{compactitem}

We call $W$ irredundant if each term of $W$ includes at least one unfrozen arrow.

  

Given an ice quiver with potential $(Q,F,W)$, define the relative Jacobian ideal of $\widehat{kQ}$ as

$$\overline{\langle\partial_\alpha W|\alpha\in Q_1\backslash F_1\rangle}$$

and the relative Jacobian algebra as

$$J(Q,F,W):=\widehat{kQ}/ \overline{\langle\partial_\alpha W|\alpha\in Q_1\backslash F_1\rangle}.$$

  

An ice quiver with potential $(Q,F,W)$ is called

\begin{compactitem}

\item reduced if $W$ is irredundant and the relative Jacobian ideal is admissible.

\item trivial if its relative Jacobian algebra is a product of (possibly infinite?) copies of $k$.

\end{compactitem}

\end{definition}

\begin{remark}

Note that when $F=\varnothing$, an ice quiver with potential is just a quiver with potential, and the relative Jacobian algebra is just the Jacobian algebra.

\end{remark}

  

\begin{construction}(the complete relative Ginzburg dg algebra)

  

Let $(Q,F,W)$ be a (finite) ice quiver with potential.

Define a graded quiver $\widetilde{Q}$ as follows:

\begin{compactenum}

\item the vertices: $\widetilde{Q}_0:=Q_0$,

\item the arrows $\widetilde{Q}_1$ consists of three disjoint part:

\begin{compactenum}

\item the arrows of $Q$,

\item an arrow $a^*:j\rightarrow i$ of degree $-1$ for each unfrozen arrow $a:i\rightarrow j$,

\item a loop $t_i: i\rightarrow i$ of degree $-2$ for each unfrozen vertex $i$.

\end{compactenum}

\end{compactenum}

Define the complete relative Ginzburg dg algebra $\mathbf{\Gamma}_\rel(Q,F,W)$ as the dg $k$-algebra with underlying graded algebra the complete graded path algebra $\widehat{k\widetilde{Q}}$ and with differential given as the unique $k$-linear continuous endomorphism of degree $1$ which satisfies the graded Leibniz rule

$$d(uv)=d(u)v+(-1)^{|u|}ud(v)$$

for all homogeneous $u,v$, and takes the following values on the arrows of $\widetilde{Q}$:

\begin{compactitem}

\item $d(a)=0$ for each $a\in Q_1$,

\item $d(a^*)=\partial_a W$ for each unfrozen $a$,

\item $d(t_i)=e_i(\sum_{a\in Q_1}[a,a^*])e_i$ for each unfrozen vertex $i$

\end{compactitem}

\end{construction}

\begin{remark}

The Ginzburg algebra defined above should be called 3-dimensional, in accordance with the follwing more general construction.

\end{remark}

  

\begin{construction}(the $d$-dimensional complete relative Ginzburg dg algebra)

  

Let $(Q,F,W)$ be a (finite) ice quiver with potential, $d\in\{2,3\}$.

Define a graded quiver $\widetilde{Q_F}$ as follows:

\begin{compactenum}

\item the vertices: $\widetilde{Q_F}_0:=Q_0$,

\item the arrows $\widetilde{Q}_1$ consists of three disjoint part:

\begin{compactenum}

\item the arrows of $Q$ (of degree 0),

\item an arrow $a^*:j\rightarrow i$ of degree $2-d$ for each unfrozen arrow $a:i\rightarrow j$,

\item a loop $t_i: i\rightarrow i$ of degree $3-d$ for each unfrozen vertex $i$.

\end{compactenum}

\end{compactenum}

Define the $d$-dimensional (complete) relative Ginzburg dg algebra associated with $(Q,F,W)$ as the dg $k$-algebra with underlying graded algebra the complete graded path algebra $\widehat{k\widetilde{Q}}$ and with differential given as the unique $k$-linear continuous endomorphism of degree $1$ which satisfies the graded Leibniz rule

$$d(uv)=d(u)v+(-1)^{|u|}ud(v)$$

for all homogeneous $u,v$, and takes the following values on the arrows of $\widetilde{Q}$:

\begin{compactitem}

\item $d(a)=0$ for each $a\in Q_1$,

\item $d(a^*)=\partial_a W$ for each unfrozen $a$,

\item $d(t_i)=e_i(\sum_{a\in Q_1}[a,a^*])e_i$ for each unfrozen vertex $i$

\end{compactitem}

\begin{claim}

$d^2=0$. (since this the most general case, this check saves all the previous effort)

\end{claim}

\end{construction}

\begin{remark}

\begin{compactenum}

\item In \cite{kellerRelativeCalabiYauStructures2023} the differential on $a^*$ has a minus sign: $d(a^*)=-\partial_a W$. How to explain?

\item the 2-dimensional relative Ginzburg dg algebra = the relative derived preprojective algebra,

\item the cohomology of degree 0 of the $2$-dimensional relative Ginzburg dg algerba = the relative preprojective algebra,

\item the cohomology of degree 0 of the $3$-dimensional relative Ginzburg dg algerba = the relative Jacobian algebra,

\item

\end{compactenum}

\end{remark}

  

\begin{example}

Let $(Q,F,W)$ be the following ice quiver with potential $W=abc$:

\[\begin{tikzcd}

& \color{blue}\boxed{2} \\

\color{blue}\boxed{1} && \color{blue}\boxed{3}

\arrow["a", from=1-2, to=2-3]

\arrow["b", from=2-1, to=1-2]

\arrow["c", from=2-3, to=2-1]

\end{tikzcd}\]

Then the complete relative Ginzburg dg algebra $\Gamma:=\mathbf{\Gamma}_\rel(Q,F,W)$ has the following properties:

\begin{compactenum}

\item $\Gamma$ is connective and locally finite,

\item $H^0(\Gamma)=J_\rel(Q,F,W)$ is given by

\item $H^p(\Gamma)\neq 0$ for infinitely many $p<0$,

\item the Higgs category $\mathcal{H}$ ...,

\item for a good definition of Gorenstein projective dg modules, we should find

$$\Gproj\Gamma=\add\Gamma\subseteq\mathcal{D}(\Gamma)$$

\item $H^p(D\Gamma)\neq 0$ for infinitely many $p>0$, so $D\Gamma$ is not connective, not even right bounded.

\end{compactenum}

\end{example}

  

\begin{example}

Let $(Q,F,W)$ be the following ice quiver with potential:

\[\begin{tikzcd}[column sep={1cm,between origins}, row sep={1.732cm,between origins}]

& {\color{blue}\Box} && {\color{blue}\Box} &\\

{\color{blue}\Box} && \bullet && {\color{blue}\Box} \\

& {\color{blue}\Box} && {\color{blue}\Box}

\arrow[from=1-2, to=2-3]

\arrow[from=1-4, to=1-2]

\arrow[color=blue, from=1-4, to=2-5]

\arrow[color=blue, from=2-1, to=1-2]

\arrow[from=2-1, to=3-2]

\arrow[from=2-3, to=1-4]

\arrow[from=2-3, to=2-1]

\arrow[from=2-3, to=3-4]

\arrow[from=2-5, to=2-3]

\arrow[from=3-2, to=2-3]

\arrow[from=3-4, to=2-5]

\arrow[color=blue, from=3-4, to=3-2]

\end{tikzcd}\]

  

Let $\Gamma:=\mathbf{\Gamma}_\rel(Q,F,W)$ be the complete relative Ginzburg dg algebra and $B$ the boundary dg algebra. Then we have:

\begin{compactenum}

\item $\Gamma$ is connective and locally finite,

\item $H^0(\Gamma)=J_\rel(Q,F,W)$ is given by ???

\item $H^p(\Gamma)\neq 0$ for infinitely many $p<0$,

\item the Higgs category $\mathcal{H}_\Gamma$ ...,

\item for a good definition of Gorenstein projective dg modules, we should find

$$\mathcal{H}_\Gamma\xrightarrow{\sim}\Gproj\Gamma$$

\end{compactenum}

\end{example}