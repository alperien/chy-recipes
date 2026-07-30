# chy-recipes

The default recipe repo for [chy](https://github.com/alperien/chy).

This repo is generated. The chytrans translator in alperien/chy converts
Void Linux xbps templates into chy recipes, and a daily sync job pushes
the result here. PRs that edit recipes get closed; fixes go in the
translator. Recipes whose meta says `origin: handwritten` are the
exception, preserved as-is by each sync.

Layout: one recipe per directory under recipes/. shlibs.map,
provided.suggested and TRANSLATOR_VERSION come from the same translate
run.

Use with chy:

    git clone https://github.com/alperien/chy-recipes
    ln -s "$PWD/chy-recipes/recipes" "$CHY_ROOT/recipes"
    cp chy-recipes/shlibs.map "$CHY_ROOT/shlibs.map"

MIT, like chy.
