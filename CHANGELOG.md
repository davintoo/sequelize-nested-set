# Changelog
All notable changes to this project (as a library) will be documented in this file.

This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

Also this project likes fast realizes with even one change to get it live shortly.

## Next release
- Update [Docs](https://github.com/fremail/sequelize-nested-set/wiki) and README. 
- Add tests on Node v12.
- Rework `getParent()` method.

New features and bug fixes will be here.

## 1.3.1 - 2019-05-24
- Fix `makeRoot()` function: it didn't move children to new tree.

## 1.3.0 - 2019-05-08
- Fix typos in `isDescendantOf()` and `isDescendantOfOrEqualTo()` function description.
- Add Sequelize to peerDependencies.
- Add tests for Sequelize v4 and v5.
- Fix potential security vulnerability in dependencies.

## 1.2.0 - 2019-05-06
- Rename first param in `addChild()`.
- Remove redundant newRootId param from `makeRoot()`.
- Add brief API docs in [wiki](https://github.com/fremail/sequelize-nested-set/wiki).

## 1.1.3 - 2019-04-18
- Fix `addChild()`, `insertAsParentOf()`, `insertAsLastChildOf()`, `insertAsFirstChildOf()`, `insertAsNextSiblingOf()`, `insertAsPrevSiblingOf()`, `updateNode()`, `shiftRlValues()`, `shiftRlRange()`.
- Deeply clone options in functions.
- Update dev dependencies.
- Improve `isValidNode()`: check record existence.

## 1.1.2 - 2019-04-06
- Bug fix for `getSiblings()`.

## 1.1.1 - 2019-01-28
- Bug fix: disallow calling `createRoot()` w/o Sequelize record.
- Bug fix: add default value for `options` param for `delete()`.
- Bug fix for `getPrevSibling()`, `getNextSibling()`, `getFirstChild()`, `getLastChild()`, `getParent()`.
- Bug fix for `getDescendants()`, `getAncestors()`.

## 1.1.0 - 2019-01-05
- Add `rootColumnType` option.
- Bug fix: set tmp value for rootId in `createRoot()` function.

## 1.0.1 - 2018-12-21
- Bug fix: replace missed arrow functions to 'function'.

## 1.0.0 - 2018-12-21
- Add `options` as last argument to all functions making queries.
- Replace `transaction` function argument with `options`.

## 0.1.0 - 2018-12-19
- Replace arrow functions to 'function'.
- Add `lft` and `rgt` to `getDescendants` function.
- Force `depth` to integer in `getDescendants` and `getAncestors` functions.
- Remove unique modifiers from `lft` and `rgt` column declaration.
- Add options to use different column names for `lft` and `rgt` columns.
- Add CHANGELOG
