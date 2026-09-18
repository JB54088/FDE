# Technical Difficulty Signals

Use this reference when a customer's wording hides substantial engineering complexity.

## 1. "Automatic"

Ask what happens when confidence is low, inputs are missing, the target system is unavailable, or the action is irreversible. Full automation requires exception handling, retry logic, state management, permissions, monitoring, and recovery paths.

## 2. "Real-time"

Real-time requirements add latency budgets, streaming ingestion, concurrency, partial-result handling, network instability, synchronization, and monitoring. A batch workflow that finishes correctly after several minutes is a different product from a live workflow expected to react in seconds.

## 3. "Accurate" or "must be correct"

Clarify the acceptable error type and consequence. Model outputs are probabilistic. High-stakes workflows often need deterministic validation, source evidence, confidence thresholds, and human confirmation.

## 4. "All" / "entire internet" / "every system"

Coverage claims are normally constrained by access, indexing, robots rules, login requirements, API availability, private data, anti-bot controls, inconsistent formats, and changing websites.

## 5. "Directly write it into the system"

This is an integration problem, not only an AI problem. Check API availability, authentication, field mapping, write permissions, validation rules, audit requirements, rollback, duplicate prevention, and error handling.

## 6. "No human needed"

Check whether the human currently carries accountability, approves irreversible actions, handles edge cases, manages relationships, resolves ambiguity, or performs physical actions. If yes, the likely target is human-AI collaboration, not complete replacement.

## 7. "Guarantee"

A guarantee usually changes a probabilistic AI task into a system-level reliability commitment. Identify what can be validated deterministically and what cannot.

## 8. "Once deployed, it should never need maintenance"

External APIs, websites, models, security rules, credentials, business processes, and data formats change. Production automation requires observability and maintenance even when the user-facing workflow appears stable.

## 9. "It just needs to understand what the user means"

Natural-language understanding may be easy in a narrow case but difficult when intent is ambiguous, context is missing, users contradict themselves, terminology changes, or the action has business consequences. Add clarification paths and confidence-based fallbacks.

## 10. "Replace this employee"

Decompose the role into tasks before judging replacement. Many roles combine information processing with judgment, trust, accountability, coordination, and exception handling. AI may automate tasks without eliminating the role.
