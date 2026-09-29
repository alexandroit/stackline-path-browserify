# Upstream and compatibility

This independent fork starts from `path-browserify@1.0.1`, source commit
`872fec31a8bac7b9b43be0e54ef3037e0202c5fb` in
[browserify/path-browserify](https://github.com/browserify/path-browserify).
The native GitHub fork preserves the upstream history, branches and tags. Stackline work lives on `stackline`.

The original POSIX implementation and MIT license are unchanged. No runtime dependencies or Node engine declaration were added. Use an npm alias to preserve `require('path-browserify')` in existing applications.

## Issue review

Reviewed upstream open issues on 2026-09-29, including their reported use cases:

- [#35](https://github.com/browserify/path-browserify/issues/35) and [#26](https://github.com/browserify/path-browserify/issues/26): Windows path behavior is outside this POSIX implementation. Backslashes remain ordinary characters and `win32` remains null. Changing those semantics in this compatibility release would break existing browser callers. Contract tests cover the retained behavior.
- [#34](https://github.com/browserify/path-browserify/issues/34): relative `resolve()` needs a `process.cwd()` implementation in browser bundles. Supply the bundler process shim; this release does not invent a browser current working directory. A VM test checks the API with an explicit browser process shim.

The upstream test suite and the same API checks against an installed tarball run in CI. Issue review does not imply that every upstream issue is fixed.
