# Phanes

A browser-side analytics toolkit for online forms & polls

![Phanes Logo](./logo.svg)

## Description

A web app for tracking impressions, drop-offs and user behaviour in surveys/forms — designed for online polls and internal research flows, with click/hover/scroll heatmaps and privacy-first client-side aggregation.

## Features

- Capture impression counts and abandonment points in multi-page online forms or internal poll flows.
- Map funnel progression: see how users move (or don’t) from page 1 to page n.
- Visualise heatmaps of user behaviour: where people click, where their cursor hovers, how far they scroll.
- Detect “friction points” in forms or surveys — e.g., which page/question causes the most drop-outs or negative behaviour.
- Enable experiments in form-design: for example, “fewer pages, same content” versus standard to see if completion improves.
- Adapt feedback loops by combining survey responses + heatmaps + funnel data to surface actionable UX insights.
- Privacy-first data aggregation: behavioural data is processed client-side in the browser, using techniques such as probabilistic data structures (like HLL / HyperMinHash) and optionally exploring fully homomorphic encryption (FHE) for - secure aggregation.
- Open-source friendly: easily deploy via GitHub, integrate into internal research workflows for polls and forms.
