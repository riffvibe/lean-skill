# Lean - Cut the fat. Keep the smart.

<p align="center">
  <img src="https://img.shields.io/badge/OpenClaw-Skill-orange" alt="OpenClaw Skill">
  <img src="https://img.shields.io/badge/Cost-$0-green" alt="Free">
  <img src="https://img.shields.io/badge/Setup-Zero-blue" alt="Zero Setup">
</p>

**Make your agent smarter. Automatically.**

Lean optimizes every prompt before your OpenClaw agent executes, reducing failed attempts and saving you money.

## The Problem

You: "help me write code"  
Agent: "Sure! What language? What should it do? Any frameworks?"  
You: "oh, Python, to scrape websites, use requests"  
Agent: "Got it, generating..."

**Result:** 3 rounds of back-and-forth. $0.05+ wasted. Frustration.

## The Solution

Install Lean. Same conversation becomes:

You: "help me write code"  
Lean: *[Internally restructures to model-native format]*  
Agent: *[Generates perfect code immediately]*

**Result:** 1 round. $0.01 used. Done.

---

## Key Features

✨ **Automatic Optimization** - No manual work  
💰 **Real Savings** - Avoid 2-3 clarification rounds per task  
🎯 **Higher Success Rate** - Structured prompts = better results  
🔒 **Privacy First** - Uses your existing API key, no external calls  
⚙️ **Zero Setup** - Just install and forget  

---

## Installation

Send this to your OpenClaw agent:
Read https://vibemate-web.vercel.app/lean/skill.md and follow the instructions.

That's it. Lean activates automatically.

---

## How It Works

1. **You send a prompt** (like you always do)
2. **Agent detects complexity** (simple query vs complex task)
3. **If complex:** Agent internally restructures using model-native format
4. **Agent executes** optimized version
5. **You get better results** + see estimated savings

---

## Estimated Savings

| Your Usage | Without Lean | With Lean | Savings |
|------------|--------------|-----------|---------|
| 10 tasks/day | ~$15/month | ~$5/month | **$10/month** |
| 30 tasks/day | ~$45/month | ~$15/month | **$30/month** |
| 100 tasks/day | ~$150/month | ~$50/month | **$100/month** |

*Based on Claude 3.5 Sonnet pricing. Actual savings vary by task type.*

---

## Examples

### Before Lean
User: "make this faster"
Agent: "What are you referring to? Code? Process? Network?"
User: "the python script"
Agent: "Which script? What's slow?"
User: "the one in ~/projects/scraper.py"
Agent: "Analyzing..."

### With Lean
User: "make this faster"
Agent: [Internally optimizes to:]
"Analyze ~/projects/*.py files, identify performance
bottlenecks, suggest optimizations for speed"
Agent: "Found 3 optimization opportunities in scraper.py..."

---

## User Control

- Say **"turn off Lean"** to disable
- Say **"turn on Lean"** to re-enable  
- Say **"show optimization"** to see before/after

---

## Privacy & Cost

- ✅ Uses your existing OpenClaw API key
- ✅ No separate registration
- ✅ No data sent to third parties
- ✅ Open source - verify yourself

---

## FAQ

**Q: Does this slow down my agent?**  
A: Adds ~0.5-1 second per prompt. Saves 2-3 entire rounds of conversation.

**Q: What if the optimization makes it worse?**  
A: Just say "turn off Lean" and it stops immediately.

**Q: Will this work with any LLM?**  
A: Yes. Works with Claude, GPT, local models, etc.

---

## Links

- Website: https://vibemate-web.vercel.app/lean
- Install: https://vibemate-web.vercel.app/lean/skill.md
- Feedback: yaneinstein@gmail.com

---

**Built with ❤️ for the OpenClaw community**

Inspired by @steipete's CLI-first philosophy.