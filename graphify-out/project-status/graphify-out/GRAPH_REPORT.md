# Graph Report - project-status  (2026-10-16)

## Corpus Check
- cluster-only mode — file stats not available

## Summary
- 24 nodes · 26 edges · 5 communities (3 shown, 2 thin omitted)
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Community 0
- Community 1
- Community 2
- Community 3
- Community 4

## God Nodes (most connected - your core abstractions)
1. `0.3.0 REQUIRED ROWS` - 9 edges
2. `DELIVERED FEATURES` - 8 edges
3. `OVERTONE · PROJECT STATUS · 2026-10-16` - 4 edges
4. `LONGER-TERM · OUTSIDE 0.3.0` - 4 edges
5. `[DONE] Map check · structure · export` - 2 edges
6. `[PARTIAL] Hitsounds H1–H5 shipped` - 2 edges
7. `[SHIPPED] Songs library + health check` - 2 edges
8. `[OPEN · BLOCKER] R6 library precision sample` - 2 edges
9. `[CLOSED BY MEASUREMENT] T6 section labels from repetition` - 2 edges
10. `[CLOSED BY MEASUREMENT] T7 H6/H7 disposition` - 2 edges

## Surprising Connections (you probably didn't know these)
- `OVERTONE · PROJECT STATUS · 2026-10-16` --tracks--> `0.3.0 REQUIRED ROWS`  [EXTRACTED]
  README.md → docs/07-roadmap.md
- `OVERTONE · PROJECT STATUS · 2026-10-16` --tracks--> `LONGER-TERM · OUTSIDE 0.3.0`  [EXTRACTED]
  README.md → docs/07-roadmap.md
- `OVERTONE · PROJECT STATUS · 2026-10-16` --constrained by--> `[POLICY] No networked services`  [EXTRACTED]
  README.md → AGENTS.md

## Communities (5 total, 2 thin omitted)

### Community 0 - "Community 0"
Cohesion: 0.29
Nodes (7): [RESEARCH] Phase 10 real-audio accuracy → 1.0.0, LONGER-TERM · OUTSIDE 0.3.0, [DEFERRED] Phase 25 tempo-matched junction, [UNDECIDED] Export convention vs sound onset, [DEFERRED] Phase 24 other-language gates, [POLICY] No networked services, OVERTONE · PROJECT STATUS · 2026-10-16

### Community 1 - "Community 1"
Cohesion: 0.29
Nodes (7): [PARTIAL] Compile section + map builder, [PARTIAL] Hitsounds H1–H5 shipped, [SHIPPED] MSI + portable ZIP, DELIVERED FEATURES, [CLOSED BY MEASUREMENT] T7 H6/H7 disposition, [DONE] Timing · Python v3 + Rust v4, [DONE] Train section and trainer gate

### Community 2 - "Community 2"
Cohesion: 0.33
Nodes (6): 0.3.0 REQUIRED ROWS, [DONE] T1 Train browser harness EN/ES, [DROPPED] T2 signing, [DONE] T3 trainer nicer rows, [DONE] T4 trainer open questions, [DONE] T5 installer associations/setup

## Knowledge Gaps
- **13 isolated node(s):** `[DONE] Timing · Python v3 + Rust v4`, `[DONE] Train section and trainer gate`, `[PARTIAL] Compile section + map builder`, `[SHIPPED] MSI + portable ZIP`, `[DONE] T1 Train browser harness EN/ES` (+8 more)
  These have ≤1 connection - possible missing edges. (Counts symbols only; 13 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **2 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `0.3.0 REQUIRED ROWS` connect `Community 2` to `Community 1`, `Community 3`, `Community 4`?**
  _High betweenness centrality (0.016) - this node is a cross-community bridge._
- **What connects `[DONE] Timing · Python v3 + Rust v4`, `[DONE] Train section and trainer gate`, `[PARTIAL] Compile section + map builder` to the rest of the system?**
  _13 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Why does `DELIVERED FEATURES` connect `Community 1` to `Community 3`, `Community 4`?**
  _High betweenness centrality (0.014) - this node is a cross-community bridge._