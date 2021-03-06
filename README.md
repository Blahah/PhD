## PhD thesis

This is my PhD thesis. It's a work in progress.

You can see the HTML version of something like the current state here: http://rik.smith-unna.com/phd/thesis.html

Working title:

**A phylotranscriptomic reasoning framework for C4 photosynthesis research.**

Expected structure:

1. Introduction
2. Measuring transcriptome assemblies
3. In pursuit of the optimal transcriptome assembly
4. Building high-quality transcriptomic resources for C4 research
5. Reasoning about C4 with a phylogenetically structured model
6. [if time] Updating our beliefs about C4 with old and new data

Note: It may not compile cleanly while it's a WIP. I'll make releases as each chapter is done/drafted.

## Contributing

I'm putting work here *as I write it*. People often seem afraid to do this, but I make mistaked like everyone else (edit: see!), and I'm happy with that.

If you feel like reading the work, I'd love to hear what you think. Comments, questions, suggestions, and pointing out mistakes, stupidity or anything else, are all welcome! Please create an issue. Or email me (rds45<at>cam.ac.uk) if you'd prefer to talk in private (though I'm happy to be called out in public).

## Installing pre-requisites

You'll need:

- `pandoc`
- `pandoc-fignos`
- `pandoc-eqnos`
- a LaTeX distribution

e.g. on OSX:

First install MacTeX from: https://www.tug.org/mactex/

Then with homebrew:

```bash
brew install pandoc
pip install pandoc-fignos pandoc-eqnos
```

## Making the thesis

```bash
make html
# OR
make pdf
# OR
make # for both PDF and HTML
```

## Building figures from scratch

```bash
make figureimg
```

### Pre-requisites

- [`mermaid`](https://github.com/knsv/mermaid) for flow-charts
- `node.js` for mermaid
- `mmv`

e.g. on OSX:

```bash
# install node.js
wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.29.0/install.sh | bash
nvm install 5.0.0
# install mermaid
npm install --global mermaid phantomjs
# install mmv
brew install mmv
```
