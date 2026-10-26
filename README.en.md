# Technology Fishing LP

[日本語](README.md) | [English](README.en.md)

A planning and production repository for a scroll-based experience introducing Technology Fishing, kept separate from the game itself.

## Concept

Follow a single fishing line hanging from the surface and scroll down underwater. Wind patterns on the surface turn into ocean currents; as the light fades, hints of fish gradually become visible. Show the character of each technology through the fish’s movement, then guide visitors to the actual game.

## Decisions so far

- Build it as a separate work and repository from the game.
- Keep the landing page a static site with no database, game API, or WebSocket.
- Astro + TypeScript are candidates. Use static HTML for most content, and load underwater 3D independently only if needed.
- Keep normal scrolling behavior. Support `prefers-reduced-motion`, and make sure the content and game link still work without 3D.
- Begin full production after the hackathon. At this stage, keep the repository to the concept and minimal skeleton.

The fish in Technology Fishing are representations for communicating technical concepts; this is not a simulator that reproduces how each technology works internally.

## Experience flow

Introduce the work and a “Start the game” link at the surface → follow the line below the water → reveal fish gradually from their presence and shadows → briefly explain the connection between each fish’s behavior and a technology → guide visitors to the full game.

The initial concept includes the Go Fish, Docker Whale, and CSS Fish. K8s Leviathan is experimental, so whether it belongs in the main introduction is a separate decision.

## Documentation

- [Experience brief](docs/experience-brief.md): purpose, UX, technical direction, open decisions, and production order

## Development status

This repository is currently in the planning stage. The Astro app template, dependencies, hosting, and destination link to the game have not been configured yet. After the hackathon, review the brief first, then create the skeleton and a short prototype.
