# CLAUDE.md — archive-series

**Organization rules (mandatory): https://github.com/nlink-jp/.github/blob/main/CONVENTIONS.md**

## What this repository is

The umbrella for archived projects. Every submodule is **read-only on GitHub**.

## Non-negotiable rules

- **Do not open work against anything in here.** These repositories reject
  pushes. A change you write cannot be committed, released, or shared — you
  will do the work and then discover it has nowhere to go.
- **Do not apply org-wide sweeps here.** Platform matrices, test harnesses,
  README mirroring, dependency bumps: none of it reaches an archived project.
  Sweeps run over the active series umbrellas only.
- **A defect found here is knowledge, not a task.** Write it to
  `nlink-jp/knowledge` if it generalises; otherwise let it rest.
- **Do not un-archive to "just fix one thing".** Un-archiving is the owner's
  decision, and it is rarely worth it for a project that has a successor.

## Structure

```
archive-series/
├── cybersecurity/   projects archived out of cybersecurity-series
├── lab/             projects archived out of lab-series
├── lite/            projects archived out of lite-series
└── util/            projects archived out of util-series
```

The directory a project sits in records the series it belonged to. That is the
whole point of the layout: "is this archived?" and "what was it?" are both
answered by the filesystem, without a network call or a marker in a list.
