# Literature Review: Concurrency in Functional and Imperative Programming

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
7. [References](#references)

---

## Introduction

This literature review explores the question:  
**"How do functional and imperative programming languages address concurrency, and what significant historical developments influenced their evolution?"**

---

## Research Question

The research focuses on:  
> **How do functional and imperative programming languages address concurrency, and what significant historical developments influenced their evolution?**

---

## Exploration with LLM

### Question 1: What are the fundamental differences between functional and imperative approaches to concurrency?  
- Functional programming avoids shared state by leveraging **immutability** and concepts like **message passing**.  
- Imperative programming relies on threads, locks, and shared memory, which are error-prone but efficient for systems-level programming.

### Question 2: What historical milestones shaped the development of concurrency?  
- **1960s**: Thread-based systems in **C** and **Unix**.  
- **1973**: Actor Model by **Carl Hewitt**.  
- **1980s**: Erlang’s message-passing model.  
- **1990s–2010s**: Java threads, Haskell STM, and Akka frameworks.

### Question 3: Advantages and Disadvantages  
| Approach              | Advantages                                    | Disadvantages                              |
|-----------------------|-----------------------------------------------|-------------------------------------------|
| **Functional**        | Easier to debug; immutability ensures safety. | New paradigms for developers; overhead.   |
| **Imperative**        | Familiar and efficient.                      | Error-prone and complex debugging.        |

---

## Key Findings

1. Functional approaches prioritize safety and simplicity using immutable state.  
2. Imperative approaches emphasize performance but introduce complexity through shared state.  

---

## Historical Developments

- **Actor Model** (Carl Hewitt, 1973).  
- **Java Threads** and concurrency primitives.  
- **STM** in Haskell and lightweight threads in **Go**.  

---

## References

1. Carl Hewitt, “The Actor Model” (1973).  
2. Go’s Goroutines: [https://golang.org/](https://golang.org/)  
3. Akka Framework for Scala: [https://akka.io/](https://akka.io/)  

---

## Discord Summary

> **Summary**: In Week 3, I explored how functional and imperative programming languages address concurrency. Functional programming uses immutability and message-passing systems like the Actor Model to simplify concurrency, while imperative programming relies on threads and locks. Historical milestones include the Actor Model (1973), Java threads (1990s), and STM frameworks (2000s).  
>  
> **Question**: *What are the major trade-offs between lightweight threads (e.g., Go's Goroutines) and heavy threads in traditional imperative languages?*  
>  
> **Link to GitHub Repository**: [Insert URL Here]

---

# Week-3
