# keel plugin: Git

The Git panel, git actions for flows and git tools for agents. Agents read git; a person presses Commit and Push. keel's core keeps the git basics that flows need.

> **Status: planned.** The code still lives in [keel-v2](https://github.com/MiladNalbandi/keel-v2). It moves here step by step, as
> [the plugin plan](https://github.com/MiladNalbandi/keel-v2/tree/main/docs/plugins) says. There is nothing to install yet.

| | |
| --- | --- |
| id | `git` |
| needs | keel core (plugin SDK 1), Code |
| works with | — |
| parts | engine · api · web · content |
| trust level | runs code in keel |

**What it adds to keel**

- Code › Source control panel
- `git:*` actions for workflows
- `keel-git` tools for agents
- KeelBot commands /commit, /pr, /sync, /branch

**Where the code is today (keel-v2)**

- `engine/keel_engine/plugins/git`
- `keel.api.plugins.Git` (api)
- `web/src/components/plugins/GitPanel.tsx`
- `content/plugins/git`

## Layout

```
keel-plugin.yml   the manifest
engine/           Python package for keel's engine
api/              Kotlin, a thin Spring Boot jar
web/              React pages and slots (an ES module)
content/          workflows, agents, skills, commands
```

## Install

When it is released: in keel, **Control › Plugins › Marketplace › Git › Install**. keel checks the file's
signature, shows what the plugin may do, and asks you before it installs.

## License

MIT
