# Classroom Seating Arrangement Problem
## Computational Complexity Analysis

---

## 1. Problem Overview

The classroom seating arrangement problem involves placing students in a single row of seats before an examination while following two rules:

1. Friends should not sit next to each other.
2. Students from the same city should not sit next to each other.

Each student must be seated exactly once.  
The objective is to determine whether a valid seating arrangement exists that satisfies both constraints.

This problem can be modeled as a **Constraint Satisfaction Problem (CSP)**.

---

## 2. Understanding P vs NP in Context

### 2.1 What is a P Problem?

A P (Polynomial-time) problem is one that can be solved efficiently.  
The time required grows at a manageable rate as input size increases.

### 2.2 What is an NP Problem?

An NP (Nondeterministic Polynomial-time) problem is one where:
- A proposed solution can be verified quickly.
- Finding the solution may require checking many possibilities.

### 2.3 Applying to the Seating Problem

Checking a seating arrangement is easy.  
We only need to scan adjacent students once.  
Time complexity: **O(n)**

Finding a valid arrangement is difficult.  
There are **n! possible permutations** of students.

Because verification is easy but finding a solution is computationally expensive, this problem behaves like an **NP-type problem**.

---

## 3. Brute Force Approach

### 3.1 Method

The brute force method tries all possible seating arrangements.

Steps:
1. Generate all permutations of students.
2. For each permutation:
   - Check adjacency rules.
3. Stop when a valid arrangement is found.

### 3.2 Time Complexity

Number of arrangements = **n!**

Time complexity: **O(n!)**

Factorial growth increases extremely fast:
- 5 students → 120 arrangements
- 10 students → 3,628,800 arrangements
- 15 students → over 1 trillion arrangements

### 3.3 Advantages

- Guaranteed to find a solution if one exists.
- Simple to implement.

### 3.4 Limitations

- Not scalable.
- Computationally infeasible for large classes.

---

## 4. Heuristic (Smart) Approach

Instead of checking all permutations, a heuristic strategy reduces the search space.

### 4.1 Example Heuristics

- Seat students with the most friends first.
- Separate large city groups early.
- Place highly restricted students before flexible ones.

### 4.2 Why It Is Faster

- Reduces unnecessary permutations.
- Avoids exploring clearly invalid paths.
- Makes smarter placement decisions early.

### 4.3 Limitations

- May not always find a valid arrangement.
- Does not guarantee optimality.
- Depends on strategy quality.

Time complexity: Much lower than O(n!), but not guaranteed polynomial.

## 6. Conclusion
### Conclusion for Task 2

The classroom seating arrangement problem illustrates the differences between brute force and heuristic approaches. Brute force guarantees a correct solution but becomes impractical as the number of students increases due to factorial growth. Heuristic strategies, such as seating students with many friends first or separating students from the same city early, provide faster, practical solutions. While heuristics may not always yield the perfect arrangement, they efficiently satisfy most rules, making them suitable for real classroom scenarios.
