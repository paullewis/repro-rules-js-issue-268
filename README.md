# Repro for rules_js issue 268

This is a repro for https://github.com/aspect-build/rules_js/issues/268

## Running

1. `bazel clean`
1. `bazel build //src`

Note: the `package.json` has `resolutions` to a local path, which is
what causes the failure.
