# Data Structures — First Principles (JS)

This repository documents my journey of learning **Data Structures from first principles**, not for interviews, but to **think clearly about systems**.

The focus is on:

- _Why_ a data structure exists
- _What problem it replaced_
- _Where it breaks_
- _How CRUD actually behaves internally_

Everything is written in **JavaScript**, with system-level reasoning (memory, cost, tradeoffs).

---

## Philosophy

This is **not**:

- LeetCode practice
- Pattern memorization
- Competitive programming
- Speed-focused problem solving

This **is**:

- Data structures as **mini-systems**
- Understanding **constraints before solutions**
- Learning to say:  
  _“This structure fails here, this one fits better”_

Problem solving will come **later**, as a byproduct.

---

## How This Repo Is Organized

Each topic is organized by **day and structure**, not by difficulty.

```
Day_01_What_is_a_Data_Structure/
Day_08_Arrays/
Day_15_Strings/
Day_20_Linked_Lists/
Day_36_Stacks_and_Queues/
Day_50_Hash_Tables/
Day_75_Trees/

```

Each folder contains notes and experiments related to **one structure only**.

---

## Structure of Each Day / Topic

Each folder follows the same mental model:

### 1. Why This Exists

- What problem existed before this structure?
- Why earlier approaches failed

### 2. Core Constraints

- What operations are cheap
- What operations are expensive
- What invariants must be preserved

### 3. CRUD Breakdown

- **Create** – memory layout, initialization cost
- **Read** – what is actually traversed
- **Update** – what can break internally
- **Delete** – what becomes costly or complex

If CRUD isn’t clear, the structure isn’t understood.

---

### 4. Tradeoffs & Failure Points

- Where this structure performs badly
- What happens at scale
- Why it’s misused in real systems

---

### 5. JavaScript Reality Check

- How JS implements or abstracts this structure
- What JS hides vs what still matters
- Differences from lower-level implementations

---

### 6. Implementations (When Applicable)

- Built from scratch in JS
- No built-in helpers unless explicitly noted
- Focused on correctness and clarity, not cleverness

---

### 7. Observations

- Things that felt counter-intuitive
- Mental model shifts
- Mistakes or wrong assumptions corrected

---

## Ground Rules I Follow

- No problem-solving platforms during this phase
- No premature optimizations
- No advanced variants before understanding the pain
- Depth > coverage
- Clarity > speed

---

## Goal of This Repository

By the end of this journey, I should be able to:

- Choose the right data structure for a real system
- Explain **why** a structure fits or fails
- Implement core structures without relying on libraries
- Think in **constraints and tradeoffs**, not tricks

---

## Status

This is a **living repository**.  
Notes will evolve as understanding deepens.

Confident understanding > early correctness.

---
