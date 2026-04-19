Here is the link to my Level 3 AI Agent repository:
https://github.com/jv-singh/smile-ai-agent

### Evidence 1: Real Response from LPI Tools
My code actively calls the LPI tools by spawning the Node.js server as a subprocess and sending JSON-RPC requests. Here is the actual raw text returned by the `smile_overview` tool when my code calls it, proving the connection works:

> # S.M.I.L.E. — Sustainable Methodology for Impact Lifecycle Enablement
> Benefits-driven digital twin implementation methodology focusing on impact before data.

### Evidence 2: Explainability (Provenance)
Explainability isn't just a feature in my agent, it's structurally forced. The agent prints a dedicated provenance block at the end of every execution so the user knows exactly where the data came from. Here is the exact output:

PROVENANCE (tools used)
[1] smile_overview (no args)
[2] query_knowledge ({"query": "What is SMILE methodology?"})
[3] get_case_studies (no args)