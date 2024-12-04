# Anim Chess Project <!-- omit from toc -->

<div style="font-size: 1.25rem;">
<b>anim</b> <i>(n., adj.)</i>: six (6) — in Filipino/Tagalog
</div>

Anim Chess is a platform dedicated to playing Gliński's hexagonal chess variant[^1] — initially a personal project to play hexagonal chess with friends.

Features include but not limited to[^2]:
- Match-making and real time games
- Real time chat between players
- ...and many more in the pipeline. :smile:

**Contents:**
- [Project Structure](#project-structure)
  - [`apps` directory](#apps-directory)
  - [`packages` directory](#packages-directory)
  - [`tooling` directory](#tooling-directory)
- [Contributing](#contributing)
- [Inspirations](#inspirations)

# Project Structure
This project is a [monorepo](https://en.wikipedia.org/wiki/Monorepo) managed using [turborepo](https://turbo.build/repo/docs) and [pnpm](https://pnpm.io/motivation).

This section will briefly describe the project structure.

## `apps` directory
`apps/web` — The frontend for the Anim Chess Project made with AstroJS and SolidJS components. *(TBD. backend approach)*

`apps/ws` — The main websocket server made with Rust and Socket-io.

`apps/docs` — The documentation for published npm packages.

## `packages` directory
`packages/board` — The web component responsible for rendering the hexagonal chess board. Made with Lit web components.

`pacakges/field` — The package used for features such as movement generation and validation, piece placement and movement, and stalemate/check/checkmate detection.

## `tooling` directory
Contains files related to tooling used throughout the monorepo.

# Contributing
Please read the [guidelines for contributing.](https://github.com/lborres/animchess/blob/main/CONTRIBUTING.md)

# Inspirations
The animchess project was inspired by CGP Grey in their video: [Can Chess, with Hexagons?](https://youtu.be/bgR3yESAEVE?si=_PwDI9BSLCuoVSzj)

---

> [!NOTE]
> This is my first open source project. While I do my best to learn about best practices in open source project, I expect I would have made some mistakes or missed some things.
> Please create a thread in the discussions section.
> If you would rather reach out to me privately, you may send me an email: [lborresbusiness@gmail.com](mailto:lborresbusiness@gmail.com)

[^1]: [Gliński's hexagonal chess - Wikipedia](https://en.wikipedia.org/wiki/Hexagonal_chess#Gli%C5%84ski's_hexagonal_chess)
[^2]: As of 2024-12-04, these are just project goals and have yet to be realized.
