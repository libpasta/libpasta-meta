libpasta-meta
=============

This is a meta repository, designed to be used with [git-meta](https://github.com/twosigma/git-meta)
for managing the various libpasta language bindings.

Since the dependency tree looks roughly like:

```
libpasta <- libpasta-capi <- pasta-bindings <-- libpasta-java
                                            \
                                             \<-- libpasta-py
                                              \
                                               \<-- libpasta-rb
                                                \
                                                ...
```

Then making a small change (and bumping versions) requires updating 
all of these refs. The idea of a meta repository is similar to a mono-repo,
but hopefully with a bit more independence between modules.
