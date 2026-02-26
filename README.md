# vest-docs

GitHub Pages host for [Vest](https://github.com/y1ca1/vest) rustdoc documentation.

## Usage

1. From the [vest repository](https://github.com/y1ca1/vest) (`vest2.0` branch), run the provided `doc.sh` script to generate the `doc/` folder using `verusdoc`:
   ```sh
   ./doc.sh
   ```
2. Copy the generated `doc/` folder into the root of this repository:
   ```sh
   cp -r doc/ /path/to/vest-docs/doc/
   ```
3. Commit and push to `main`:
   ```sh
   cd /path/to/vest-docs
   git add doc/
   git commit -m "Update docs"
   git push
   ```

The [Deploy Docs to GitHub Pages](.github/workflows/deploy-docs.yml) workflow will automatically publish the contents of the `doc/` folder to the GitHub Pages site.
