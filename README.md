# What is this repo?

This repo contains utilities meant to be vendored in other places.

In this repo, **only relative imports** to other modules are allowed.

Also, it should work without any external deps (so, if external libraries
are required, a fallback should be provided if it's not found).

# Places where it's used:

# robocorp repo:

So, at the `robo` root it was added as:

```
git subtree add --prefix action_server/src/robocorp/action_server/vendored_deps git@github.com:robocorp/vendored_deps.git master --squash
```

And it can be updated (again, at the `robo` root) with:

```
git subtree pull --prefix action_server/src/robocorp/action_server/vendored_deps git@github.com:robocorp/vendored_deps.git master --squash
```

# robotframework-lsp repo:

So, at the `robotframework-lsp` root it was added as:

```
git subtree add --prefix robocorp-code/src/robocorp_code/vendored_deps git@github.com:robocorp/vendored_deps.git master --squash
```

And it can be updated (again, at the `robotframework-lsp` root) with:

```
git subtree pull --prefix robocorp-code/src/robocorp_code/vendored_deps git@github.com:robocorp/vendored_deps.git master --squash
```

