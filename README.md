# SyntaxSentinel — Pedagogical Code Review Assistant (C4)
**Course:** Prompt Engineering (SCSE4041) | **Team ID:** PE-B49-07 | **Team Name:** Code Gaurdians  
**Faculty Mentor:** Dr. Ankit Vijay Bansal | **Batch:** 58  

## Overview
SyntaxSentinel is a two-stage prompt-engineered code review mentor for first-year programming students learning **Python** and **C**. Unlike standard AI assistants that leak complete solutions, SyntaxSentinel diagnoses syntax, logic, memory-bounds, and style bugs while providing Socratic hints that guide students to fix their own code.

## Live Prototype Link
* **Google AI Studio Prototype:** (https://aistudio.google.com/app/prompts?state=%7B%22ids%22:%5B%221ctTeMsz1bidCn9g6LnS0YoNj2C1z8HnS%22%5D,%22action%22:%22open%22,%22userId%22:%22108000139777286792633%22,%22resourceKeys%22:%7B%7D%7D&usp=sharing)

## Prompt Pipeline Architecture
1. **P1 (`prompts/final/P1_code_triage.txt`):** Classifies language, detects line-level bugs, and outputs a strict JSON diagnosis.
2. **P2 (`prompts/final/P2_pedagogical_mentor.txt`):** Consumes the student code and P1's JSON output to generate two-tier Socratic hints under strict anti-solution guardrails.

## Team Members & Contributions
* **Pragati Singhal** (`S24CSEU1650`) — Team Leader, Prompt Architecture (`P1` & `P2`), Guardrail Engineering & GitHub Repository 
* **Aastha Sucheta** (`S24CSEU0192`) — Evaluation Test Suite Design (Normal/Edge/Invalid Cases), Error Analysis & Technical Report 
* **Hritvika Chunduri** (`S24CSEU0716`) — Prompt Iteration Benchmarking (`v1`–`v4`), Workflow Diagrams & Demonstration Reel
