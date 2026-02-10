# Example: Code Generation

## Before Lean
**User:** "write me a function"

**Agent:** "What should the function do? Which language?"

**User:** "oh, Python, to validate email"

**Agent:** "Generating..."

**Cost:** 3 rounds × ~2000 tokens = ~$0.03

---

## With Lean

**User:** "write me a function"

**Agent (Internal):** *Optimizes to:*

<task>Function Generation</task>
<language>Python</language>
<purpose>Email validation</purpose>
<constraints>
- Use regex for RFC 5322 compliance
- Handle edge cases (subdomains, special chars)
- Return boolean
</constraints>
<output>Complete function with docstring and test cases</output>

**Agent:** "Here's your email validation function..." *(delivers immediately)*

**Cost:** 1 round × ~1500 tokens = ~$0.01

**Savings:** $0.02 (67% reduction)
