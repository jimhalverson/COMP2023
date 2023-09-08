# Computational Physics

PHYS 7321, Fall 2023

Instructor: Jim Halverson

E-mail: j.halverson@northeastern.edu

Phone: 617-373-2957

Office Hours: Dana 226, TF 11:30-12:30, see below.

TA & Grader: Sneh Pandya, ``pandya.sne@northeastern.edu``

# Course Information

**Course Schedule:** Lectures TF 9:50-11:30.

**Course Location:** EXP 201! (Excitement, not factorial).

**Office Hours:** I will hold office hours in Dana 226, TF 11:30-12:30. Due to the dynamic nature of the material and schedules, I will also answer questions on Slack for one hour per week. To take advantage of this, post a question in ``#ask-jim`` and I will respond in the order the are asked. These should be higher level questions regarding the science and algorithms in the class and in your homework. For "my code won't run" level questions, ask your classmates for help in ``#debugging``, and if you're really stuck, in ``#ask-sneh``. 

**Lectures:** I'll type code and we will debug in real time. Pedagogically, I think this makes sense. Let's talk about it.

**Description:** Here's the official course description listed by the registrar's office.

> Covers basic numerical methods for differentiation, integration, and matrix operations used in linear algebra problems, discrete Fourier transforms, and standard and stochastic ordinary and partial differential equations. Specific applications of these methods may include classical chaos, computation of eigenstates of simple quantum systems, classical phase transitions, boundary value problems, pattern formation, and molecular dynamics and classical/quantum Monte Carlo methods to simulate the equilibrium and nonequilibrium properties of condensed phases.

To be sure, this is important material and I will teach you a good deal of it. 

However, missing from this written-years-ago description is any nod toward computer science's ongoing revolution in machine learning (ML) and artificial intelligence (AI). This interface is of increasing importance to an increasing number of Ph.D. students in Physics. As your professor, it would be remiss of me if I didn't teach you the basics. Therefore, the entire course will be in Python and we will also cover:

- Introduction to Python.
- Supervised Learning.
- Reinforcement Learning.
- Genetic Algorithms.
- Generative Models.
- ML Theory: NNGP and NTK.

This list covers a broad swath of the recent progress in ML, and in each case we will focus not only on the basics of the techniques, but also applications within Physics. 

**Course Goals:** Every subfield in physics develops niche techniques crucial to its success. However, most also rely crucially on broad computational techniques that are applicable to many subfields. Our goals in this course address the latter, and are:
- Proficiency in Python.
- Proficiency in the basics of ML.
- Assessing problems with respect to the potential use of computational techniques.
- Ability to rapidly develop and implement computational techniques to solve problems.

For most of you, maximizing your strengths in these areas will be extremely useful to your Ph.D. research. These skills also have much broader application, e.g. in many different types of industry, where you may one day work.


**Resources:** Given the constantly evolving nature of the subject, my lectures will rely on a number of different resources, including some written by friends. Two excellent resources for the intersection of physics and ML are:
- [IAIFI](http://www.iaifi.org), officially the NSF AI Institute for Artificial Intelligence and Fundamental Interactions, an interdisciplinary institute with a focus on the intersection of AI and physics in collaboration between Northeastern, MIT, Harvard, and Tufts.
- [Physics $\cap$ ML](http://www.physicsmeetsml.org), pronounced "Physics Meets ML," a virtual seminar series organized by myself and some friends that builds on a meeting we ran at Microsoft Research in 2019.

A simple perusal of the website will give you a sense of what's out there. Details can be found in links to slides and videos. More broadly, some canonical ML references are:
- [Deep Learning](https://www.deeplearningbook.org), by Ian Goodfellow, Yoshua Bengio, and Aaron Courville.
- [Geometric Deep Learning](https://geometricdeeplearning.com), by Michael Bronstein, Joan Bruna, Taco Cohen, and Petar Veličković.
- [Reinforcement Learning](http://incompleteideas.net/book/the-book-2nd.html), by Richard Sutton and Andrew Barto.

Of course, I am also heavily influenced by and indebted to my collaborators on related topics. Some of our recent works include
- [NN-FT](https://arxiv.org/abs/2307.03223). Neural network field theories are a new approach to field theory inspired by ML theory. The above link presents the most modern and thorough treatment, see also [here](https://arxiv.org/abs/2008.08601) for our original work and [here](https://arxiv.org/abs/2112.04527) for a brief article that developed a number of new concepts, including when an NN-FT is a *quantum* field theory.
- [Searching for Ribbons with Machine Learning](https://arxiv.org/abs/2304.09304) uses ML to build a state of the art algorithm for verifying ribbonness of a knot. Together with slice obstructions, this may be used to study the Smooth Poincaré Conjecture in four dimensions (SPC4), a major open problem in topology. Using it, we ruled out over 800 potential counterexamples to SPC4. See also the fantastic [Man and Machine](https://arxiv.org/abs/0906.5177) article about SPC4.
- [Machine Learning in the String Landscape](https://arxiv.org/abs/1707.00655) one of the original papers on ML for String Theory. One aspect that has stood the test of time is the introduction of conjecture generation, a technique for making ML rigorous.

I may post a few more here as I finish two exciting works in early Fall 2023.

Finally, it's 2023 and this is a course on computational physics. Therefore, unless for some unforeseen reason it becomes a problem, large language models (LLMs) may be used as coding assistants. My only rule is that you use *free* tools, fairness reasons, such as [ChatGPT](http://chat.openai.com) or [GitHub Copilot](https://github.com/features/copilot). The latter is free with a student account; to learn about that, post in ``#ask-sneh``. While this might be controversial to some, a goal of this course is to teach you to be a *productive* computational scientist, and that means using the best tools available. Crucially from an educational perspective, though these are useful, LLMs can produce code that is either wrong or doesn't run, so you still have to know what you're doing. You might find if you're just learning that you shouldn't use LLMs for awhile, test it out and see what works.

**Homework:** We'll have homeworks, probably biweekly. I hope they're challenging and educational, but especially fun.

**Project:** There will also be a final project, done in coordination with a Northeastern faculty member. This is an excellent opportunity to learn about a new field, and to make a good impression on a potential Ph.D. advisor. The goal of the project is to implement a non-trivial algorithm in service of a physics problem, and obtain some non-trivial resuls. At the beginning of the semester you will 1) choose a faculty member to work with, 2) develop a plan with them, and 3) present the plan in a slide template, as one of the early homework assignments, which must be approved. 

**Late homework policy:** No late homeworks will be accepted. Instead, you will be allowed to drop your lowest homework grade.

**Academic Integrity:** Be sure to review Northeastern Academic Integrity policies, which are [here](http://www.northeastern.edu/osccr/academic-integrity-policy/).

**Grading:** Homework 70%, Project 30%. 

# Course Material

Topics are organized by order of presentation, not by strict adherence to the category. 

- ***Part 1: Python Essentials.*** 
    - Conda environments and pip.
    - Jupyter notebooks and Google Colab
    - Conditionals and Loops
    - Data Structures
    - Scientific computing libraries
    - Parallel processing
    - Large language models as coding assistants.

- ***Part 2: Computational Physics.*** This is a beautiful subject with a history spanning decades. Some of the topics we may include are:
    - Mechanics applications of Numerical Differentiation
    - Wave Equations
    - Heat Flow
    - Electrostatics 
    - Schrodinger Equation
    - Introduction to Probability, Statistics, and Bayesian Inference
    - Monte Carlo and the Ising Model

- ***Part 3: Physics $\cap$ ML.*** Machine learning is an enormous field, and applications within phyiscs are vast. Some of the topics we may include are:
    - Optimization: Gradient Descent and Genetic Algorithms
    - Neural networks
    - Supervised learning
    - Reinforcement Learning
    - Generative Models
    - ML Theory: NNGP and NTK.

# Comments and Recommendations

- **Level Up:** Colleagues who have taught the course in previous years have noted that some students have much more programming experience than others. Since a major course goal is to get *everyone* proficient in Python, more advanced students may sometimes feel that the lectures or homeworks are too simple. In such cases, I would remind you that our overall goal is to learn to produce *useful scientific code*, which requires (in order of importance):
    1. **Correctness.** If it's not correct, it's not useful.
    2. **Efficiency.** Even if it's correct, it might be so slow that it's not useful. Or, making it faster might make it *more* useful, opening up new scientific possibilities. Making a code more efficient often requires careful thought with respect to algorithm choice / development, especially as it regards computational complexity.
    3. **Beauty.** In addition to correctness and efficiency, beauty / readability also matters. 
    
    
    Our lectures and homeworks will generally focus on correctness. If you're looking for more of a challenge, I strongly encourage you to "level up" by making your code more efficient and readable. If you go above and beyond, Sneh and I will take it into account as potential extra credit. It'll also just make you a stronger computational physicist.

- During lecture, please ask questions! An interactive classroom will be beneficial to all.

- We will cover a lot of material, and it is important to not get behind. Since homework assignments are biweekly, there will be ample time to ask general questions in office hours that may or may not be related to the homework.

- **Undergraduates:** Ph.D. level courses differ from undergraduate courses in some important ways, especially with respect to grading. Please ask me about them in office hours if you have questions.

