# fips-argagg
This repo holds the fipsified [argagg](https://github.com/MODit3D/argagg), Argument Aggregator for parsing command line options in C++.

Using the fips build system: https://github.com/floooh/fips

## Using

To use argagg, add it to your `fips.yml`:

```cmake
imports:
     fips-argagg:
         git: https://github.com/MODit3D/fips-argagg.git
```

Because argagg is header only, you do not need a fips_deps(argagg) in CMakeLists.txt.
