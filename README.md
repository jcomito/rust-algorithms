# Contest Algorithms in Rust

[![Build Status](https://travis-ci.org/EbTech/rust-algorithms.svg?branch=master)](https://travis-ci.org/EbTech/rust-algorithms)
[![Latest Version](https://img.shields.io/crates/v/contest-algorithms.svg)](https://crates.io/crates/contest-algorithms)

A collection of classic data structures and algorithms, emphasizing usability, beauty and clarity over full generality. As such, this should be viewed not as a blackbox *library*, but as a whitebox *cookbook* demonstrating the design and implementation of algorithms. I hope it will be useful to students and educators, as well as fans of algorithmic programming contests.

This repository is distributed under the [MIT License](LICENSE). The license text need not be included in contest submissions, though I would appreciate linking back to this repo for others to find. Enjoy!

## For Students and Educators

When learning a new algorithm or data structure, it's often helpful to see or play with a concrete implementation. As such, this repository catalogues several classic algorithms in their simplest forms.

In addition, the Rust language has outstanding pedagogical attributes. Its compiler acts as a teacher, enforcing strict discipline while pointing to clearer ways to structure one's logic.

## For Programming Contests

The original intent of this project was to build a reference for use in programming contests ranging from [Codeforces](https://codeforces.com) to [Google's Kick Start and Code Jam](https://codingcompetitions.withgoogle.com), [LeetCode](https://leetcode.com/contest) and [HackerRank](https://www.hackerrank.com/contests). As a result, it contains algorithms that are frequently useful to have in one's toolkit, with an emphasis on code that is concise and easy to modify under time pressure.

Most competitive programmers rely on C++ for its fast execution time. However, it's notoriously unsafe, diverting a considerable share of the contestant's time and attention on mistake prevention and debugging. Java is the next most popular choice, offering a little safety at some expense to speed of coding and execution.

To my delight, I found that Rust eliminates entire classes of bugs, while reducing visual clutter to make the rest easier to spot. And, it's *fast*. There's a learning curve, to be sure. However, a proficient Rust programmer stands to gain a competitive advantage as well as a more pleasant experience!

For help in getting started, you may check out [some of my past submissions](https://codeforces.com/contest/1168/submission/55200038).

Other online judges that support Rust:
- [Kattis](https://open.kattis.com/help/rust)
- [Timus](http://acm.timus.ru/help.aspx?topic=rust)
- [SPOJ](https://www.spoj.com/)

## Programming Language Advocacy

My other goal is to appeal to developers who feel limited by mainstream, arguably outdated, programming languages. Perhaps we have a better option.

Rather than try to persuade you with words, this repository aims to show by example. If you're new to Rust, see [Jim Blandy's *Why Rust?*](http://www.oreilly.com/programming/free/files/why-rust.pdf) for a brief introduction, or just [dive in!](https://doc.rust-lang.org/book/)

## Contents

- [Basic graph representations](src/graph/mod.rs): adjacency lists, minimum spanning tree, Euler path, disjoint set union 
- [Network flows](src/graph/flow.rs): Dinic's blocking flow, Hopcroft-Karp bipartite matching, min cost max flow
- [Connected components](src/graph/connectivity.rs): 2-edge-, 2-vertex- and strongly connected components, bridges, articulation points, topological sort, 2-SAT
- [Associative range query](src/arq_tree.rs): known colloquially as *segtrees*
- [GCD Math](src/math/mod.rs): canonical solution to Bezout's identity
- [Arithmetic](src/math/num.rs): rational and complex numbers, linear algebra, safe modular arithmetic
- [FFT](src/math/fft.rs): fast Fourier transform, number theoretic transform, convolution
- [Scanner](src/scanner.rs): utility for reading input data ergonomically
- [String processing](src/string_proc.rs): Knuth-Morris-Pratt string matching, suffix arrays, Manacher's palindrome search
