# AGENTS.md — archive-series

## Project summary

Umbrella repository for nlink-jp's **archived** projects. Every submodule here
is read-only on GitHub: it accepts no commits, no releases, and no pull
requests. Projects are grouped by the series they belonged to before they were
archived, so `ls */` answers "what was this, and where did it live".

The catalog — one row per project — is [README.md](README.md); this file covers
only how to work with the umbrella (ADR-005).

## Key commands

| Command | Purpose |
|---------|---------|
| `git clone --recurse-submodules https://github.com/nlink-jp/archive-series.git` | Clone with all archived projects |
| `git submodule update --init` | Populate submodules in an existing clone |
| `git submodule add https://github.com/nlink-jp/<name>.git <series>/<name>` | Register a newly archived project |

`clone-all.sh` does not clone this umbrella by default — pass `--with-archive`.

## Gotchas

- **Nothing here is fixable.** A bug found in an archived project cannot be
  patched, released, or even committed. Record the finding elsewhere (the
  knowledge base) rather than opening work against a repository that will
  reject the push.
- **The build, test, and release rules of the series do not apply here.** Do
  not add `make test-linux`, bump platform matrices, or sync READMEs in these
  projects. They are frozen.
- Licences are not uniform across the submodules, and this umbrella licenses
  nothing — see the note at the top of README.md.
- Submodule checkouts default to detached HEAD. That is the correct state for
  an archived project; do not `git checkout main` to "fix" it.
- Submodule URLs are HTTPS only (SSH fails on machines without key auth).
- Every submodule needs a catalog row in README.md.

## Module path

Repository: `github.com/nlink-jp/archive-series`
