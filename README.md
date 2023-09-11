This repository contains the files used for the CryptoVerif tutorial at the  Summer School on real-world crypto and privacy 2023.

CryptoVerif installations instructions can be found in [INSTALLATION.md](INSTALLATION.md), it is of course needed for this tutorial.

While this tutorial was designed as a live experience, some material can still be of use for people wishing to learn more about CryptoVerif. The slides may not always be standalone, but for people knowladgeable about crypto, it should still allow to discover CryptoVerif. Feedback is welcome.

The tutorial starts with [slides-morning.pdf](slides-morning.pdf), where a few files are used as demos: [live-demo-1.ocv](live-demo-1.ocv),  [live-demo-2.ocv](live-demo-2.ocv),  [live-demo-2.ocv](live-demo-2.ocv). This tutorial introduces basic cryptographic notions (indistinguishability, IND-CPA, SUF-CMA, proofs by reductions, the few basic syntaxix constructions of CryptoVerif and a first small proof in CryptoVerif of the equivalence of two IND-CPA variant.

After the morning tutorial, the first practical session sheet is [instructions-practical-session-1.pdf](instructions-practical-session-1.pdf), trying to prove the security of an ENC-then-MAC construction. To help with the basic syntax of CryptoVerif, a [cheatsheet.ocv](cheatsheet.ocv) is provided. Correction files are also available (see the files prefixed with `corr-enc-then-MAC)`, but only open them after really trying !).

In the afternoon, with [slides-afternoon.pdf](slides-afternoon.pdf), we delve into more complex constructs, with the goal of enabling students to do a proof of a signed diffie-helman protocol. It is then followed with the corresponding  [instructions-practical-session-2.pdf](instructions-practical-session-2.pdf), this time relying on the base template [template-signedDH.ocv](template-signedDH.ocv) (and once again with the correction, see `corr-signedDH.ocv`).

A wrap up with references additional material concludes this tutorial: [slides-afternoon-wrapup.pdf](slides-afternoon-wrapup.pdf).


