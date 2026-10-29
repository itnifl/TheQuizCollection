# TDT4136 Introduction to Artificial Intelligence

[← All courses](../readme.md)

> **Link types:** 📝 starts a quiz · 📖 opens reading material (lecture notes, course pages, external sites)

[![Artificial Intelligence](https://img.shields.io/badge/Artificial%20Intelligence-5C2D91?style=for-the-badge&logoColor=white)](https://www.ntnu.edu/studies/courses/TDT4136)
[![Search Algorithms](https://img.shields.io/badge/Search%20Algorithms-007ACC?style=for-the-badge&logoColor=white)](https://en.wikipedia.org/wiki/Search_algorithm)
[![A* Search](https://img.shields.io/badge/A*%20Search-2E7D32?style=for-the-badge&logoColor=white)](https://en.wikipedia.org/wiki/A*_search_algorithm)
[![Admissible Heuristic](https://img.shields.io/badge/Admissible%20Heuristic-37474F?style=for-the-badge&logoColor=white)](https://en.wikipedia.org/wiki/Admissible_heuristic)

## Quizzes

### Assignment quizzes

- 📝 [Assignment 1 Learning – Part 1](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136assignment1learningpart1) – setup and uninformed search (BFS, DFS, UCS)
- 📝 [Assignment 1 Learning – Part 2](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136assignment1learningpart2) – informed search (Greedy Best-First, A*)
- 📝 [Assignment 1 Learning – Part 3](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136assignment1learningpart3) – A*, admissibility and consistency
- 📝 [Assignment 2 Learning – Part 1](https://dev-quizmachine.itautomasjon.no/p/tdt4136assignment2learning) – constraint satisfaction problems
- 📝 [Assignment 2 Learning – Part 2](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136assignment2learningpart2)
- 📝 [Assignment 2 Learning – Part 3](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136assignment2learningpart3)
- 📝 [Assignment 2 Core Concepts](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136assignment2coreconcepts)
- 📝 [Assignment 3 Learning – Part 1](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136assignment3learningpart1)
- 📝 [Assignment 3 Core Concepts](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136assignment3coreconcepts)
- 📝 [Assignment 4 Learning – Part 1](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136assignment4learningpart1)
- 📝 [Assignment 4 Learning – Part 2](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136assignment4learningpart2)

### Lecture quizzes

- 📝 [Lecture 5 (Chapter 7) – Logical Agents](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136lecture5chapter7)
- 📝 [Lecture 6 (Chapter 8) – First-Order Logic](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136lecture6chapter8)
- 📝 [Lecture 7 (Chapter 9) – Inference in First-Order Logic](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136lecture7chapter9)
- 📝 [Lecture 8 (Chapter 6) – Adversarial Search and Games](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136lecture8chapter6)
- 📝 [Lecture 9 (Chapter 24) – Introduction](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136lecture9chapter24introduction)
- 📝 [Lecture 9 (Chapter 24)](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136lecture9chapter24)
- 📝 [Lecture 10 (Chapter 17) – Introduction](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136lecture10chapter17introduction)
- 📝 [Lecture 10 (Chapter 17)](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136lecture10chapter17)
- 📝 [Lecture 11 (Chapter 11) – Introduction](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136lecture11chapter11introduction)
- 📝 [Lecture 11 (Chapter 11)](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136lecture11chapter11)
- 📝 [Lecture 12 (Chapters 10 and 28) – Introduction](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136lecture12chapter10and28introduction)
- 📝 [Lecture 12 (Chapters 10 and 28)](https://dev-quizmachine.itautomasjon.no/Quiz/Take/tdt4136lecture12chapter10and28)

## About Assignment 1 – Search algorithms

A hand-computation exercise set on the search algorithms from the lectures. The problem is a "speedrunning route" through an abstract map of Doom's *E1M8: Phobos Anomaly* (states A–I, start A, goal F): every edge costs 1, obstacles add cost (stairs +1, lift +2), and each state carries a heuristic value h(n) (h(A) = 25, h(I) = 22, h(F) = 0). There are eight tasks across three parts; successors are generated in alphabetical order and ties are broken alphabetically. Pseudocode references are to *Artificial Intelligence: A Modern Approach* – Breadth-First-Search (Fig. 3.9, p. 95) and Best-First-Search (Fig. 3.7, p. 91).

**Learning outcomes:**
- Trace BFS, DFS, UCS, Greedy Best-First and A* by hand and produce the expansion order, path and path cost
- Compare informed and uninformed strategies on the same graph
- Explain why A* can miss the optimal solution when the heuristic is not consistent
- State and prove or disprove admissibility and consistency for a given heuristic
- Relate the choice of frontier data structure and tie-breaking to search behaviour

## Resources

- 📖 [NTNU TDT4136 – Introduction to Artificial Intelligence (official course page)](https://www.ntnu.edu/studies/courses/TDT4136)
- 📖 [AIMA – Russell & Norvig, *Artificial Intelligence: A Modern Approach*](https://aima.cs.berkeley.edu/)
- 📖 [aimacode – reference implementations (GitHub)](https://github.com/aimacode)
- 📖 [PathFinding.js – interactive search and pathfinding visualiser](https://qiao.github.io/PathFinding.js/visual/)
