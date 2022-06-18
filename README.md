# TypeScriptToLua Neovim Plugin Template

This template project uses [TypeScriptToLua](https://typescripttolua.github.io/)
to create a neovim lua plugin.

## Notice for TypeScriptToLua

There are many differences between Typescript for JavaScript and TypeScriptToLua
for Lua:

1. Features from languages(JavaScript and Lua): [Caveats | TypeScriptToLua](https://typescripttolua.github.io/docs/caveats)
1. To support JavaScript's function behavior in Lua: [The Self Parameter | TypeScriptToLua](https://typescripttolua.github.io/docs/the-self-parameter)
1. Using other modules: you can use external Lua code but not TypeScript files
from npm packages. [External Lua Code | TypeScriptToLua](https://typescripttolua.github.io/docs/external-lua-code)
1. Publish TSToLua modules: with the previous item, the good news is you can use
TypeScriptToLua to publish this Lua module with **types** and can be used in
other TSToLua projects.
[Publishing Modules | TypeScriptToLua](https://typescripttolua.github.io/docs/publishing-modules)
1. Extend TypeScript to support features in Lua: [Language Extensions | TypeScriptToLua](https://typescripttolua.github.io/docs/advanced/language-extensions)

## How to use this template

First change the project name and related path.

1. In `package.json`:
  * Update meta data `name`, `repository.url`, `author`, etc.
  * Update project name path in `main`, `types`
1. In `tsconfig.json`:
  * Update project name path in `compilerOptions.outDir`

This project favors `yarn` and use `yarn` to install dependencies, use
`yarn build` to generate lua code. The output files will be in `./lua/<project name>/`.

Finally, use `yarn dev` to build in realtime
as source files change.

## TODO

* [ ] Examples to use GitHub CI to automatically build code on git push.
* [ ] Provide Neovim API type declarations (how to automatically generate them?)
as a npm package.
