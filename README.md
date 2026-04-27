# Alban Reynaud Michez
Contact: **alban DOT reynaud AT univ DASH grenoble DASH alpes DOT fr**

## About
I am a PhD student in computer science, specifically in the formal study of programming languages.
I am working at [Verimage laboratory](https://www-verimag.imag.fr), Grenoble. My supervisors are [Sylvain Boulmé](https://www-verimag.imag.fr/~boulme/) and [David Monniaux](https://www-verimag.imag.fr/~monniaux/).

## PhD work

LLBC (_low-level borrow-calculus_) is a model of Rust that is centered around borrows. It was intially introduced for the purpose of the [Aeneas verification project](github.com/AeneasVerif/aeneas). In an [ICFP'24 article](https://dl.acm.org/doi/10.1145/3674640), Ho, Fromherz and Protzenko studied LLBC. The connected it with an execution model on a heap, specified a borrow-checker (with a symbolic semantics), and proved its soundness.

**My PhD project consists in formalizing this work in the Rocq prover**. I proved key results about the soundness of LLBC on a minimal fragment, containing mutable borrows, conditionals and loops. This effort lead me to identify a missing argument in the original proof, and to propose a fix. The code is available [here](https://github.com/AeneasVerif/mechanized-llbc). In [this preprint](https://hal.science/hal-05527340) we detail the introduced techniques.

With Vincent Rébiscoul, we are working on adding a CompCert backend to this formalization, as a way to have a proof-of-concept certified compiler with a borrow-checker for Rust. This formalization could also serve to prove the soundness of the functional translation of Aeneas.

## Articles
### International Conferences
[**Modular verification of op-based CRDTs in separation logic**](https://dl.acm.org/doi/10.1145/3563351) \
Abel Nieto, Léon Gondelman, Alban Reynaud, Amin Timany and Lars Birkedal, Oopsla 2022.

[**A Practical Mode System for Recursive Definitions**](https://dl.acm.org/doi/pdf/10.1145/3434326) \
Alban Reynaud, Gabriel Scherer and Jeremy Yallop, POPL 2021.

[**Verifying a Solver for Linear Mixed Integer Arithmetic in Isabelle/HOL**](https://link.springer.com/chapter/10.1007%2F978-3-030-55754-6_14) \
Ralph Bottesch, Max W. Haslbeck, Alban Reynaud and René Thiemann, NFM 2020.

### National Conferences
**[Formal Verification of Borrow-Checking by Local Commutation Diagram](https://hal.science/hal-05428143)** \
Alban Reynaud Michez, JFLA 2026.

This article is completed by the following preprint. I recommand to refer it instead:

**[Mechanizing the proof of a borrow calculus](https://hal.science/hal-05527340)** \
Alban Reynaud Michez, 2026.
