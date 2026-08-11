# Contributing to the organization profile

This repository controls the public profile shown at
[github.com/odysseia-greek](https://github.com/odysseia-greek). Keep it concise,
welcoming, and accurate for readers who may not know the project yet.

## Profile changes

- Edit `profile/README.md` for copy, links, and layout.
- Prefer links to a repository over duplicating repository-specific setup steps.
- Check every new relative link from the `profile` directory.
- Keep the mascot at `profile/images/mascot.png` so profile markup stays stable.

## Diagrams

Diagram sources and generated assets live in `profile/diagrams`. Install
[D2](https://d2lang.com/tour/install), edit the relevant `.d2` file, and render
its matching SVG:

```sh
d2 --layout=dagre --theme=200 \
  profile/diagrams/architecture.d2 \
  profile/diagrams/architecture.svg
```

Repeat for every edited diagram. Commit the source and SVG together, and make
sure the profile README references the SVG rather than a tool-specific source.

## Pull requests

Explain what became clearer or more accurate and how you checked it. Screenshots
are useful for substantial visual changes to the organization profile.
