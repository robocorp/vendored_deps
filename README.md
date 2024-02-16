# What is this repo?

This repo contains utilities meant to be vendored in other places.

In this repo, **only relative imports** to other modules are allowed.

Also, it should work without any external deps (so, if external libraries
are required, a fallback should be provided if it's not found).

# Places where it's used:

# robocorp repo:

At the `robo` root it was added at:

`action_server/src/robocorp/action_server/vendored_deps`

Update there with:

`pip install https://github.com/robocorp/vendored_deps/archive/master.zip --target .`


# robotframework-lsp repo:

At the `robotframework-lsp` root it was added as:

`robocorp-code/src/robocorp_code/vendored_deps`

Update there with:
`pip install https://github.com/robocorp/vendored_deps/archive/master.zip --target .`

