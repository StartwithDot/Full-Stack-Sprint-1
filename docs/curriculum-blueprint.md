# Full Stack Sprint 1 — Curriculum Blueprint

**Status: Working draft**

## 1. Purpose

This document defines how Sprint 1 will be designed around one real project: **Poll Maker**.

The project is the vehicle for learning. Topics should not be introduced merely because they are part of a technology stack. A new concept should appear because the learner has encountered a problem that the concept helps solve.

The intended progression is:

```
Project need
  ↓
New problem
  ↓
Why does this problem exist?
  ↓
New concept
  ↓
Individual practice
  ↓
Use the concept in Poll Maker
  ↓
Checkpoint
  ↓
Next problem
```

## 2. Learner profile

Sprint 1 must work for:

- learners with no formal IT background
- learners with some digital experience
- learners with prior programming experience

The curriculum therefore needs to distinguish between:

### Foundation

Mental models and basic skills required to participate:

- files and folders
- editor and terminal
- browser and developer tools
- HTML structure
- CSS basics
- JavaScript fundamentals
- variables, values, arrays, objects, conditions, loops, functions
- events and debugging

### Full-stack concepts

Concepts created by the need for different parts of an application to communicate:

- browser vs server
- request and response
- HTTP
- JSON
- APIs and routes
- asynchronous operations
- persistence
- database concepts
- SQL
- CRUD

### Product-engineering awareness

Introduced lightly in Sprint 1 and developed further in later sprints:

- validation
- error handling
- user experience
- security limitations
- architecture
- testing
- deployment
- maintainability

Sprint 1 should prioritise understanding over breadth.

## 3. Core project

### Poll Maker

A single-poll voting application:

- one question
- multiple options
- anyone can vote
- vote counts are stored persistently
- options can be added and removed
- results can be displayed visually

Deliberate scope limits are part of the curriculum. Advanced features should be deferred when adding them would hide the underlying learning.

## 4. The learning rule

Every major concept should answer four questions:

1. **What can we do now?**
2. **What problem do we have now?**
3. **What new idea solves that problem?**
4. **What will we build to prove we understand it?**

The curriculum should avoid introducing a technology without first establishing the problem it solves.

## 5. Project arc

The starting phase model is:

| Phase | Purpose |
|---|---|
| Understand | establish the web/application mental model and define the Poll Maker |
| Practice | learn and practise foundations and first full-stack concepts |
| Build | assemble the browser, server and database into one working application |
| Deliver | improve reliability, document the system, demonstrate understanding and hand over |

These phases are a planning model, not a fixed week count.

## 6. Proposed milestone logic

Milestones are gates that demonstrate shared understanding before the next dependency is introduced.

### Milestone 1 — Discovery / Web Mental Model

The learner can explain the basic browser/application relationship and what is being built.

### Milestone 2 — First Working Frontend

The poll works using in-memory browser data.

The limitation is intentional: refreshing loses the data.

That limitation creates the need for persistence.

### Milestone 3 — First End-to-End Flow

A request can travel:

browser → server → database → server → browser

and the learner can explain each step.

### Milestone 4 — Core Poll Maker

The core voting and option-management behaviour works using persistent data.

### Milestone 5 — Handover

A fresh learner can run the project from the written setup instructions, and the original learner can explain the important layers and decisions.

## 7. Task design

A final task system should retain the traceability principles used in the Data Engineering curriculum:

- stable task IDs
- clear working order
- exact file paths
- reviewable evidence
- one task mapped to a concrete outcome

The exact track letters, group numbers and task counts are **not yet final**.

## 8. Time-box design

Each unit should answer:

### Before you start

What should be read, understood or prepared?

### By the end you can

What can the learner actually do?

### At a glance

Which concepts are being learned and which tasks immediately use them?

### Task groups

What does the learner build or investigate?

### Teaching notes

What is the common trap? What proves it is correct? Why will this matter later?

### End-of-unit checkpoint

What evidence shows that the learner understood rather than copied?

### If time is short

Which tasks can be reduced without breaking a milestone?

## 9. Teaching philosophy

The central principle is:

> Every new concept should arrive because the existing system has reached a meaningful limitation.

Examples:

- browser memory is temporary → persistence becomes necessary
- one page cannot permanently own the data → a server becomes useful
- the server needs durable storage → database becomes necessary
- the browser and server need to communicate → HTTP/API concepts become necessary
- the request takes time → asynchronous thinking becomes necessary
- users can make invalid requests → validation and error handling become necessary
- localStorage is not security → authentication becomes a future-sprint problem
- polling is not true real-time → WebSockets become a future-sprint problem

## 10. Relationship to later sprints

Sprint 1 should intentionally create questions that later sprints can answer.

The exact Sprint 2 and Sprint 3 curriculum is outside the scope of this document, but Sprint 1 should leave clear conceptual hooks rather than pretending the first version is a complete production system.

## 11. Repository design

The repository should preserve the distinction between:

- **individual practice** — safe space to learn and make mistakes
- **shared build** — the real group product
- **curriculum/docs** — the material that explains the journey
- **delivery** — final communication and handover
- **admin** — operational pointers where required

The exact technical source tree for the Poll Maker will be decided after the learning architecture is reviewed.

## 12. Design checklist

Before publishing Sprint 1, verify:

- [ ] the project is small enough to understand end to end
- [ ] every major concept is introduced because of a project need
- [ ] beginner prerequisites are explicit
- [ ] intermediate learners are still challenged
- [ ] milestones test understanding, not just completion
- [ ] learning outcomes are written as actions
- [ ] the shared build is separated from individual practice
- [ ] task IDs and cross-references are stable
- [ ] future-sprint hooks are explicit
- [ ] no advanced technology is included merely for appearance
