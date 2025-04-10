| index | [npm-run-all] | [run-s] | [run-p] | [Node API] |
|-------|---------------|---------|---------|------------|

# npm-run-all2

[![npm version](https://img.shields.io/npm/v/npm-run-all2.svg)](https://www.npmjs.com/package/npm-run-all2)
[![Downloads/month](https://img.shields.io/npm/dm/npm-run-all2.svg)](http://www.npmtrends.com/npm-run-all2)
[![tests](https://github.com/bcomnes/npm-run-all2/workflows/tests/badge.svg)](https://github.com/bcomnes/npm-run-all2/actions)
[![Coverage Status](https://codecov.io/gh/bcomnes/npm-run-all2/branch/master/graph/badge.svg)](https://codecov.io/gh/bcomnes/npm-run-all2)
[![neostandard javascript style](https://img.shields.io/badge/code_style-neostandard-brightgreen?style=flat)](https://github.com/neostandard/neostandard)

* == CLI tool /
  * allows, run MULTIPLE npm-scripts
    * in parallel
    * sequential

## npm-run-all2 why?

* ⚠️`npm-run-all`'s maintenance fork ⚠️ +   
  * dependabot updates, 
  * release automation
  * removal of babel troubleshoot

## ⤴️ 's goal

- **Simplify**
  - Reason:🧠 official `npm run-script` command can NOT run MULTIPLE scripts & we want to run MULTIPLE scripts -> redundant a bit🧠
  - _Example:_
    ```
    # WITHOUT USING it
    npm run clean && npm run build:css && npm run build:js && npm run build:html
    
    # USING it
    npm-run-all clean build:*
    ``` 
- **Cross platform**
  - OTHERWISE, Node.js Windows users can NOT use `&`
    - `&`
      - enable run MULTIPLE commands PARALLEL
    - Reason: 🧠 `npm run-script` uses `cmd.exe` by default & NOT supported `&`🧠
    - ALTERNATIVE
      - `npm-run-all --parallel` 

## 💿 How to install?

* requirements
  * `Node@>=14`
    * if you use older versions -> it could work / BUT NO guarantees
* 
  ```bash
  $ npm install npm-run-all2 --save-dev
  # or
  $ yarn add npm-run-all2 --dev
  ```

## 📖 How to use?

### CLI Commands

- [npm-run-all]
  - MAIN one
- [run-s]
- [run-p]

#### Yarn / pnpm Compatibility

* == compatible with BOTH Yarn & pnpm

### -- via -- Node API

- [Node API]

[npm-run-all]: docs/npm-run-all.md
[run-s]: docs/run-s.md
[run-p]: docs/run-p.md
[Node API]: docs/node-api.md
