# rocker-compose

Composition tool for running multiple containers on a host.

TODO: usage manual

### Dependencies

Use [gb](http://getgb.io/) to test and build.

### Fetch dependencies

```bash
gb vendor update -all
```

### Build

```bash
gb build
```

### Test 

```bash
gb test
```

### Test something particular

```bash
gb test -run TestMyFunction
```

### TODO

[ ] Should remove obsolete containers (e.g. removed from compose.yml)
[ ] EnsureContainer for containers out of namespace (cannot be created)
[ ] Introduce templating for compose.yml to substitute variables from the outside
[ ] client.go execution functions
[ ] Refactor config.go - move some functions to config_convert.go
[ ] Add labels for containers launched by compose?
[ ] rocker-compose executable with docker connection and cli flags
[ ] ansible-module mode for rocker-compose executable
[ ] Choose and adpot logging framework
[ ] Attach stdout of launched (or existing) containers
[ ] Force-restart option
[ ] Never remove volumes of some containers
[ ] Parallel pull operation
[ ] Force-pull option (if image is existing, only for "latest" or non-semver tags?)
[ ] Clean command, keep_versions config attribute for containers
[ ] Dry mode
[ ] Cross-compilation for linux and darwin (run in container? how gb will work?)

