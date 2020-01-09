# dvc.api.summon()

Instantiate an object, described in a _summon file_.

## Signature

```py
def summon(
  name,
  repo=None,
  rev=None,
  summon_file="dvcsummon.yaml",
  args=None
)
```

## Parameters

- `name` - object to summon

- `repo` - path or Git URL of a DVC repository

- `rev` - (optional)
  [Git revision](https://git-scm.com/book/en/v2/Git-Internals-Git-References)
  (such as a branch name, a tag, or a commit hash). This only works with `repo`
  URLs.

- `summon_file` - YAML file describing the object in question. Defaults to
  `dvcsummon.yaml`.

- `args` - arguments to pass onto the object, if any