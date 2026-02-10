# Example: Data Analysis

## Before Lean
**User:** "analyze this"

**Agent:** "Analyze what? I don't see any data attached."

**Result:** Confusion and wasted tokens

---

## With Lean

**User:** "analyze this"

**Agent (Internal):** *Optimizes to:*

<task>Data Analysis Request</task>
<action>
1. Check for recently discussed files or data
2. If found, proceed with analysis
3. If not found, ask: "What would you like me to analyze? 
   (Recently you mentioned: [list recent context])"
</action>

**Agent:** "I see you recently worked with ~/Documents/sales_data.csv. Analyze that?"

**Result:** Smart context awareness, fewer wasted tokens
