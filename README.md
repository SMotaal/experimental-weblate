# Experimental Weblate

> **Important Note**: This is not meant for use yet.

Experimental deployment of the Weblate backend.

## Getting Started

This repository uses a locally hosted Weblate container intended to be used on environments that support `docker` and `npm`.

> **Important Note**: Non-linux-compatible environments will often run into interoperability problems. If you are on Windows, please make sure you are using the [Windows Linux Subsystem (WSL)](https://docs.microsoft.com/en-us/windows/wsl/faq).

### Cloning `sources/WeblateOrg/docker-compose`

This code is cloned directly from the [WeblateOrg/docker-compose][] into `sources/WeblateOrg/docker-compose`.

> After `cloning` the repo, run **`npm run test:WeblateOrg/docker-compose`** locally

You can use `npm run pull:WeblateOrg/docker-compose` which will pull the latest version of the codebase using `subtree` as follows:

1. Local configure the `WeblateOrg/docker-compose` remote pointing to `https://github.com/WeblateOrg/docker-compose.git` if necessary.
2. Stash local changes.
3. Perform `git subtree pull --squash` or `add`.
4. Pop stashed changes back.

> **Note**: Using subtree makes it easier to retain external sources directly when commiting and pushing code. This is more straightforward than `submodules` when upstreaming is not necessary.

### Testing `sources/WeblateOrg/docker-compose`

You can use `npm run test:WeblateOrg/docker-compose` which will simply `cd` into `sources/WeblateOrg/docker-compose` and run `./test.sh`.

> **Note**: Make sure you have `docker-compose` setup on your local environment.

### Configuring `sources/WeblateOrg/docker-compose`

Refer to https://docs.weblate.org/en/latest/admin/install/docker.html.

[weblateorg/docker-compose]: https://github.com/WeblateOrg/docker-compose
