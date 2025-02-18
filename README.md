Example usage

```yml
name: Build and Deploy for Github Pages
on:
  workflow_dispatch:
  push:
    paths:
      - "src/**"
      - "public/**"
      - ".github/workflows/**"
      - "package.json"
      - "vite.config.ts"
      - "astro.config.mjs"
      - "yarn.lock"
    branches:
      - main

jobs:
  build-deploy:
    uses: hrgui/my-personal-gh-workflows/.github/workflows/bun_gh_pages.yml@main
```
