:construction: **Work In Progress** :construction:

Here we prototype a "concrete syntax tree" for OCaml, and the functionalities
that come with it: a parser, some iterators, a converter to the official
parstree, etc.

The aim is for this CST to be used in tools like ocamlformat and any other
project that might want to manipulate ocaml sources, e.g. merlin/lsp code
actions, some refactoring tools, etc.

Currently it is a raw import from
[tarides/neocamlformat](https://github.com/tarides/neocamlformat), so it is a
bit dated and lacking many of the functionnality mentionned above. However we
eventually expect for the CST parser to track the latest released version of
the OCaml parser while still being buildable/usable on older releases of OCaml,
for this reason we avoid depending on compiler-libs and instead "vendor" a
subset of it.
