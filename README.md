# @hishprorg/saepe-pariatur

[Read the Docs](https://@hishprorg/saepe-pariatur.dev)

## Like Lodash, but in TypeScript and for ESNext.

Stop shipping code built for browsers from 2015. Really though, look at all the [issues](https://github.com/lodash/lodash/issues/2930).

You may prefer this because it's:

* **TypeScript & docs**: Includes type declaration files and js with JSDocs for best in class experience.
* **Zero deps**: Built from scratch with no runtime dependencies or polyfills.
* **ESNext**: Uses modern idiomatic syntax, data structures, and control flow techniques.
* **Modular**: Pick what you need. Supports tree-shaking, no side effects, and works with all bundlers.
* **Lazy**: Leverage generators, iterators, and functional composition.
* **Tests**: All modules have comprehensive test suites and public apis are 100% covered.

## Docs

📖 Available at [@hishprorg/saepe-pariatur.dev](https://@hishprorg/saepe-pariatur.dev)

## Get Started

This library is available as an [npm package](https://www.npmjs.com/package/@hishprorg/saepe-pariatur).

To install the package you need to have [npm](https://www.npmjs.com/get-npm) (or [yarn](https://yarnpkg.com/getting-started/install)) installed and then run:

```bash
npm install @hishprorg/saepe-pariatur
```

## How to use

Just import any function or class you need.

```js
import { sorted, times, uniqueId } from '@hishprorg/saepe-pariatur'

times(5, (i) => i)
// -> [0, 1, 2, 3, 4]

sorted([4, 3, 2, 1])
// -> [1, 2, 3, 4]

uniqueId('user_')
// -> 'user_101225005'
...
```

See the full list of [modules](https://@hishprorg/saepe-pariatur.dev/modules.html).

## Data model
This library features a data model similar to [Python](https://docs.python.org/3/reference/datamodel.html#special-method-names) but not always. Only the missing parts have been implemented, while respecting the JS standards.

For example, in Python collections, `size()` is a method, while in JS it's just a property. So this library uses `size` property instead of method. Similarly, the `len` function implementation checks for both `length` and `size` since many JS objects have a `length` property.

## Special method names
This library adds support for operators using object methods such as:
  - `obj.eq(other)`  adds custom `obj == other`.
  - `obj.lt(other)`  adds custom `obj < other`.
  - `obj.lte(other)`  adds custom `obj <= other`.
  - `obj.gt(other)`  adds custom `obj > other`.
  - `obj.gte(other)`  adds custom `obj >= other`.
  - `obj.compare(other)`  overloads sorting operations.

When working with objects, functions in this library use these custom operators for equality and sorting. You can also apply operators to values like `eq(x, y)`, `lte(x, y)`, `compare(x, y)`, etc.

## New Types

[`Decimal`](https://@hishprorg/saepe-pariatur.dev/classes/decimal.Decimal.html) provides support for correct rounded floating point arithmetic, with arbitrary precision.

Some common base interfaces and typing patterns you may have seen like `Optional`, `Result`, `Comparable`, `Iterator`, and others.

### Sorted Containers
  - [SortedSet](https://@hishprorg/saepe-pariatur.dev/classes/collections.SortedSet.html)
  - [SortedMap](https://@hishprorg/saepe-pariatur.dev/classes/collections.SortedMap.html)
  - [SortedTree](https://@hishprorg/saepe-pariatur.dev/classes/collections.SortedTree.html)

### Other Containers
  - [Deque](https://@hishprorg/saepe-pariatur.dev/classes/collections.Deque.html)
  - [FrozenSet](https://@hishprorg/saepe-pariatur.dev/classes/collections.FrozenSet.html)
  - [LRUCache](https://@hishprorg/saepe-pariatur.dev/classes/collections.LRUCache.html)


## Contributing
If you want to contribute to the project and make it better, your help is very welcome. Contributing is also a great way to learn more about social coding on Github, new technologies and and their ecosystems and how to make constructive, helpful bug reports, feature requests and the noblest of all contributions: a good, clean pull request. You will be listed as a **Champion** on the official site as well.


## License

[Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0)
