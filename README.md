# Build file generation with Gazelle

1. Add dependencies in requirements.txt.
2. Generate `gazelle_python.yaml`.
   ```sh
   $ bazel run //:gazelle_python_manifest.update
   ```
3. Generate `BUILD.bazel`.
   ```sh
   $ bazel run //:gazelle
   ```