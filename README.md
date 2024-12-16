# Week 3: Concurrency in Programming Languages

**Author**: James Shan  
**Course**: Programming Languages (CPSC-354)  
**Date**: September 15, 2024  

---

## Table of Contents
1. [Introduction](#introduction)
2. [Summary](#summary)
3. [Research Question](#research-question)
4. [Interaction with LLM](#interaction-with-llm)
5. [Key Findings](#key-findings)
6. [Historical Developments](#historical-developments)
7. [Advantages and Disadvantages](#advantages-and-disadvantages)
8. [Discord Summary](#discord-summary)
9. [References](#references)

---

## Introduction

Concurrency is a cornerstone of modern software development, enabling systems to perform multiple tasks simultaneously. This week’s exploration delves into how **functional** and **imperative** programming languages address concurrency, emphasizing their unique approaches, historical context, and trade-offs.

This report aims to provide an engaging and structured analysis of concurrency paradigms, supported by historical milestones and academic references. It also links to the Week 3 [literature review](https://github.com/TEDJS235/Week-3/literature-review), further expanding on the topic.

---

## Summary

Functional programming languages like **Erlang** and **Haskell** simplify concurrency by leveraging **immutability**, **pure functions**, and high-level abstractions such as **message passing** and **software transactional memory (STM)**. These tools avoid mutable shared state, significantly reducing bugs like race conditions and deadlocks.

In contrast, imperative programming languages such as **C** and **Java** rely on low-level constructs like **threads**, **locks**, and **shared memory** to manage concurrency. While these methods offer greater performance and flexibility, they are more error-prone and require meticulous debugging.

Significant historical milestones, such as Carl Hewitt's **Actor Model (1973)** and the development of **Go’s Goroutines**, have shaped the evolution of concurrency paradigms. These advancements continue to influence how developers build scalable and efficient systems today.

---

## Research Question

> **How do functional and imperative programming languages address concurrency, and what significant historical developments influenced their evolution?**

---

## Interaction with LLM

To deepen my understanding, I engaged with a large language model (LLM) to explore how functional and imperative paradigms tackle concurrency. Through iterative questions, I gained insights into historical advancements like the **Actor Model** and frameworks such as **Akka** and **Goroutines**.

The LLM also provided high-level overviews and practical examples, which I verified against academic literature and official documentation. This collaboration helped clarify complex concepts and identify key trade-offs between paradigms.

For example:
- The LLM explained how **message passing** eliminates the need for shared memory, a hallmark of functional programming. This prompted further investigation into Erlang's concurrency model.
- It suggested looking into **Java’s thread model**, which inspired me to revisit Java’s **java.util.concurrent** package for more granular control over concurrency.

The process underscored the value of using LLMs as a starting point for research while cross-referencing with authoritative sources.

---

## Key Findings

1. **Functional Programming**:
   - Simplifies concurrency by emphasizing **immutability** and **pure functions**.
   - Adopts high-level abstractions like **message passing** and **STM** to avoid mutable shared state.
   - Examples: Erlang’s Actor Model, Haskell’s STM.

2. **Imperative Programming**:
   - Offers fine-grained control through **threads**, **locks**, and shared memory.
   - Introduces risks like **race conditions** and **deadlocks**, increasing debugging complexity.

3. **Trade-offs**:
   - Functional approaches reduce errors but may have performance overhead.
   - Imperative methods provide high performance but at the cost of greater complexity.

---

## Historical Developments

- **Actor Model (1973)**: Introduced by Carl Hewitt, it laid the foundation for message-passing systems, influencing languages like Erlang and frameworks like Akka ([source](https://scholar.google.com/scholar?q=Actor+Model+Carl+Hewitt)).
- **Java Threads**: Introduced in the 1990s, offering primitive concurrency mechanisms ([source](https://docs.oracle.com/javase/7/docs/api/java/lang/Thread.html)).
- **Go’s Goroutines**: Lightweight concurrency primitives enabling scalable applications ([source](https://golang.org/doc/effective_go#goroutines)).
- **Akka Framework**: A Scala-based framework leveraging the Actor Model for distributed systems ([source](https://akka.io)).

---

## Advantages and Disadvantages

| **Approach**        | **Advantages**                                 | **Disadvantages**                            |
|----------------------|-----------------------------------------------|---------------------------------------------|
| **Functional**       | Simpler concurrency, fewer bugs.              | Performance overhead, requires paradigm shift. |
| **Imperative**       | High performance, low-level control.          | Error-prone, debugging complexity.          |

---

## Discord Summary

In discussions this week, we compared lightweight threads like **Goroutines** to traditional heavyweight threads, exploring how each affects scalability and debugging. Functional programming’s reliance on **immutability** and **message passing** emerged as a safer, albeit less performant, model for concurrency. Conversely, imperative programming’s granular control, while powerful, demands careful management to avoid pitfalls like race conditions.

---

## References

1. Hewitt, C. (1973). **Actor Model of Computation**. [Scholar Link](https://scholar.google.com/scholar?q=Actor+Model+Carl+Hewitt).
2. Go Documentation. [Golang.org](https://golang.org/doc/effective_go#goroutines).
3. Akka Framework. [Akka.io](https://akka.io).
4. Oracle. **Java Threads Documentation**. [Oracle Docs](https://docs.oracle.com/javase/7/docs/api/java/lang/Thread.html).
5. Week 3 Literature Review. [GitHub](https://github.com/TEDJS235/Week-3/literature-review).

---
