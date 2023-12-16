# Ren'py, un moteur libre et multiplateforme pour créer des jeux

Discovery of Ren'Py in french initially prepared for `Capitole du Libre` 2023.

## Run the presentation

Use Asciidoctor reveal.js (or `Asciidoc Slides` in VS Code) to generate a presentation from `presentation.adoc`, then get started.

## Build the presentation

### Prepare to build

Building the presentation requires [Ruby](https://www.ruby-lang.org/en/) with `bundle`. To install `bundle`, run the following command after installing ruby:

```sh
gem install bundle
```

Once bundle is installed, install the project dependencies by running the following commands from the project's directory:

```sh
bundle config --local path .bundle/gems
bundle
```

### Build the presentation

Run the following command from a shell to generate the file `presentation.html`

```sh
bundle exec asciidoctor-revealjs \
  -r asciidoctor-kroki \
  -a revealjsdir=https://cdn.jsdelivr.net/npm/reveal.js@5.0.2 \
  presentation.adoc
```
