# testing-codebases

Unison codebases that tests and benchmarks in [unisonweb/unison](https://github.com/unisonweb/unison)
run against, too large to keep in that repository. Each is a release here, with the codebase
as a `.tar.gz` asset that unpacks to `.unison/v2/unison.sqlite3`, the layout `ucm -C <dir>`
expects. `scripts/testing-codebase.sh` in the main repository downloads one by name, checks
its SHA-256, and caches it in a directory named by that hash.

| Release | Contents |
| --- | --- |
| `jit-2026-10-19` | project `jit-tests`, branch `main`: the `@pchiusano/misc-benchmarks` suite and the libraries base 7.19.2, json 1.3.4, cloud 20.15.1 and benchmark 2.0.0; what the JIT's benchmark transcripts run in |
