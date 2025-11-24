# json-anything-endproduct

<!-- Strong badge header -->
[![npm version](https://img.shields.io/npm/v/json-anything-endproduct.svg)](https://www.npmjs.com/package/json-anything-endproduct)
[![npm downloads](https://img.shields.io/npm/dm/json-anything-endproduct.svg)](https://www.npmjs.com/package/json-anything-endproduct)
[![bundle size](https://img.shields.io/bundlephobia/minzip/json-anything-endproduct.svg)](https://bundlephobia.com/package/json-anything-endproduct)
[![license](https://img.shields.io/badge/license-MIT-green.svg)](../LICENSE)
[![module](https://img.shields.io/badge/module-ESM-blue.svg)](#)
[![dependencies](https://img.shields.io/badge/dependencies-none-brightgreen.svg)](#)
[![maintenance](https://img.shields.io/badge/maintenance-active-brightgreen.svg)](#)
[![tested with](https://img.shields.io/badge/tested%20with-Node%20%3E=%2012-brightgreen.svg)](#)

JSON → Anything Converter — compact ES module with 25 dependency-free converters for quick conversions, docs and prototypes.

Why this package stands out:

- Small and dependency-free — ideal for embedding in docs or developer tools.
- Multi-format: CSV, YAML-like, SQL, TypeScript, language class generators and more.
- ESM-first: ship as a modern ES module (`type: module`).

Quick install (local development):

```bash
# from project root
cd npm
npm install
```

Install from npm (when published):

```bash
npm install json-anything-endproduct
```

Quick usage (ES modules)

```js
import { toCSV, toYAML, toMarkdownTable } from 'json-anything-endproduct';

const data = [{ id: 1, name: 'Alice' }, { id: 2, name: 'Bob' }];
console.log(toCSV(data));
console.log(toYAML(data));
console.log(toMarkdownTable(data));
```

Test from the repo (no publish):

```bash
node -e "import('./npm/index.js').then(m=>console.log(m.toCSV([{a:1,b:2}])))"
```

Core API (selected converters)

- toYAML — YAML-like serializer
- toCSV — CSV generator (headers from keys)
- toTypeScript — TypeScript interface generator
- toJS — pretty-printed JSON
- toSchemaSummary — key:type summary
- toHTMLTable / toHTML — HTML table
- toQuery / toFormURLEncoded — URL encoders
- toMarkdownTable — Markdown table
- toPlantUML / toMermaid — diagram skeletons
- toSQLInsert / toSQLiteInsert / toMySQLInsert / toPostgresInsert — SQL INSERTs
- toBashExport — bash env exports
- toCSharp / toJava / toPythonDataclass / toGoStruct / toRustStruct / toDartClass / toPHPArray — language-specific outputs
- toProto — naive proto3 generator


License

MIT


