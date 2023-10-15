# Geoelements website

[![LICENSE](https://img.shields.io/badge/license-MIT-lightgrey.svg?style=flat-square)](https://raw.githubusercontent.com/geoelements/geoelements.github.io/main/LICENSE)

## Build and compile

```
bundle config set --local path './vendor/bundle'
bundle config build.eventmachine --with-ldflags="-Wl,-undefined,dynamic_lookup"
bundle install
bundle exec jekyll build
bundle exec jekyll serve --incremental
```
