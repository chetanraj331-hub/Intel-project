Substrate → Packaging → Facility Knowledge Graph

An interactive, sourced and weighted knowledge graph with a multi-agent simulation of semiconductor substrate supply risk, built as part of my IIM Mumbai capstone on Intel (June 2026).

🔗 Live demo: https://github.com/chetanraj331-hub/Profile/blob/main/substrate_agent_graph_v2.html

Problem

Advanced packaging for AI and client chips depends on a few chokepoints, such as ABF film, FCBGA substrate makers and a small set of facilities. It is hard to see how a price hike, a capacity expansion or geopolitical risk at one layer moves risk elsewhere in the chain.

What it does
Maps the chain: raw materials → substrate suppliers → packaging tech (EMIB, EMIB-T, Foveros) → facilities (state/country) → processors → end use
Overlays PESTEL factors on the chain
~50 nodes and ~100 relationships; node size and shape show the current weight tier (normal / elevated / high / critical)
33 cited sources; every node carries a confidence tag (high / medium / estimate) and a business-impact note
Agents tab: toggle simulated agents (Supply Concentration, Cost & Pricing, Capacity & Investment) and recompute weights
Live AI tab: optional Gemini call with Google Search grounding, running in the browser (your key stays in memory and is never saved)
Manual override: click a node and drag its weight slider
My role

Designed the model, collected and cited the sources, defined the agent logic and weighting, and built the D3 visualization. The output feeds prioritized capacity-planning recommendations.

Tech

JavaScript, D3.js v7, Gemini API (optional). A single self-contained index.html.
