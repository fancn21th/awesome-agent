# Agent Levels

You can think of L1 to L4 as four progressive levels of agent capability. This is not an industry-wide standard, but it is a very practical engineering-oriented way to classify agent systems.

## L1: Prompted Assistant

At its core, this is a large-model application wrapped with a system prompt.

Key characteristics:

- Most of its capability comes from prompting.
- It takes one input and produces one output.
- It does not execute real tools.
- It cannot read from or write to an external environment.

Typical examples:

- Standard chatbots.
- Copywriting generators.
- Summarization, translation, and Q&A pages.

It can answer, but it cannot do.

## L2: Tool-Using Agent

At its core, this is where the model starts calling tools.

Key characteristics:

- The model can decide when to call a tool.
- It has a basic action loop: think, call a tool, continue generating.
- It can look up information, send requests, and execute functions.
- Its understanding of environment state is usually still weak.

Typical examples:

- AI assistants that can search the web.
- Customer support agents that call databases or APIs.
- Agents that generate charts, send emails, or create calendar events through functions.

At this level, the system no longer just answers questions. It can use tools to complete tasks.

## L3: State-Aware Agent

At its core, this is where the model not only calls tools, but first understands the current environment and then performs incremental operations.

Key characteristics:

- It reads the current state before making decisions.
- It modifies existing context instead of rebuilding everything from scratch every time.
- It emphasizes environment consistency, object references, and resource constraints.
- It behaves more like it is operating a real system than calling isolated functions.

Typical examples:

- A diagram agent that reads the current canvas before adding, deleting, or editing shapes.
- A writing agent that reads the current document before making local revisions.
- A workflow agent that checks current task status before updating a process.

At this point, the agent starts to feel like it has a model of world state, rather than being only a function router.

## L4: Evaluated Engineering Agent

At its core, this is where the agent enters an engineering optimization phase.

Key characteristics:

- It has test sets, evals, scorers, or benchmarks.
- It can systematically compare prompt, tool, or strategy changes before and after an iteration.
- It can be improved continuously instead of being judged by subjective demos.
- It focuses on stability, regressions, and success rate, not just single-run performance.

Typical examples:

- An agent with a golden dataset.
- An agent with scorers for tool choice, structure, or schema quality.
- An agent workflow that supports A/B comparison and regression checks.

It is not just usable. It is manageable and improvable over time.

## One-Line Summary

- L1: Can talk.
- L2: Can use tools.
- L3: Can understand and operate on environment state.
- L4: Can be systematically evaluated and iteratively optimized.

## A Common Point Of Confusion

L1 to L4 is not purely about being smarter. It is more about being more engineered, more executable, and more controllable.

Many projects use strong models, but if they lack tools, state handling, or evaluation, they still belong to a lower level.

## How To Apply This To A Project

If you apply this lens to a real project:

- If it supports tool calling, it is already beyond L1.
- If it reads current state before making changes, it is beyond L2.
- If it has evals and scorers, it is approaching or already at L4.

This framing is useful because it shifts the question from "How smart is the model?" to "How much real work can the system do, and how well can we improve and control it?"