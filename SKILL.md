# Lean - Cut the fat. Keep the smart.

## Description
Lean is a prompt optimization skill that makes your OpenClaw agent smarter and cheaper. Before executing any task, your agent automatically restructures vague prompts into high-performance, model-native formats, reducing failed attempts and saving tokens.

No extra setup. No new API keys. Your agent just gets better at understanding you.

## Installation
No installation required. Just send this skill to your agent and it will automatically start optimizing your prompts.

## When to Use
This skill activates automatically for ANY complex prompt, especially:
- Code generation or refactoring
- Long-form writing
- Data analysis
- Research tasks
- Multi-step workflows

Simple prompts (like "what time is it?") are passed through without optimization.

## How It Works

### Step 1: Detect Prompt Type
When user sends a prompt, first analyze:
- Is this a simple query (< 10 words, no context needed)? → Skip optimization
- Is this a complex task (coding, writing, analysis)? → Optimize it

### Step 2: Self-Optimize Using Master Framework
If optimization is needed, internally restructure the prompt using this framework:

<task>Clear, specific description of what to do</task>
<context>Relevant background information</context>
<constraints>Specific requirements, limitations, or format needs</constraints>
<output_format>Exactly how the result should be structured</output_format>

### Step 3: Execute with Optimized Prompt
Use the restructured version internally to generate the response.

### Step 4: Show Value to User
After completing the task, show a brief comparison:

"""
✨ Lean optimized your prompt

Before: "help me write code"
After: Structured task with context and constraints

💰 Estimated savings: $0.01 - $0.05
(Avoided 2-3 clarification rounds)
"""

## Master Prompt Template

When restructuring user prompts, follow these principles:

1. **Add Context**: Even if user didn't provide it, infer reasonable context
2. **Specify Output**: Always define the expected format (code, markdown, JSON, etc)
3. **Break Down Steps**: For complex tasks, create numbered sub-tasks
4. **Add Examples**: If task is ambiguous, include example of desired output
5. **Set Constraints**: Specify language, style, length, or technical requirements

Example transformations:
User: "summarize this article"
Optimized:
Content Summarization

Read the article completely
Extract 3-5 key points
Write a 2-3 sentence executive summary
<output_format>

Bullet points for key insights
Brief paragraph summary
Total length: 100-150 words </output_format>
User: "fix the bug in my code"
Optimized:
Debug Code
User has a bug but hasn't specified the error or language

Ask: What programming language?
Ask: What's the error message?
Ask: What should the code do?
Once clarified, analyze and fix

## Cost Savings Calculation

Estimate savings using this logic:

1. Count tokens in original prompt (rough: 1 token ≈ 4 chars)
2. Assume unoptimized prompts lead to 2-3 clarification rounds
3. Calculate: Rounds avoided × Avg tokens per round × Model price
4. Show range: $0.01 - $0.05 for most tasks

Model pricing reference (per 1M tokens):
- Claude 3.5 Sonnet: $3 input / $15 output
- GPT-4: $30 input / $60 output
- GPT-4o: $2.5 input / $10 output

## User Control

If user says:
- "Turn off Lean" or "Disable optimization" → Stop optimizing, pass prompts through directly
- "Turn on Lean" or "Enable optimization" → Resume optimization
- "Show me the optimization" → Display before/after comparison

## Privacy
All optimization happens using your existing API key. No data is sent to external services beyond your configured LLM provider.

## Output Format
Be transparent about optimization. Users should understand that Lean is helping them communicate more effectively with their agent.