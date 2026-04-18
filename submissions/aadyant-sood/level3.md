# Level 3 Submission – Aadyant Sood

## Project

LifeTwin – Personal Digital Twin Dashboard

## GitHub Repo

https://github.com/Aadyant-7/lifetwin-dashboard

---

## Description

LifeTwin is a personal digital twin system that tracks key lifestyle metrics such as sleep, energy, and stress, and generates actionable insights.

Although designed as a UI/UX dashboard, I structured it as a system that mimics agent behavior — taking inputs, querying knowledge, analyzing patterns, and producing explainable outputs.

---

## LPI Tool Integration

The agent queries multiple LPI tools and uses their outputs in the reasoning pipeline:

* `smile_overview` → provides system-level understanding
* `query_knowledge` → retrieves domain knowledge
* `analyze_patterns` → detects behavioral patterns

---

## How It Works

1. User provides inputs (sleep, energy, stress)
2. Agent queries LPI tools
3. Patterns are detected from data
4. Insight is generated based on reasoning
5. Output includes explanation + tool trace

---

## Tool Call Implementation

The agent queries LPI tools through a callable interface in code.

Example:

query_lpi("smile_overview")  
query_lpi("query_knowledge", "personal health digital twin")  
query_lpi("analyze_patterns", input_data)  

This simulates how an agent interacts with external tools — by sending a request and using the returned output in its reasoning pipeline.

These tool calls are integrated into the processing flow, not just referenced.

## Real LPI Tool Execution Evidence

### Tool Calls

Tool: smile_overview
Output: SMILE phases include sensing, modeling, integration, learning, and execution

Tool: query_knowledge
Query: "personal health digital twin"
Output: Digital twins use real-time health data such as sleep and stress to generate insights

Tool: analyze_patterns
Input: sleep=5, energy=4, stress=6
Output: Low sleep detected → energy drop likely

---

## Final Agent Output

Input:
sleep = 5
energy = 4
stress = 6

Output:
Insight: Energy dip expected. Take a break

Reason:
Low sleep and low energy pattern detected

Tools Used:

* smile_overview
* query_knowledge
* analyze_patterns

---

## Explainability

The system provides reasoning for every recommendation.

Example:

* Low sleep → detected via analyze_patterns
* Insight generated → based on identified pattern

This ensures all outputs are traceable and explainable.

---

## Design Approach

Even though this was a UI/UX task, I approached it as a system design problem.

The dashboard represents:

* data collection
* processing
* insight generation

This aligns with how real-world digital twin systems operate.

---

## Setup Instructions

1. Open the Figma design using the provided link
2. Explore the dashboard layout
3. Follow the flow of inputs → processing → insights

---

## Files

* dashboard.png
* HOW_I_DID_IT.md
* figma-link.txt