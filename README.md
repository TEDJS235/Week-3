# Week 3: Concurrency in Programming Languages

**Author**: James Shan  
**Course**: Programming Languages (CPSC-354)  
**Date**: September 15, 2024  

---

## Table of Contents
1. [Introduction](#introduction)
2. [Summary](#summary)
3. [Research Question](#research-question)
4. [Exploration with LLM](#exploration-with-llm)
5. [Key Findings](#key-findings)
6. [Historical Developments](#historical-developments)
7. [Advantages and Disadvantages](#advantages-and-disadvantages)
8. [Discord Summary](#discord-summary)
9. [References](#references)

---

## Introduction

In Week 3, I explored how **functional** and **imperative** programming paradigms address concurrency. This week emphasized the advantages, challenges, and historical context of concurrent programming, essential for building modern scalable systems.

---

## Summary

In **Week 3**, the focus was on exploring concurrency in functional and imperative programming languages, highlighting their unique approaches and trade-offs. Concurrency, essential in modern systems, allows multiple tasks to run simultaneously, requiring careful design to avoid pitfalls like race conditions and deadlocks.

Imperative programming (e.g., **C**, **Java**) uses **threads**, **locks**, and **shared memory** to manage concurrency. While this approach provides high performance and flexibility, it is prone to issues like thread interference and deadlocks, which complicate debugging and testing.

Functional programming, on the other hand, leverages **immutability**, **pure functions**, and higher-level abstractions like **message passing** (e.g., Actor Model) and **software transactional memory (STM)**. Languages like **Haskell** and **Erlang** simplify concurrency by avoiding mutable shared state, reducing errors while promoting scalability.

Historical milestones such as the **Actor Model (Carl Hewitt, 1973)** laid the foundation for message-passing systems, while frameworks like **Akka** in Scala and lightweight concurrency primitives like **Go’s Goroutines** further advanced concurrent programming. These developments provide efficient, reliable tools to build scalable systems.

This week’s exploration reinforced the importance of choosing the appropriate concurrency model for a given problem. While functional programming reduces complexity, imperative approaches offer performance benefits at the cost of increased management overhead.

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

In **Week 3**, I explored the topic of concurrency in programming languages, focusing on the contrast between functional and imperative approaches. Functional programming manages concurrency by emphasizing **immutability**, **pure functions**, and abstractions like **message passing** (e.g., the Actor Model) and **software transactional memory (STM)**. These features avoid shared mutable state, reducing common issues like race conditions and deadlocks. Languages like **Erlang** and **Haskell** exemplify this paradigm, providing tools that make concurrent programming safer, more predictable, and scalable.  

Imperative programming, on the other hand, relies on low-level constructs such as **threads**, **locks**, and shared memory to manage concurrency. While these approaches are powerful and offer high performance, they come with trade-offs, such as the risk of **thread interference**, **deadlocks**, and greater debugging complexity. Developers must manually handle synchronization, which increases overhead and potential for errors.  

Historically, the **Actor Model (1973)** by Carl Hewitt laid the foundation for functional concurrency models by introducing message passing. Later advancements like **Go’s Goroutines** and **Scala’s Akka Framework** built on these ideas to offer scalable and lightweight concurrency primitives. Goroutines, in particular, enable massive parallelism with minimal memory overhead, making them ideal for cloud-scale applications.  

This week, I reflected on the trade-offs between lightweight threads (e.g., Goroutines) and traditional heavyweight threads. Lightweight threads allow for efficient concurrency scheduling, but may introduce challenges when interfacing with shared state or blocking calls. Comparing the two models highlights the balance between performance, scalability, and ease of programming.

---

## References  

1. Actor Model: Carl Hewitt (1973).  
2. Go Documentation: [https://golang.org](https://golang.org).  
3. Akka Framework: [https://akka.io](https://akka.io).  
4. Programming Languages: Lecture Notes and HackMD Guide.  

---

## GitHub Repository

[https://github.com/TEDJS235/Week-3](https://github.com/TEDJS235/Week-3)
