# NewsAware: A Domain-Adaptive, Knowledge-Aware Newsroom Agent
A prototype agent for knowledge-grounded evaluation of news and public claims.

## Overview
NewsAware is a prototype AI agent designed to analyze news and text for sentiment, credibility, and factual reliability.

## Research Motivation

Current AI systems often generate fluent but unreliable outputs, including unsupported claims and subtle misinformation. This is especially critical in journalism, where factual accuracy and trust are essential.

NewsAware is motivated by the need for:
- Evidence-aware reasoning in language models  
- Detection of overgeneralized or misleading claims  
- Structured evaluation beyond surface-level text generation  

This project represents a first step toward knowledge-grounded and domain-adaptive AI systems.

## Architecture

![NewsAware Architecture](assets/process.png)

## Problem
Large language models often generate:
- Unsupported claims
- Hallucinated facts
- Biased or exaggerated statements

This is critical in journalism, where accuracy and trust are essential.

## Approach
NewsAware uses a simple agentic workflow:

Input → Analyze → Check Evidence → Refine

- Analyze: Extract sentiment and key claim  
- Check: Evaluate presence of supporting evidence  
- Refine: Adjust credibility based on reasoning  

## Workflow

Input → Analyze → Check Evidence → Refine

## Example

Input:
"Studies show that prolonged mobile phone use and blue light exposure significantly harm cognitive function and mental health."

Output:
- Sentiment: Negative  
- Credibility: Medium–Low  
- Reason:
  - Uses vague attribution ("studies show") without citing sources  
  - Overstates scientific consensus on cognitive and mental health effects  
  - Does not distinguish correlation from causation  
  - Lacks verifiable sources or references
 
## Future Direction
- Knowledge graph integration  
- Retrieval-based evidence checking (RAG)  
- Multi-step evaluation agents
