# RAG Levels

You can think of L1 to L4 as four progressive levels of RAG capability. This is not an industry-wide standard, but it is a practical engineering-oriented framework for understanding how retrieval systems mature.

This version is organized around the three core dimensions of RAG:

- R: Retrieval
- A: Augmentation
- G: Generation

The point is not only to say that one level is "better" than another, but to show how the system changes across these three dimensions as it becomes more engineered.

## L1: Stuffed Context

At its core, this is not really RAG yet. It is an application that manually places reference material into the prompt.

R:

- There is no real retrieval step.
- Context is selected manually by humans or fixed templates.
- The system cannot dynamically search for the right knowledge.

A:

- Reference material is copied directly into the prompt.
- Augmentation is static and usually the same for every user or request.
- There is little or no logic for filtering, ranking, or adapting context.

G:

- The model generates an answer from the stuffed prompt.
- Output quality depends heavily on prompt wording and whatever context was manually included.
- Generation may look informed, but it is limited by a fixed context window.

Key characteristics:

- There is no retrieval step.
- The system depends on humans or fixed templates to decide what context to include.
- It works only when the amount of knowledge is small and stable.

Typical examples:

- A chatbot with a pasted FAQ block in the system prompt.
- A demo app with a few hardcoded product notes.
- A support assistant that uses one fixed reference document.

It can answer with extra context, but it cannot scale knowledge access.

## L2: Search-Based RAG

At its core, this is where the system starts retrieving relevant information from an external knowledge source.

R:

- The system retrieves relevant chunks from a knowledge source.
- Retrieval is usually driven by keyword search, vector search, or hybrid search.
- The main goal is recall and relevance for the current query.

A:

- Retrieved chunks are inserted into the prompt before generation.
- Augmentation becomes dynamic instead of fixed.
- The system may apply basic chunk selection, truncation, or ordering.

G:

- The model generates an answer grounded in the retrieved context.
- Generation quality depends not only on the model, but also on retrieval quality and prompt assembly.
- Hallucination risk is reduced, but weak retrieval still causes weak answers.

Key characteristics:

- It has a retrieval step before generation.
- It uses search, embeddings, or hybrid retrieval to find relevant chunks.
- Retrieved context is injected into the prompt for answer generation.
- Quality depends heavily on chunking, indexing, and retrieval relevance.

Typical examples:

- A docs chatbot backed by vector search.
- A knowledge base assistant that retrieves articles before answering.
- An internal company search assistant over handbooks or tickets.

At this level, the system no longer relies on manually stuffed context. It can fetch knowledge on demand.

## L3: State-Aware RAG

At its core, this is where retrieval becomes aware of user state, task context, and interaction history.

R:

- Retrieval depends on user state, session history, task context, or environment state.
- The system can retrieve differently for different users, roles, steps, or tasks.
- Retrieval may include routing, filtering, re-ranking, and multi-stage search.

A:

- Augmentation is no longer just "append top-k chunks".
- The system can merge retrieved knowledge with working context, prior messages, or intermediate results.
- Augmentation becomes selective, structured, and aware of what the model already knows in the current workflow.

G:

- Generation uses both retrieved knowledge and current state to produce context-sensitive output.
- The model can generate answers, edits, or actions that are specific to the current environment.
- Output becomes less like generic Q&A and more like task-aware assistance.

Key characteristics:

- Retrieval depends on the current task, session, user, or environment state.
- The system can combine short-term context with long-term knowledge.
- It can refine, re-rank, filter, or route retrieval based on what is already known.
- It behaves more like a working memory system than a single-shot search pipeline.

Typical examples:

- A coding assistant that retrieves code differently based on the current file and cursor position.
- A writing assistant that retrieves background material based on the current draft section.
- A workflow assistant that retrieves different procedures based on the current ticket state.

At this point, RAG starts to feel context-aware instead of being just search plus prompt stuffing.

## L4: Evaluated Engineering RAG

At its core, this is where RAG becomes an engineered system that can be measured, compared, and improved continuously.

R:

- Retrieval is measured with metrics such as hit rate, MRR, nDCG, recall, or passage relevance.
- Different retrievers, chunking strategies, embedding models, and rerankers can be compared systematically.
- Retrieval quality is no longer judged only by intuition.

A:

- Augmentation strategies are treated as tunable system design choices.
- Teams can compare prompt templates, chunk ordering, citation formatting, context compression, and schema structure.
- Augmentation is optimized for groundedness, efficiency, and task success.

G:

- Generation is evaluated for factuality, grounding, usefulness, task success, and regression risk.
- Output quality is tested with eval sets, scorers, or business metrics.
- Generation becomes part of an iterative engineering loop, not a one-off demo layer.

Key characteristics:

- It has eval sets, retrieval metrics, answer-quality scorers, or business success metrics.
- It can compare chunking, embedding models, retrievers, rerankers, and prompting strategies.
- It tracks regressions in retrieval quality, grounding, citation accuracy, or task success.
- It is optimized through systematic iteration rather than subjective demos.

Typical examples:

- A RAG system with a golden question set and expected supporting passages.
- A retrieval pipeline with hit-rate, MRR, nDCG, or groundedness evaluation.
- A production workflow that runs A/B tests across retrieval and generation strategies.

It is not just a RAG demo. It is a RAG system that can be operated and improved like real infrastructure.

## One-Line Summary

- L1: R is manual, A is static, G is prompt-bound.
- L2: R becomes searchable, A becomes dynamic, G becomes retrieval-grounded.
- L3: R becomes state-aware, A becomes context-aware, G becomes task-aware.
- L4: R, A, and G all become measurable and continuously optimizable.

## A Common Point Of Confusion

RAG maturity is not only about better models or bigger vector databases. It is about how retrieval improves, how augmentation becomes more selective and structured, and how generation becomes more grounded and testable.

Many teams say they have RAG when they only have L1 or a weak L2 pipeline. If retrieval is not state-aware and cannot be evaluated, the system is still at an early stage.

## How To Apply This To A Project

If you apply this lens to a real project:

- If R is still manual, A is still fixed, and G only works off stuffed prompts, it is L1.
- If R can search a knowledge base and A can dynamically insert retrieved context, it is at least L2.
- If R changes with state and A adapts to workflow context, it is L3.
- If R, A, and G are all evaluated and optimized with metrics or evals, it is approaching or already at L4.

This framing is useful because it shifts the question from "Do we have RAG?" to "How do retrieval, augmentation, and generation evolve as the system becomes more robust, context-aware, and improvable?"
