# vest-docs

GitHub Pages host for [Vest](https://github.com/y1ca1/vest) rustdoc documentation.

## Usage

1. Generate the documentation locally with `cargo doc`:
   ```sh
   cargo doc --no-deps
   ```
2. Copy the generated `target/doc/` folder into the root of this repository as `doc/`:
   ```sh
   cp -r target/doc/ /path/to/vest-docs/doc/
   ```
3. Commit and push to `main`:
   ```sh
   cd /path/to/vest-docs
   git add doc/
   git commit -m "Update docs"
   git push
   ```

The [Deploy Docs to GitHub Pages](.github/workflows/deploy-docs.yml) workflow will automatically publish the contents of the `doc/` folder to the GitHub Pages site.
