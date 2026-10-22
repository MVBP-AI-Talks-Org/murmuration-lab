# Erdős Distance Lab — AI-Talks.org

An interactive HTML5 Canvas sandbox for the **Erdős planar unit-distance problem**, developed as a companion to the AI-Talks.org essay *The New Act of Creation: AI, Creativity, and the Future of Science*.

## Open the lab

**GitHub Pages:** https://mvbp-ai-talks-org.github.io/murmuration-lab/erdos-distance-lab/

**Source:** [index.html](./index.html). No build, external libraries, or backend required. The existing Murmuration Lab remains at the repository root.

## Controls

- Drag points. Double-click blank canvas space to add a point; Shift-click a point to remove it.
- Select square lattice, √2/√5/√10 rescaled square lattices, triangular lattice, regular polygon, or seeded random cloud.
- Change point count (9–196), visual matching tolerance, grid and edge overlays.
- Compare candidate configurations; try a *heuristic local search* (not mathematically certified optimization).
- Save a PNG snapshot.

## Mathematical caution

For exact Erdős unit distances, points `P_i` and `P_j` must satisfy `|P_i − P_j| = 1` **exactly**. The interface counts within a user-selected tolerance for practical dragging. Its comparisons are finite configurations and **do not reproduce or validate the 2026 AI-generated asymptotic counterexample**, which uses deeper algebraic number theory.

Research: [Alon et al. (2026)](https://arxiv.org/abs/2605.20695), [Sawin (2026)](https://arxiv.org/abs/2605.20579), [Erdős Problem 90](https://www.erdosproblems.com/90).

## WordPress integration

Simplest: Add a WordPress Button or paragraph link to the GitHub Pages URL above (recommended for mobile). A responsive `iframe` may be possible using a Custom HTML block if the site's WordPress plan and security filters permit it:

```html
<div style="position:relative;width:100%;height:780px;max-width:100%;">
  <iframe title="Erdős Distance Lab" src="https://mvbp-ai-talks-org.github.io/murmuration-lab/erdos-distance-lab/" loading="lazy" style="border:0;width:100%;height:100%;border-radius:12px;"></iframe>
</div>
```
