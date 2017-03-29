# PyMC3: Implement non-parametric Bayesian Methods #

## Abstract ##

Bayesian nonparametrics (BNP) is a major part of the cutting edge in machine learning today. Since Tom Ferguson's initial work on the  Dirichlet process in the 1970s, there have been tremendous extensions and forays into the field. Bayesian nonparametric models promise flexibility and scalability while maintaining strong theoretical guarantees. In particular, the Bayesian paradigm offers decision-theoretic guarantees on consistency, while the nonparametric approach liberates the modeler from assumptions that are rarely satisfied and difficult to test for, but near impossible to do inference without.

However, BNP models are not as popular as other supervised or unsupervised learning techniques for several reasons. Firstly, BNP models begin by placing probability distributions on spaces of probability distributions. The mathematical maturity required to read papers on Bayesian nonparametrics makes them inaccessible to many practitioners of data analysis, who would otherwise benefit from these techniques. Secondly, posterior inference, in many classes of BNP models is intractable, necessitating approximations, though this is less of a problem with frameworks like PyMC3 and Stan. Finally, there exist very few if any practical implementations of Bayesian nonparametric techniques.

In this GSoC project, I'd like to implement some of the more commonly used Bayesian nonparametric models in PyMC3. I'd also like to write extensive documentation and tutorials to help make PyMC3 and Bayesian nonparametric modelling more accessible to end users who may not have any experience with advanced machine learning.

## Technical Details ##

Over the course of the summer, I'd like to implement combinatorial BNP models in PyMC3, as well as improve on inference techniques for these models. I plan on implementing the Dirichlet process \[[Ferguson 1973](https://projecteuclid.org/euclid.aos/1176342360), [Sethuraman 1994](http://www3.stat.sinica.edu.tw/statistica/oldpdf/A4n216.pdf)\], the Dirichlet process mixture model \[[Antoniak 1974](https://projecteuclid.org/euclid.aos/1176342871)\], Polya trees \[[Müller 2013](https://projecteuclid.org/download/pdfview_1/euclid.cbms/1362163749)\] and the hierarchical Dirichlet process \[[Teh et al. 2006](https://www.stats.ox.ac.uk/~teh/research/npbayes/jasa2006.pdf)\].

[Edward](https://github.com/blei-lab/edward) \[[Tran el al. 2016](https://arxiv.org/abs/1610.09787)\] has recently added Dirichlet processes and I hope to use their implementation as a reference.

## Schedule of Deliverables

### May 1th - May 28th, **Community Bonding Period**

Spend time familiarizing myself with the PyMC3 codebase, and start with API design for the underlying combinatorial stochastic processes. Also, review existing literature to familiarize myself with any identified issues with implementing Bayesian nonparametric models.

### May 29th - June 2nd
Implement the Dirichlet process.

### June 5th - June 9th 
Debug the Dirichlet process implementation, along with adding tests and documentation.

### June 12th - June 16th
Implement Dirichlet process mixture models for clustering.

### June 19th - June 23th, **End of Phase 1**
Buffer time for anything that's overrun, along with debugging and documenting Dirichlet process mixture models. Commit everything thus far and submit a pull request.

### June 26 - June 30th, **Begin of Phase 2**
Begin implementing Polya trees for density estimation.

### July 3rd - July 7th
Polya trees are difficult to implement, so this week is meant for debugging.

### July 10th - July 14th
Write up documentation and tests for Polya trees. Commit everything thus far and submit a pull request.

### July 17th - July 21th, **End of Phase 2**
I'm leaving this week as a buffer for any overruns, as well as clearing up any issues with the PR.

### July 24th - July 28th, **Begin of Phase 3**
Begin implementing hierarchical Dirichlet processes for clustering and grouping data.

### July 31st - August 4th
Debug the hierarchical Dirichlet process implementation. Add tests and documentation.

### August 7th - August 11th
At this point, I'd like to start working on a tutorial on BNP models in PyMC3 accessible to someone with just a first course in machine learning or statistics.

### August 14th - August 18th
Complete writing the tutorial. Submit a pull request for hierarchical Dirichlet processes.

### August 21st - August 25th, **Final Week**
Fix any issues with the pull request.

### August 28th - August 29th, **Submit final work**
Celebrate!

## Future work and extensions
Bayesian nonparametrics is advancing at an extraordinary pace. A straightforward extension to the work I've proposed would be to add other prior processes: Pitman-Yor, hierarchical beta, and other stickbreaking prior processes. I plan to write the code in a modular way so that the prior distributions are decoupled from the clustering and density estimation models. This would make implementing other priors for the same models, and other models for the same priors as straightforward as possible. I plan on continuing working on BNP models in PyMC3 after GSoC as a regular contributor.

## Development Experience
While I'm comfortable coding in Python and Haskell, this is my first formal programming project. I've used both Haskell and Python for data analysis, either for college projects or at think tanks and NGOs during internships.

## Other experience
I graduated with a bachelor's in economics and mathematics from St. Stephen's College, Delhi in 2016. I am currently working for a year with a group of academics aiming to improve policy implementation in India through a data driven approach, before I begin my graduate studies in statistics this fall at the University of Minnesota, where I aim to study the posterior consistency of variational inference in Bayesian nonparametric models. I have always believed that statistical literacy is an important part of general literacy, and in the larger scope of my work I hope to make Bayesian statistics more accessible to the general public through teaching as well as through FOSS like PyMC3.

## Why this project?
As a statistics graduate student, I plan on working on theoretical guarantees for Bayesian nonparametric models. Implementing these models for PyMC3 is a great way to get open source software development experience, while bettering my grasp on the literature. Equally importantly, I'm very interested in helping people learn and understand statistics, therefore writing tutorials for lay audiences will help improve my communication skills before grad school.
