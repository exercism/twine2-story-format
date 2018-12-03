# Twine 2 story format

The story format is based on [snowman](https://github.com/klembot/snowman), and its only difference is that any text within code blocks aren't converted to links.

We have separate formats for development and production. In the development version, the Javascript is contained within the compiled HTML file, while in the production version, it is not. This is because we want to have control on when the Javascript loads on production, especially when we want to bind events to the walkthrough right after it is initialized. A consequence of this is that in order to update the story format on production, we need to copy over the generated JS into [exercism/website](https://github.com/exercism/website).
