# Graphify Analysis Summary

## Repository
- **Name:** refacer
- **Model:** gemini-2.5-flash-lite
- **Analysis Date:** 2026-06-16

## Graph Metrics
- **Nodes:** 165
- **Edges:** 195
- **Communities:** 11 (10 shown, 1 thin omitted)

## File Sizes
- **graph.json:** ~112 KB ✓ (under 5 MB limit)
- **GRAPH_REPORT.md:** Available ✓
- **graph.html:** Available ✓

## Analysis Quality
- **Extraction:** 95% EXTRACTED · 5% INFERRED · 0% AMBIGUOUS
- **Inferred Edges:** 9 edges (avg confidence: 0.67)
- **Token Cost:** 0 input · 0 output

## Graph Freshness
- **Built from commit:** `fe947b67`
- **Check freshness:** Run `git rev-parse HEAD` and compare to `fe947b67`
- **Update graph:** Run `graphify update .` after code changes (no API cost)

## Top Connections (God Nodes)
1. Refacer - 16 edges
2. SCRFD - 11 edges
3. ArcFaceONNX - 10 edges
4. app.py - 4 edges
5. docker/run.sh - 4 edges

## Key Components
- Computer vision library for face recognition
- SCRFD (face detection)
- ArcFace (face recognition)
- Recognition pipeline and Docker integration

## Local Source
- **Working Directory:** `graphify-out/` (local working output, not committed)
- **Note:** `graphify-out/` contains build artifacts (cache, backups) and should NOT be committed directly. Only curated files (GRAPH_REPORT.md and graph.json) are saved to `docs/graphify/`.

## Usage
- Review `GRAPH_REPORT.md` for detailed analysis and community navigation
- View `graph.json` for full graph data structure
- Open `graph.html` locally for interactive graph visualization
