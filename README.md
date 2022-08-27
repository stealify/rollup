# rollup
A Collection of Rollup dependent tooling - Mainly used to build awsome stuff.

## Contains
- rollupRequire and rollupRequireSync (A require implementation using rollup to load code)
  - Electron ESM - loaderSync executes rollup fully sync and blocks your current process until everything is loaded.
    - Allows you to @stealify/rollup/loader loader
- rollupImport and rollupImportSync (a dynamic import Implementation based on rollup);
  - Mainly used in development or highly dynamic environments or as ts loader it is usefull at last for me
  
## Why? 
I do not want to write so much rollup.config.js files and keep them in sync so i add simply the rollup instructions into my main js
my main js is then able to load dynamic on runtime. Should i need to bundle that it is not a problem simply reuse the same configuration.
