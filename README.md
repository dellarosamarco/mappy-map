# mappy-map

Generated H3 geography artifacts for Mappy, built by
`tool/boundaries/build_h3_geography_release.py` from the main repository.

```
h3-geography/<overture-release>/<CC>.mh3      schema-v8 binary country pack
h3-geography/<overture-release>/<CC>.mh3.br   the same, brotli-10, ready to upload as-is
h3-geography/<overture-release>/h3-geography-size-report.json
h3-geography/<overture-release>/build-timing.csv   per-country wall clock and worker time
h3-geography/<overture-release>/build.log          the builder's own log
```

Artifacts are pushed as they are produced, so a partial build is a valid
partial set. `build-timing.csv` records, for every country: divisions,
seconds of worker time actually spent on it, elapsed seconds (which includes
waiting behind other countries in the shared pool), artifact sizes, and the
wall-clock time since the build started at which it finished.
