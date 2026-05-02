# NewsAware: A Domain-Adaptive, Knowledge-Aware Newsroom Agent

## Overview
NewsAware is a prototype AI agent designed to analyze news and text for sentiment, credibility, and factual reliability.

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

## Example


Input:
"Recent reports confirm that a widely used COVID-19 vaccine increases the risk of severe neurological disorders, but this information is being suppressed by mainstream media."

Output:
- Sentiment: Negative  
- Credibility: Low  
- Reason:
  - Makes a serious public health claim without citing verifiable sources  
  - Uses vague attribution ("recent reports") without evidence  
  - Suggests conspiracy framing ("information is being suppressed")  
  - No supporting data, study, or institution referenced  

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
  - Lacks specific evidence or data  

## Future Direction
- Knowledge graph integration  
- Retrieval-based evidence checking (RAG)  
- Multi-step evaluation agents
