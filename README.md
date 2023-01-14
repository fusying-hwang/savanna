# Build file generation with Gazelle

1. Add dependencies in `requirements.in`
2. Generate lock file `requirements_lock.txt`
   ```
   $ bazel run //:requirements.update
   ```
3. Generate `gazelle_python.yaml`.
   ```sh
   $ bazel run //:gazelle_python_manifest.update
   ```
4. Generate `BUILD.bazel`.
   ```sh
   $ bazel run //:gazelle
   ```