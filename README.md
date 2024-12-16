# Week 3: Concurrency in Programming Languages

**Author**: James Shan  
**Course**: Programming Languages (CPSC-354)  
**Date**: December 15, 2024  

---

## Table of Contents
1. [Introduction](#introduction)
2. [Research Question](#research-question)
3. [Exploration with LLM](#exploration-with-llm)
4. [Key Findings](#key-findings)
5. [Historical Developments](#historical-developments)
6. [Advantages and Disadvantages](#advantages-and-disadvantages)
7. [Discord Summary](#discord-summary)
8. [References](#references)

---

## Introduction

In Week 3, I explored how **functional** and **imperative** programming paradigms address concurrency. This week emphasized the advantages, challenges, and historical context of concurrent programming, essential for building modern scalable systems.

---

## Research Question

> **How do functional and imperative programming languages address concurrency, and what significant historical developments influenced their evolution?**

---

## Exploration with LLM

### Functional vs Imperative Approaches to Concurrency

- **Functional Programming**:
  - Avoids shared mutable state by emphasizing **immutability**.
  - Uses high-level abstractions such as **message passing** and **STM**.
  - Examples: Erlang’s Actor Model, Haskell's STM.

- **Imperative Programming**:
  - Relies on **threads**, **locks**, and shared memory.
  - Provides performance benefits but introduces challenges like race conditions.

---

## Key Findings

1. Functional programming simplifies concurrency but may introduce performance overhead.
2. Imperative programming offers fine-grained control at the cost of complexity and debugging overhead.

---

## Historical Developments

- **Actor Model** (1973): Carl Hewitt introduced message-passing systems.
- **Java Threads**: Introduced primitive concurrency mechanisms in the 1990s.
- **Go’s Goroutines**: Lightweight concurrency primitives improve scalability.
- **Akka Framework**: Scala-based Actor Model framework for distributed systems.

---

## Advantages and Disadvantages

| **Approach**        | **Advantages**                                 | **Disadvantages**                            |
|----------------------|-----------------------------------------------|---------------------------------------------|
| Functional           | Simpler concurrency, fewer bugs.             | Performance overhead, requires paradigm shift. |
| Imperative           | High performance, low-level control.         | Error-prone, debugging complexity.          |

---

## Discord Summary  

In **Week 3**, I explored concurrency in functional and imperative programming languages. Functional programming emphasizes **immutability** and high-level abstractions like **message passing**, making concurrency safer and less error-prone. Imperative programming uses **threads** and **locks**, which offer performance but require careful handling to avoid race conditions and deadlocks. Historical developments such as the **Actor Model (1973)**, **Java threads (1990s)**, and **Go’s Goroutines** have shaped modern concurrent programming.

**Interesting Question**:  
What are the major trade-offs between lightweight threads (e.g., Go's Goroutines) and heavy threads in traditional imperative languages?

---

## References  

1. Actor Model: Carl Hewitt (1973).  
2. Go Documentation: [https://golang.org](https://golang.org).  
3. Akka Framework: [https://akka.io](https://akka.io).  
4. Programming Languages: Lecture Notes and HackMD Guide.  

---

## GitHub Repository

[https://github.com/TEDJS235/Week-3](https://github.com/TEDJS235/Week-3)
