# Release procedure

-   Make sure CHANGELOG.md is up to date
-   `npm version {major|minor|patch}`
-   Push the commit to `main` through a merged PR
-   GitHub Actions will automatically create tag `v<package.json version>` if it does not exist
-   GitHub Actions will publish `@piaggiofastforward/rlayers` to GitHub Packages after tagging
-   If needed, publish manually with `NODE_AUTH_TOKEN=<github_pat_with_write_packages> npm publish`
