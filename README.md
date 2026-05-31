# RayGPT Public Knowledge Graph

This repository publishes contains a knowledge graph that code-wizards can use with their coding agents.

The knowledge graph keeps relationships and concepts between functions and tools while removing private source path metadata. Feel free to extend this concept further based on your needs. 

## Quick Start for Users

### Option A: Clone the repository

```bash
git clone <your-github-repo-url>
cd <repo-name>
```

### Option B: Download ZIP from GitHub

1. Open the GitHub repository page.
2. Click **Code**.
3. Click **Download ZIP**.
4. Extract it and open the folder in your editor.

## Files You Need

- `public-graph/graph.json` -> machine-readable graph for coding agents
- `public-graph/graph.html` -> interactive visualization in browser
- `public-graph/manifest.public.json` -> export metadata

## View the Graph in Browser

Run a local static server from the repository root:

```bash
cd public-graph
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000/graph.html
```

## Use with Your Coding Agent

Typical workflow:

1. Point your agent/tool to `public-graph/graph.json`.
2. Ask it to answer questions using graph entities, communities, and edges.
3. Use `public-graph/graph.html` for manual exploration and validation.

Example prompts you can give your agent:

- "Load `public-graph/graph.json` and list the top communities by node count."
- "Find scripts or functions related to plan optimization and QA checks."
- "Show neighboring entities connected to `CheckClinicalGoals.py`."

## Limitations

This graph is excellent for discovery and relationship mapping, but it is not a full replacement for source code and knowledge.
