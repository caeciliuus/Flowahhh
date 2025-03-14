---
tags:
  - lecture
  - videonotes
  - S1
  - chenflix
  - ma162
Type: Video Notes
Date: 2024-09-26
Class: "[[MA 16200]]"
---
[[Calculus - Early Transcendentals, Third Edition.pdf#page=665&offset=,,|Calculus - Early Transcendentals, Third Edition, 10.1. An Overview]]
- A sequence is a list of numbers in a particular order
	- For example, $\{1,2,3,4,5,\dots\}$ is called an infinite series
- Can also write sequences using an explicit formula
	- $\{1,2,3,4,5,\dots\}=\{a_{n}\}^\infty _{n=1}$
- Sometimes we use recurrence relation
	- $\{1,2,3,4,5,\dots\}$ where $a_{1}=1$ and $a_{n+1}=a_{n}+1$ -> $a_{2}=a_{1}+1$
	- $\{2,4,6,8,\dots\},a_{1}=2,a_{n}=a_{n}+2$
- A sequence is said to converge if $\lim_{ n \to \infty }a_{n}$ exists
	- If $\lim_{ n \to \infty }a_{n}$ DNE, then the sequence diverges

>[!exm] $a_{n}=\frac{(-1)^n n}{2n^2+1},\text{ n = 1, 2, 3}$
>![[Pasted image 20240926193208.png|center|400]]
>$$a_{1}=-\frac{1}{3},a_{2}=-\frac{13}{19},a_{3}=\frac{4}{33},\dots$$
>$$\lim_{ n \to \infty } a_{n}=\lim_{ n \to \infty } (-1)^n\cdot \lim_{ n \to \infty } \frac{n}{2n^2+1}=0$$
>$$\text{Where }(-1)^n\text{ has no effect on magnitude. Since the limit exists, this sequence converges}$$

- A series is the sum of the terms in a sequence
	- $\{1,2,3,4,5\}$ is a sequence, $1+2+3+4+5$ is a series
	- Like with sequences, we can express series compactly: $1+2+3+4+5+\dots=\sum ^\infty _{n=1}n$, called infinite series because no end to the summation. Can also have finite series
- The sum of the first $n$ terms is called the $n$th partial sum, written as $S_{n}$
- If the partial sum appears to approach some finite number, we say the series converges

>[!exm] $\sum^\infty _{n=1} \frac{1}{2n}$
>$$=\frac{1}{2}+\frac{1}{4}+\frac{1}{8}+\frac{1}{16}+\dots$$
>$$S_{1}=\frac{1}{2},S_{2}=\frac{1}{4}+\frac{1}{2},S_{3}=\frac{1}{2}+\frac{1}{4}+\frac{1}{8},S_{4}=\frac{1}{2}+\frac{1}{4}+\frac{1}{8}+\frac{1}{16}\dots S_{10}=\frac{1023}{1024}$$
>$$\lim_{ n \to \infty } S_{n}=1$$

