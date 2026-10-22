# RAG Website Chatbot

**Status:** Built; production deployment status is not specified

## Overview

I built a retrieval-augmented generation (RAG) website chatbot designed to answer questions using retrieved information rather than relying only on a language model's general knowledge. The project combined a retrieval pipeline with contextual prompt construction and LLM response generation in a website chatbot experience.

## My contribution

I implemented document ingestion, retrieval for user questions, contextual prompt construction, and LLM response generation. I also implemented context-grounded response generation intended to improve relevance and reduce unsupported responses.

This was an implemented engineering approach, not a claim that retrieval eliminates hallucinations. No measured hallucination-reduction percentage or formal answer-quality score is available, and the resume does not specify production traffic or a production service-level objective.

## High-level workflow

Document ingestion → retrieval for a user question → contextual prompt construction → LLM response generation → website chatbot response

At query time, retrieved information supplied context for generation. This kept the response process connected to the ingested material, while still leaving the generated answer subject to the quality of retrieval and the behaviour of the language model.

## Technology

The supported technical description is deliberately capability-focused: document ingestion, information retrieval, contextual prompt construction, LLM integration, and a website chatbot interface. The available brief does not identify a particular frontend or backend framework, vector database, embedding model, chunking method, or reranking implementation, so none is claimed here.

## Engineering considerations

RAG separates two quality problems that need to be considered together. Retrieval must surface useful context for the question, and generation must use that context appropriately. A fluent response can still be wrong when retrieval is weak, the source material is incomplete, or the model draws unsupported conclusions.

Grounding was therefore an architectural approach intended to improve relevance and reduce unsupported answers, not a guarantee of factual correctness. The public evidence does not establish user-visible citations, access-control enforcement, prompt-injection protection, or an implemented fallback or escalation path, so this case study does not imply those features.

## Outcomes and limitations

I delivered a website chatbot combining retrieval and LLM generation. Production deployment status, deployment scale, and formal evaluation methodology are not specified in the resume brief. No quantitative claim is made about answer quality, latency, cost, usage, or hallucination reduction, and completed production hardening is not claimed.

## Evidence

This sanitised description excludes private source documents, proprietary prompts, credentials, and employer-owned implementation. It records my stated contribution and the implemented high-level workflow without treating unavailable public code as evidence that the work is unknown.
