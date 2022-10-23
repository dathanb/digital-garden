# Dathan's digital garden

Based on [Quartz](https://quartz.jzhao.xyz/)

Content goes on the `master` branch in the `content/` directory.

When that branch gets pushed, a github action runs to export the markdown in the `content/` directory as HTML using the Hugo theme, and commits to the `publish` branch.

Then the GitHub Pages deploy action picks up on the commit to the `publish` branch and publshes to `https://dathanb.github.io/digital-garden`
