# Prashray Nagar Portfolio

Jekyll source for [nagarprashray.github.io](https://nagarprashray.github.io), focused on ASIC/FPGA design and verification work.

## Local development with Docker

The project is locked to the GitHub Pages Jekyll dependency set. From the
repository root, install/update the cached gems and build the production site:

```powershell
docker run --rm -v "${PWD}:/srv/jekyll" -w /srv/jekyll ruby:3.3 bash -lc "bundle config set --local path vendor/bundle && bundle install && bundle exec jekyll build"
```

Run the local development server:

```powershell
docker run --rm -v "${PWD}:/srv/jekyll" -w /srv/jekyll -p 4000:4000 ruby:3.3 bash -lc "bundle config set --local path vendor/bundle && bundle exec jekyll serve --host 0.0.0.0"
```

Then open `http://localhost:4000`. The generated `_site`, Bundler configuration,
and installed gem cache are intentionally ignored by Git.

GitHub Pages can build the site directly from the repository's default branch.
