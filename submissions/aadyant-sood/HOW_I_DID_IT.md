## What I Did

I set up the LPI Developer Kit locally and ran the test client to verify that all tools were working correctly. I also created a visual diagram to explain the SMILE methodology in a simple and user-friendly way.

---

## Step by Step

1. Cloned the repository
2. Installed dependencies using npm install
3. Ran the test client using npm run test-client
4. Verified all tools passed successfully
5. Used a local LLM to understand SMILE methodology
6. Created a visual diagram for better understanding

---

## Test Results

I ran the test client and confirmed that all LPI tools passed successfully:

* smile_overview
* query_knowledge
* analyze_patterns
* (all tools passed: 7/7)

---

## LLM Usage

I used TinyLlama via Ollama as a local LLM.

Prompt:
Explain SMILE methodology in simple terms and how it relates to digital twins.

Response:
The SMILE methodology is a structured approach used to model real-world systems as digital twins. It includes stages such as sensing data, modeling systems, integrating information, learning patterns, and generating insights.

---

## Model Choice

TinyLlama was chosen because it is lightweight, runs locally, and allows quick experimentation without external dependencies.

---

## SMILE Reflection

The SMILE methodology structures systems into phases that help model real-world entities as digital twins. It connects data collection, processing, and insight generation into a unified workflow.

---

## Problems Faced

Initially, I found it difficult to understand and simplify the SMILE phases. I also needed to structure the explanation in a way that is easy for non-technical users to understand.

---

## Learnings

I learned how digital twin systems are structured and how different phases of SMILE contribute to solving real-world problems. I also understood how LPI tools interact to generate insights.

---

## Level 3 Work

For Level 3, I designed a personal digital twin dashboard called LifeTwin using Figma.

The dashboard visualizes key health metrics such as sleep, energy, and stress. It includes a digital twin sync status and an AI-powered insight section to help users understand patterns in their daily routine.

---

## Explainability

The system generates insights based on patterns in user data such as sleep, energy, and stress.

For example:

* Low sleep + low energy → system suggests rest
* High stress → system highlights patterns

These insights are conceptually derived using LPI tools such as smile_overview and query_knowledge.
