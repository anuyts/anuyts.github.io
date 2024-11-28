## Reading materials

This is a list of reading materials that I would recommend for any or all of the following reasons:

- because they're related to my research,
- because they're relevant to master thesis students,
- because I like them.

### General

* The [nLab](https://ncatlab.org) is a kind of Wikipedia for type theory and category theory. The accessibility of its articles varies wildly, but in any case it's always a good place to start looking for literature pointers.
* The [1lab](https://1lab.dev/) is a "formalised, cross-linked reference resource for cubical methods in
  Homotopy Type Theory", but also contains an [introduction to type theory](https://1lab.dev/1Lab.intro.html) and a formalization of category theory. The 1lab pages' source files are literate Agda files: they are both valid markdown and valid Cubical Agda files.
* When you've found an interesting paper, its bibliography is a good place to look for related *older* papers. Using Google Scholar or the publisher's websites, you can also get a list of *newer* papers citing the current one, thus browsing the citation graph in reverse direction.

### Introduction to Category Theory

* Categories for the Working Mathematician, by Saunders Mac Lane (1971)
* Category Theory, by Steve Awodey (2006)
* An accessible and very thorough introduction to category theory, from a viewpoint of functional programming: <br/>
  <https://bartoszmilewski.com/2014/10/28/category-theory-for-programmers-the-preface/> <br/>
  **Note:** I have been told that Milewski's text may overfocus on examples relevant to functional programming and in particular examples that fit within the limitations of Haskell to the extent that it may be antididactical.
* Especially relevant for monads & side effects: a brief but very illuminating text by H. Kleisli about the Kleisli category: <br/>
  <http://www.ams.org/journals/proc/1965-016-03/S0002-9939-1965-0177024-4/S0002-9939-1965-0177024-4.pdf> <br/>
  You can understand monads in functional programming as follows: pure programs (without side effects) are arrows in the category `Type` of types and functions; effectful programs (with side effects) in monad `T : Type -> Type` are arrows in the Kleisli category of `T`. <br/>
  **Note:** This text deals with the Kleisli category for a *co*monad rather than a monad. Moreover, it is an older text, and it uses the term "standard construction" instead of comonad.
* A text about monads and universal algebra from a mathematical viewpoint, by Anthony Voutas: <br/>
  "The basic theory of monads and their connection to universal algebra" <br/> 
  <https://voutasaur.us/monad-algebra.pdf> <br/> 
  What's nice is that he takes his time to explain everything and does not require much prior knowledge. Section 1 is a formula-free introduction, sections 2 and 3 are certainly worth the while. Sections 4 and 5 are interesting but not especially relevant.

### Introduction to Simple Type Theory

* The book "Types and Programming Languages" (a.k.a. TAPL) by Benjamin C. Pierce, chapter 9 and prerequisites (see the dependency graph in the book's front matter). This book is also the lecture material of the [Formal Systems](https://onderwijsaanbod.kuleuven.be/syllabi/e/H04H8BE.htm) course.
  Aside of introducing simple type theory, this book focuses more on aspects of computation and decidability and less on matters of logic, soundness or categorical models. I expect that the master thesis is more likely focus on the latter.
  It seems pdfs are available online.

### Introduction to Haskell

(Not a necessity to learn Agda. Haskell is an incarnation of the kind of theoretical programming languages that is studied in the [Formal Systems](https://onderwijsaanbod.kuleuven.be/syllabi/e/H04H8BE.htm) course.)

* [Learn you a Haskell for Great Good, Miran Lipovača](http://learnyouahaskell.com/). Note: this tutorial parodies grammatical errors made by non-native English speakers.

### Introduction to Dependent Type Theory and Agda

- I still think chapter 1 (and appendix A.2) of the HoTT-book is one of the better ones: <https://homotopytypetheory.org/book/>
- I did my best to write good lecture notes for the Formal Systems course: <https://github.com/anuyts/teaching-tt>

Alternatives are:

- [Programming Language Foundations in Agda](https://plfa.github.io/)
- The book "Verified Functional Programming in Agda" by Aaron Stump
- Type Theory and Functional Programming by Simon Thompson: <https://www.cs.kent.ac.uk/people/staff/sjt/TTFP/>
- Agda exercise sessions from the Formal Systems course (not used every academic year): <https://github.com/anuyts/agda-sessions>
- The 1lab (see above).

### Introduction to Coq

(Coq is very powerful but also a bit harder to learn. We usually stick to Agda.)

* <https://github.com/coq/coq/wiki>
* <https://github.com/coq/coq/wiki/Other%20Coq%20Resources>

### Introduction to Lean
The Lean theorem prover is newer than both Coq and Agda and has a large community of people working on the formalization of mathematical results.

* <https://leanprover-community.github.io/learn.html>
* <https://leanprover-community.github.io/teaching/resources.html>

### Homotopy Type Theory (HoTT)

* The [HoTT-book](https://homotopytypetheory.org/) by the Univalent Foundations Program, especially chapters 1-2 and appendices A.1-3
* Related to h-levels (the degree of complexity of a type or topological space): HoTT book §3.1 - 3.3 and §7.1.

#### Cubical Type Theory and Cubical Agda

* [Official Agda documentation](https://agda.readthedocs.io/en/latest/language/cubical.html)
* Andrea Vezzosi, Anders Mörtberg, Andreas Abel (2021): [Cubical Agda: A Dependently Typed Programming Language with Univalence and Higher Inductive Types](https://staff.math.su.se/anders.mortberg/papers/cubicalagda2.pdf), JFP Vol 31
* The 1lab (see above)
* The [Agda Cubical library](https://github.com/agda/cubical)

* The original paper on cubical type theory:
  
  > Cyril Cohen, Thierry Coquand, Simon Huber, Anders Mörtberg (2015): [Cubical Type Theory: A Constructive Interpretation of the Univalence Axiom](https://doi.org/10.4230/LIPIcs.TYPES.2015.5), 21st International Conference on Types for Proofs and Programs (TYPES 2015)
  
  is a scientific breakthrough but not a good introduction to the subject.
  
* Video material

  * [HoTTEST Summer School lecture by Anders Mörtberg (2022)](https://www.youtube.com/watch?v=x4cz1OgpU3M)
  * [HoTTEST lecture by Andrea Vezzosi (2021)](https://www.youtube.com/watch?v=9RFt1Q2pHE8)
  * ["What are hcomp and hfill?" by Jim Fowler (2022)](https://www.youtube.com/watch?v=MVtlD22Y8SQ)

### Parametricity

* The book "Types and Programming Languages" (a.k.a. TAPL) by Benjamin C. Pierce, chapters 23 and 24 and prerequisites (see the dependency graph in the book's front matter). This book is also the lecture material of the Formal Systems course.
* An accessible paper about parametricity: [Wadler, 1989, Theorems for Free](https://people.mpi-sws.org/~dreyer/tor/papers/wadler.pdf)
* Reynolds's original paper about parametricity (less accessible): [Reynolds, 1983, Types, Abstraction and Parametric Polymorphism](http://www.cse.chalmers.se/edu/year/2010/course/DAT140_Types/Reynolds_typesabpara.pdf)

### Side effects and Monads

Haskell is a purely functional programming language, meaning that functions behave as in mathematics: they have an input and an output, and the output depends on the input, and that's it. They do not *do* anything.
Side effects (the technical term for doing something after all) are modelled in Haskell using the category theoretic concept of monads.
Relevant resources:

* A chapter in the aforementioned Haskell tutorial: <http://learnyouahaskell.com/a-fistful-of-monads>
* Kleisli's paper, mentioned above, is especially relevant.
* Voutas's paper, mentioned above, explains monads more categorically.

### Universal algebra, algebraic theories and its relevance to type theory

Group theory is the study of groups and is an instance of the formal concept of an "algebraic theory / Lawvere theory".

Simple/dependent type theory can be seen as the study of models of type theory and in this sense is an instance of the formal concept of a "multisorted/generalized algebraic theory".

Relevant resources:

* Gentle introduction to some prior concepts:
  Altenkirch, Ghani, Hancock, McBride, Morris, 2009, Indexed Containers
  <https://www.cambridge.org/core/services/aop-cambridge-core/content/view/FB9C7DC88A65E7529D39554379D9765F/S095679681500009Xa.pdf/indexed-containers.pdf>
* Voutas's paper, mentioned above.
* I also synthesized the most important ideas (including some more advanced ones) here, though with few examples: <https://anuyts.github.io/files/keml-diagrams.pdf>
* I tried to explain the relevance to type theory in chapter 3 of my [PhD thesis](https://anuyts.github.io/files/phd.pdf).
  (In both instances, my contribution is only to describe what exists.)
* Altenkirch, Kaposi, 2016: Type Theory in Type Theory using Quotient Inductive Types:
  <https://dl.acm.org/doi/abs/10.1145/2914770.2837638>
  (Inductive types are closely related to algebraic theories)

### Presheaf models of type theory

(To the extent that you're interested. Note: this subject has a tendency to turn your master thesis into a literature study.)
For the concept of a model, see the resources on algebraic theories. The idea is that if we have a model of a dependently typed system in which we know that there is no semantic (semantic means: in the model) counterpart of a proof of the false proposition, then our type system must be sound as the false proposition is then known to be unprovable.

The concept of presheaf models is inherently quite technical and takes time to sink in.

Relevant resources:

* [Martin Hofmann, 1997, Syntax and Semantics of dependent types](https://www.tcs.ifi.lmu.de/mitarbeiter/martin-hofmann/pdfs/syntaxandsemanticsof-dependenttypes.pdf), chapter 4
* In section 2.3 and chapter 4 of my [PhD thesis](https://anuyts.github.io/files/phd.pdf), I attempted to give an accessible introduction to presheaves and how presheaf categories constitute models of dependent type theory. Examples are provided. 

### Communication

* Writing readable texts
   * [Derek Dreyer at ICFP'21](https://www.youtube.com/watch?v=KfEVdMMY1aQ)
   * [Derek Dreyer at ICFP'16](https://www.youtube.com/watch?v=PM1Atui30qU)
   * [Benjamin Pierce, The Curse of Knowledge (slides)](https://cseweb.ucsd.edu/~npolikarpova/plmw/plmw2018-curse-of-knowledge.pdf)
   * [Jesper Cockx, Ten common writing issues in student papers](https://jesper.cx/posts/writing-issues.html)
   * [Stephen Heard, A road map for writing an Introduction](https://scientistseessquirrel.wordpress.com/2024/04/09/a-road-map-for-writing-an-introduction/)
* Giving comprehensible talks
   * [Derek Dreyer in 2019](https://www.youtube.com/watch?v=TCytsY8pdsc)
   * [Simon Peyton Jones](https://www.microsoft.com/en-us/research/academic-program/give-great-research-talk/)
   * Information on inclusivity w.r.t. [color blind](https://en.wikipedia.org/wiki/Color_blindness) people that I found helpful:
      * [The best charts for color blind viewers](https://www.datylon.com/blog/data-visualization-for-colorblind-readers)
      * [Color blindness simulator](https://www.color-blindness.com/coblis-color-blindness-simulator/)
* [All of Derek Dreyer's slides](https://people.mpi-sws.org/~dreyer/research.html)

#### Citing

Good frameworks to typeset your bibliography (assuming you're using LaTeX) are bibTeX and biber. Both use the same reference file format `.bib`.

From [DBLP](dblp.uni-trier.de) you can obtain excellent bibTeX (and other) citation records. Citation records obtained from Google Scholar are often sloppy and need to be manually adjusted where information is missing, wrong, or garbled.

In the 21st century, please make sure that every bibliography entry contains a clickable URL (unless a somewhat permanent-looking link affiliated to either the publisher or one of the authors or their institutions is hard to find).

### Community

If you are interested in ongoing research discussions or even job opportunities in the research communities related to our work, the following communication channels may be of interest:

Mailing lists:

* agda: <https://lists.chalmers.se/mailman/listinfo/agda>
* Dutch categories and types seminar: <https://dutchcats.github.io/>
* [EuroProofNet](https://europroofnet.github.io/): I think you need to apply via the EU COST system but they definitely intend to be very open. Ask around (e.g. ask me) if you get stuck.
* HoTT: see <https://homotopytypetheory.org/links/>
* HoTTEST electronic seminar series: <https://www.math.uwo.ca/faculty/kapulkin/seminars/hottest.html>
* types @ Chalmers: <https://lists.chalmers.se/mailman/listinfo/types>
* types @ UPenn: <http://lists.seas.upenn.edu/mailman/listinfo/types-list>
* types-announce: <http://lists.seas.upenn.edu/mailman/listinfo/types-announce>
* UCLouvain/ULB/VUB joint seminar series on category theory: <https://uclouvain.be/fr/instituts-recherche/irmp/seminaire-de-theorie-des-categories.html> <br/>
  It seems that you just need to mail them if you want to subscribe to their mailing list.
* 🕰️ EUtypes: <https://mailman.science.ru.nl/mailman/listinfo/eutypes> (I don't think this is active anymore.)

Zulip chats:

* <https://agda.zulipchat.com>
* <https://categorytheory.zulipchat.com>
* <https://c-t.zulipchat.com> (Categories & types)
* <https://dutchcats.zulipchat.com> (Dutch categories and types seminar)
* <https://epn.zulipchat.com> (EuroProofNet)
* <https://hott.zulipchat.com>
* <https://leanprover.zulipchat.com>
* <https://typ.zulipchat.com>

-----

[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC_BY--NC_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)
