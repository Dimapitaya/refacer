# Graph Report - C:\AI_AGENT_WORKSPACE\repos\refacer  (2026-06-16)

## Corpus Check
- cluster-only mode — file stats not available

## Summary
- 165 nodes · 195 edges · 11 communities (10 shown, 1 thin omitted)
- Extraction: 95% EXTRACTED · 5% INFERRED · 0% AMBIGUOUS · INFERRED: 9 edges (avg confidence: 0.67)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `fe947b67`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- [[_COMMUNITY_Community 0|Community 0]]
- [[_COMMUNITY_Community 1|Community 1]]
- [[_COMMUNITY_Community 2|Community 2]]
- [[_COMMUNITY_Community 3|Community 3]]
- [[_COMMUNITY_Community 4|Community 4]]
- [[_COMMUNITY_Community 5|Community 5]]
- [[_COMMUNITY_Community 6|Community 6]]
- [[_COMMUNITY_Community 7|Community 7]]
- [[_COMMUNITY_Community 8|Community 8]]
- [[_COMMUNITY_Community 9|Community 9]]
- [[_COMMUNITY_Community 10|Community 10]]

## God Nodes (most connected - your core abstractions)
1. `Refacer` - 16 edges
2. `SCRFD` - 11 edges
3. `ArcFaceONNX` - 10 edges
4. `app.py` - 4 edges
5. `docker/run.sh` - 4 edges
6. `recognition/arcface_onnx.py` - 4 edges
7. `recognition/face_align.py` - 4 edges
8. `recognition/main.py` - 4 edges
9. `recognition/scrfd.py` - 4 edges
10. `refacer.py` - 4 edges

## Surprising Connections (you probably didn't know these)
- `RefacerMode` --uses--> `ArcFaceONNX`  [INFERRED]
  refacer.py → recognition/arcface_onnx.py
- `RefacerMode` --uses--> `SCRFD`  [INFERRED]
  refacer.py → recognition/scrfd.py
- `Namespace` --uses--> `SCRFD`  [INFERRED]
  recognition/main.py → recognition/scrfd.py
- `Namespace` --uses--> `ArcFaceONNX`  [INFERRED]
  recognition/main.py → recognition/arcface_onnx.py

## Import Cycles
- None detected.

## Communities (11 total, 1 thin omitted)

### Community 0 - "Community 0"
Cohesion: 0.07
Nodes (28): app.py, ast_hash, mtime, semantic_hash, docker/run.sh, ast_hash, mtime, semantic_hash (+20 more)

### Community 1 - "Community 1"
Cohesion: 0.07
Nodes (28): app.py, ast_hash, mtime, semantic_hash, docker/run.sh, ast_hash, mtime, semantic_hash (+20 more)

### Community 2 - "Community 2"
Cohesion: 0.15
Nodes (3): Enum, Refacer, RefacerMode

### Community 3 - "Community 3"
Cohesion: 0.10
Nodes (17): Open In Colab, demonstration, Disclaimer, How to Install FFmpeg, Insightface, Insightface example, Installation, ONNX Runtime repository (+9 more)

### Community 4 - "Community 4"
Cohesion: 0.13
Nodes (15): ArcFaceONNX, CoreML Requirements, CPU Requirements, FFmpeg, Insightface, inswapper_128.onnx, Namespace, Recognition Module (+7 more)

### Community 5 - "Community 5"
Cohesion: 0.26
Nodes (4): distance2bbox(), distance2kps(), Decode distance prediction to bounding box.      Args:         points (Tensor, SCRFD

### Community 6 - "Community 6"
Cohesion: 0.18
Nodes (3): Namespace, ArcFaceONNX, parse_args()

### Community 7 - "Community 7"
Cohesion: 0.36
Nodes (5): estimate_norm(), norm_crop(), trans_points(), trans_points2d(), trans_points3d()

### Community 8 - "Community 8"
Cohesion: 0.50
Nodes (4): refacer.py, ast_hash, mtime, semantic_hash

### Community 9 - "Community 9"
Cohesion: 0.50
Nodes (4): recognition/face_align.py, ast_hash, mtime, semantic_hash

## Knowledge Gaps
- **70 isolated node(s):** `run.sh script`, `mtime`, `ast_hash`, `semantic_hash`, `mtime` (+65 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **1 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `SCRFD` connect `Community 5` to `Community 2`, `Community 6`?**
  _High betweenness centrality (0.037) - this node is a cross-community bridge._
- **Why does `ArcFaceONNX` connect `Community 6` to `Community 2`?**
  _High betweenness centrality (0.025) - this node is a cross-community bridge._
- **Are the 3 inferred relationships involving `SCRFD` (e.g. with `Namespace` and `.__init_apps()`) actually correct?**
  _`SCRFD` has 3 INFERRED edges - model-reasoned connections that need verification._
- **Are the 3 inferred relationships involving `ArcFaceONNX` (e.g. with `Namespace` and `.__init_apps()`) actually correct?**
  _`ArcFaceONNX` has 3 INFERRED edges - model-reasoned connections that need verification._
- **What connects `run.sh script`, `mtime`, `ast_hash` to the rest of the system?**
  _70 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Community 0` be split into smaller, more focused modules?**
  _Cohesion score 0.06896551724137931 - nodes in this community are weakly interconnected._
- **Should `Community 1` be split into smaller, more focused modules?**
  _Cohesion score 0.06896551724137931 - nodes in this community are weakly interconnected._