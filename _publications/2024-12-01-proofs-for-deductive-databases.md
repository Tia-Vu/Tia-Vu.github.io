---
title: "Proofs of Equality in Deductive Databases"
collection: publications
category: theses
permalink: /publication/2024-12-01-proofs-for-deductive-databases
excerpt: 'A proof system for extensions of Datalog with equality, giving methods for debugging and verifying the correctness of query results. Includes an elegant proof system for Egglog (an extension of Datalog with equality saturation), a proof checker mechanized in Rocq, and a case study optimizing NetKAT programs with Egglog.'
date: 2024-12-01
venue: 'M.S. Thesis, Cornell University'
paperurl: 'https://ecommons.cornell.edu/items/ecd3bf16-e18a-48de-80de-8c7e2d7ff2c1'
citation: 'Vu, Tia. (2024). &quot;Proofs of Equality in Deductive Databases.&quot; <i>M.S. Thesis, Cornell University</i>.'
---

Completed under the guidance of [Nate Foster](https://www.cs.cornell.edu/~jnfoster/) and
[Ryan Doenges](https://ryandoeng.es).

Datalog engines that support equality saturation can derive powerful conclusions, but
offer little insight into *why* a given fact holds. This thesis designs a proof system for
extensions of Datalog with equality, providing a foundation for debugging and verifying
the correctness of query results.

- Created an elegant and extensible proof system for the Egglog language, an extension of
  Datalog with equality saturation
- Programmed a verified proof checker for the proof system, mechanized in Rocq
- Applied the system in a case study optimizing NetKAT programs using Egglog

[Read the thesis on Cornell eCommons](https://ecommons.cornell.edu/items/ecd3bf16-e18a-48de-80de-8c7e2d7ff2c1)
