# eslint-plugin-vue-scoped-css

[eslint-plugin-vue-scoped-css](https://www.npmjs.com/package/eslint-plugin-vue-scoped-css) is ESLint plugin for [Scoped CSS in Vue.js].

[![NPM license](https://img.shields.io/npm/l/eslint-plugin-vue-scoped-css.svg)](https://www.npmjs.com/package/eslint-plugin-vue-scoped-css)
[![NPM version](https://img.shields.io/npm/v/eslint-plugin-vue-scoped-css.svg)](https://www.npmjs.com/package/eslint-plugin-vue-scoped-css)
[![NPM downloads](https://img.shields.io/badge/dynamic/json.svg?label=downloads&colorB=green&suffix=/day&query=$.downloads&uri=https://api.npmjs.org//downloads/point/last-day/eslint-plugin-vue-scoped-css&maxAge=3600)](http://www.npmtrends.com/eslint-plugin-vue-scoped-css)
[![NPM downloads](https://img.shields.io/npm/dw/eslint-plugin-vue-scoped-css.svg)](http://www.npmtrends.com/eslint-plugin-vue-scoped-css)
[![NPM downloads](https://img.shields.io/npm/dm/eslint-plugin-vue-scoped-css.svg)](http://www.npmtrends.com/eslint-plugin-vue-scoped-css)
[![NPM downloads](https://img.shields.io/npm/dy/eslint-plugin-vue-scoped-css.svg)](http://www.npmtrends.com/eslint-plugin-vue-scoped-css)
[![NPM downloads](https://img.shields.io/npm/dt/eslint-plugin-vue-scoped-css.svg)](http://www.npmtrends.com/eslint-plugin-vue-scoped-css)
[![Build Status](https://github.com/future-architect/eslint-plugin-vue-scoped-css/workflows/CI/badge.svg?branch=master)](https://github.com/future-architect/eslint-plugin-vue-scoped-css/actions?query=workflow%3ACI)
[![Coverage Status](https://coveralls.io/repos/github/future-architect/eslint-plugin-vue-scoped-css/badge.svg?branch=master)](https://coveralls.io/github/future-architect/eslint-plugin-vue-scoped-css?branch=master)
<!--
[![Greenkeeper badge](https://badges.greenkeeper.io/future-architect/eslint-plugin-vue-scoped-css.svg)](https://greenkeeper.io/)
-->

## Features

This ESLint plugin provides linting rules relate to better ways to help you avoid problems when using [Scoped CSS in Vue.js].

- Provides linting rules for Scoped CSS.
- Supports CSS syntax including level 4 selectors.
- Supports `<style lang="scss">`.
- Supports `<style lang="stylus">`.
- Parses `<style>`, `<template>` and `<script>` blocks.

You can check on the [Online DEMO](https://future-architect.github.io/eslint-plugin-vue-scoped-css/playground/).

<!--DOCS_IGNORE_START-->

## Documentation

See [documents](https://future-architect.github.io/eslint-plugin-vue-scoped-css/).

## Installation

```bash
npm install --save-dev eslint eslint-plugin-vue-scoped-css
```

> **Requirements**
> 
> - ESLint v5.0.0 and above
> - Node.js v8.10.0 and above

<!--DOCS_IGNORE_END-->

## Usage

<!--USAGE_SECTION_START-->

Create `.eslintrc.*` file to configure rules. See also: [http://eslint.org/docs/user-guide/configuring](http://eslint.org/docs/user-guide/configuring).

Example **.eslintrc.js**:

```js
module.exports = {
  extends: [
    // add more generic rulesets here, such as:
    // 'eslint:recommended',
    'plugin:vue-scoped-css/recommended'
  ],
  rules: {
    // override/add rules settings here, such as:
    // 'vue-scoped-css/no-unused-selector': 'error'
  }
}
```

## Configs

This plugin provides 3 predefined configs:

- `plugin:vue-scoped-css/base` - Settings and rules to enable this plugin
- `plugin:vue-scoped-css/recommended` - Above, plus rules for better ways to help you avoid problems
- `plugin:vue-scoped-css/all` - All rules of this plugin are included

<!--USAGE_SECTION_END-->

## Rules

<!--RULES_SECTION_START-->

The `--fix` option on the [command line](https://eslint.org/docs/user-guide/command-line-interface#fixing-problems) automatically fixes problems reported by rules which have a wrench :wrench: below.

<!--RULES_TABLE_START-->

## Recommended for Vue.js 3.x

Enforce all the rules in this category with:

```json
{
  "extends": "plugin:vue-scoped-css/vue3-recommended"
}
```

| Rule ID | Description |    |
|:--------|:------------|:---|
| [vue-scoped-css/no-deprecated-deep-combinator](https://future-architect.github.io/eslint-plugin-vue-scoped-css/rules/no-deprecated-deep-combinator.html) | disallow using deprecated deep combinators | :wrench: |
| [vue-scoped-css/no-parsing-error](https://future-architect.github.io/eslint-plugin-vue-scoped-css/rules/no-parsing-error.html) | disallow parsing errors in `<style>` |  |
| [vue-scoped-css/no-unused-keyframes](https://future-architect.github.io/eslint-plugin-vue-scoped-css/rules/no-unused-keyframes.html) | disallow `@keyframes` which don't use in Scoped CSS |  |
| [vue-scoped-css/no-unused-selector](https://future-architect.github.io/eslint-plugin-vue-scoped-css/rules/no-unused-selector.html) | disallow selectors defined in Scoped CSS that don't use in `<template>` |  |
| [vue-scoped-css/require-scoped](https://future-architect.github.io/eslint-plugin-vue-scoped-css/rules/require-scoped.html) | enforce the `<style>` tags to has the `scoped` attribute |  |
| [vue-scoped-css/require-v-deep-argument](https://future-architect.github.io/eslint-plugin-vue-scoped-css/rules/require-v-deep-argument.html) | require selector argument to be passed to `::v-deep()` | :wrench: |
| [vue-scoped-css/require-v-global-argument](https://future-architect.github.io/eslint-plugin-vue-scoped-css/rules/require-v-global-argument.html) | require selector argument to be passed to `::v-global()` |  |
| [vue-scoped-css/require-v-slotted-argument](https://future-architect.github.io/eslint-plugin-vue-scoped-css/rules/require-v-slotted-argument.html) | require selector argument to be passed to `::v-slotted()` |  |

## Recommended for Vue.js 2.x

Enforce all the rules in this category with:

```json
{
  "extends": "plugin:vue-scoped-css/recommended"
}
```

| Rule ID | Description |    |
|:--------|:------------|:---|
| [vue-scoped-css/no-parsing-error](https://future-architect.github.io/eslint-plugin-vue-scoped-css/rules/no-parsing-error.html) | disallow parsing errors in `<style>` |  |
| [vue-scoped-css/no-unused-keyframes](https://future-architect.github.io/eslint-plugin-vue-scoped-css/rules/no-unused-keyframes.html) | disallow `@keyframes` which don't use in Scoped CSS |  |
| [vue-scoped-css/no-unused-selector](https://future-architect.github.io/eslint-plugin-vue-scoped-css/rules/no-unused-selector.html) | disallow selectors defined in Scoped CSS that don't use in `<template>` |  |
| [vue-scoped-css/require-scoped](https://future-architect.github.io/eslint-plugin-vue-scoped-css/rules/require-scoped.html) | enforce the `<style>` tags to has the `scoped` attribute |  |

## Uncategorized

No preset enables the rules in this category.
Please enable each rule if you want.

For example:

```json
{
  "rules": {
    "vue-scoped-css/require-selector-used-inside": "error"
  }
}
```

| Rule ID | Description |    |
|:--------|:------------|:---|
| [vue-scoped-css/require-selector-used-inside](https://future-architect.github.io/eslint-plugin-vue-scoped-css/rules/require-selector-used-inside.html) | disallow selectors defined that is not used inside `<template>` |  |

<!--RULES_TABLE_END-->
<!--RULES_SECTION_END-->

<!--DOCS_IGNORE_START-->

## Contributing

Welcome contributing!

Please use GitHub's Issues/PRs.

### Development Tools

- `npm test` runs tests and measures coverage.  
- `npm run update` runs in order to update readme and recommended configuration.  

<!--DOCS_IGNORE_END-->

## License

See the [LICENSE](LICENSE) file for license rights and limitations (MIT).

[Scoped CSS in Vue.js]: https://vue-loader.vuejs.org/guide/scoped-css.html
