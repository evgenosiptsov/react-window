Changelog
------------

### Unreleased
* Remove `overflow:hidden` from inner container ([souporserious](https://github.com/souporserious) - [#56](https://github.com/bvaughn/react-window/pull/56))

https://github.com/bvaughn/react-window/pull/

### 1.1.2
* 🐛 Fixed edge case `scrollToItem` bug that caused lists/grids with very few items to have negative scroll offsets.

### 1.1.1
* 🐛 `FixedSizeGrid` and `FixedSizeList` automatically clear style cache when item size props change.

### 1.1.0
* 🎉 Use explicit `constructor` and `super` to generate cleaner component code. ([Andarist](https://github.com/Andarist) - [#26](https://github.com/bvaughn/react-window/pull/26))
* 🎉 Add optional `shouldForceUpdate` param reset-index methods to specify `forceUpdate` behavior. ([nihgwu](https://github.com/nihgwu) - [#32](https://github.com/bvaughn/react-window/pull/32))

### 1.0.3
* 🐛 Avoid unnecessary scrollbars for lists (e.g. no horizontal scrollbar for a vertical list) unless content requires them.

### 1.0.2

* 🎉 Enable Babel `annotate-pure-calls` option so that classes compiled by "transform-es2015-classes" are annotated with `#__PURE__`. This enables [UglifyJS to remove them if they are not referenced](https://github.com/mishoo/UglifyJS2/pull/1448), improving dead code elimination in application code. ([Andarist](https://github.com/Andarist) - [#20](https://github.com/bvaughn/react-window/pull/20))
* 🎉 Update "rollup-plugin-peer-deps-external" and use new `includeDependencies` flag so that the "memoize-one" dependency does not get inlined into the Rollup bundle. ([Andarist](https://github.com/Andarist) - [#19](https://github.com/bvaughn/react-window/pull/19))
* 🎉 Enable [Babel "loose" mode](https://babeljs.io/docs/en/babel-preset-env#loose) to reduce package size (-8%). ([Andarist](https://github.com/Andarist) - [#18](https://github.com/bvaughn/react-window/pull/18))

### 1.0.1
Updated `README.md` file to remove `@alpha` tag from NPM installation instructions.

# 1.0.0
Initial release of library. Includes the following components:
* `FixedSizeGrid`
* `FixedSizeList`
* `VariableSizeGrid`
* `VariableSizeList`
