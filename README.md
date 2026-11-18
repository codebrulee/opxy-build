# Codebrulee's Open-XY build

The GitHub Pages site for a personal [Open-XY](https://github.com/etcetc000/open-xy)
build: `index.html` (what it is, what's different, credits) and
`opxy-builder.html` (the browser builder, from `sdk.py kit --personal`).

Not an official Open-XY release. No Teenage Engineering firmware is hosted
here; the builder patches the user's own stock OS 1.2.1 `os.ldr` in the browser.

## Rebuilding

1. In the Open-XY source checkout (`codebrulee/open-xy`, branch named in
   `index.html`), run:

       python sdk.py kit --personal --stock-os <stock os.ldr> --out <dir> \
         --collection kit-collection.json --extension <folder> ...

2. Copy `<dir>/opxy-builder.html` here and update the build line in
   `index.html`'s footer.
