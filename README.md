# @osjwnpm/quibusdam-ab-consequatur

[![npm](https://img.shields.io/npm/v/@osjwnpm/quibusdam-ab-consequatur)](https://www.npmjs.com/package/@osjwnpm/quibusdam-ab-consequatur)

`@osjwnpm/quibusdam-ab-consequatur` is a node command line tool to generate directory structure tree.

## Installation

```bash
npm i @osjwnpm/quibusdam-ab-consequatur -g
```

## Usage

```bash
$ @osjwnpm/quibusdam-ab-consequatur -h
Usage: @osjwnpm/quibusdam-ab-consequatur [options]

Generate a directory structure tree

Options:
  -V, --version          output the version number
  -i, --ignore <ig>      ignore specific directory name, separated by comma or '|'  
  -l, --layer <layer>    specify the layer of output
  -d, --directory <dir>  specify the directory to generate structure tree
  -f, --only-folder      output folder only
  --icon                 output emoji icon, prefixing filename or directory
  -o, --output <output>  export content into a file, appending mode by default      
  -h, --help             display help for command
```

## Examples

Ignore `.git` and `node_modules` directory.

```bash
$ @osjwnpm/quibusdam-ab-consequatur -i '.git|node_modules' # or @osjwnpm/quibusdam-ab-consequatur -i '.git,node_modules'
@osjwnpm/quibusdam-ab-consequatur
├──📄.editorconfig
├──📄.eslintrc.js
├──📄.gitignore
├──📄.prettierrc.js
├──📄.release-it.json
├──📄CHANGELOG.md
├──📄LICENSE
├──📄package-lock.json
├──📄package.json
├──📄README.md
└──📁src
    ├──📄config.js
    ├──📄generate.js
    ├──📄index.js
    ├──📄toTree.js
    └──📄utils.js
```

Show emoji icon, prefixing filename or directory.

```bash
$ @osjwnpm/quibusdam-ab-consequatur -i '.git,node_modules' --icon
@osjwnpm/quibusdam-ab-consequatur
├──📄.editorconfig
├──📄.eslintrc.js
├──📄.gitignore
├──📄.prettierrc.js
├──📄.release-it.json
├──📄CHANGELOG.md
├──📄LICENSE
├──📄package-lock.json
├──📄package.json
├──📄README.md
└──📁src
    ├──📄config.js
    ├──📄generate.js
    ├──📄index.js
    ├──📄toTree.js
    └──📄utils.js
```

Export output into `result.md`, and append mode by default.

```bash
$ @osjwnpm/quibusdam-ab-consequatur -i '.git,node_modules' -o result.md
@osjwnpm/quibusdam-ab-consequatur
├──📄.editorconfig
├──📄.eslintrc.js
├──📄.gitignore
├──📄.prettierrc.js
├──📄.release-it.json
├──📄CHANGELOG.md
├──📄LICENSE
├──📄package-lock.json
├──📄package.json
├──📄README.md
└──📁src
    ├──📄config.js
    ├──📄generate.js
    ├──📄index.js
    ├──📄toTree.js
    └──📄utils.js
```
## License

[MIT](./LICENSE)
