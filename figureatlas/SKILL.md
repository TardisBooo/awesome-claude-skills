---
name: figureatlas
description: Pick one of 300 verified figure types for a paper, slide, poster, or video frame, then export HTML or SVG.
---

# FigureAtlas

FigureAtlas is a figure catalog for papers, slides, posters, and video frames. The source catalog has 300 verified types across 15 families. This page points at that catalog instead of copying it.

Repository: https://github.com/TardisBooo/figureatlas

## When to Use This Skill

- A paper panel needs one chart, diagram, map, or illustration.
- The same figure must fit a journal column, a 16:9 slide, a 4:3 slide, a poster, or a 1080p video frame.
- An agent should pick an existing figure id instead of inventing a new chart type.

## What This Skill Does

1. **Pick a frame**: journal single column, journal double column, 16:9 slide, 4:3 slide, A0 poster, or 1080p video.
2. **Pick one id**: read `CATALOG.md` and choose one of the 300 verified types.
3. **Export**: call `render_figure(id)` and write HTML or SVG.

## How to Use

### Basic Usage

```text
Pick a FigureAtlas figure for a single-column volcano plot and export SVG.
```

### Advanced Usage

```text
Use FigureAtlas id 161 for a volcano plot, fit it to a 16:9 slide, and export HTML.
```

## Example

**User**: "I need a forest plot for a journal column."

**Output**:

The agent selects the forest-plot id from `CATALOG.md` and exports HTML or SVG for a single column. It does not invent a 301st type.

**Credit:** TardisBooo, https://github.com/TardisBooo/figureatlas

## Tips

- Keep the figure id inside the published catalog.
- Use the bilingual homepage when you need a Chinese or English title.
- Open the screenshot in `assets/gallery/atlas/` before exporting a new frame.

## Common Use Cases

- Journal figures
- Slide figures
- Poster and video frames
