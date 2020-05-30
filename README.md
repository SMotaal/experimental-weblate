# Experimental Weblate

Experimental deployment of the Weblate backend.

## Getting Started

### Sources

#### [WeblateOrg/docker-compose][]

This code is cloned directly from the [WeblateOrg/docker-compose][] into `sources/WeblateOrg/docker-compose`.

You can use `npm pull:WeblateOrg/docker-compose` which will pull the latest version of the codebase using `subtree` as follows:

1. Local configure the `WeblateOrg/docker-compose` remote pointing to `https://github.com/WeblateOrg/docker-compose.git` if necessary.
2. Stash local changes.
3. Perform `git subtree pull --squash` or `add`.
4. Pop stashed changes back.

> **Note**: Using subtree makes it easier to retain external sources directly when commiting and pushing code. This is more straightforward than `submodules` when upstreaming is not necessary.

[weblateorg/docker-compose]: https://github.com/WeblateOrg/docker-compose
