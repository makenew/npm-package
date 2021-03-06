# npm Package Skeleton

[<img src="https://makenew.github.io/makenew.svg" alt="Make New" height="20">](https://makenew.github.io/)
[![npm](https://img.shields.io/npm/v/makenew-npm-package.svg)](https://www.npmjs.com/package/makenew-npm-package)
[![GitHub license](https://img.shields.io/github/license/makenew/npm-package.svg)](./LICENSE.txt)
[![David](https://img.shields.io/david/makenew/npm-package.svg)](https://david-dm.org/makenew/npm-package)
[![David](https://img.shields.io/david/dev/makenew/npm-package.svg)](https://david-dm.org/makenew/npm-package#info=devDependencies)
[![Travis](https://img.shields.io/travis/makenew/npm-package.svg)](https://travis-ci.org/makenew/npm-package)

## Description

Bootstrap a new [npm package] in less than a minute.

[npm package]: https://docs.npmjs.com/how-npm-works/packages

### Features

- [Node.js]'s [npm] package structure.
- [Travis CI] ready.
- [Keep a CHANGELOG].
- Consistent coding with [EditorConfig].
- Badges from [Shields.io].

[EditorConfig]: http://editorconfig.org/
[Keep a CHANGELOG]: http://keepachangelog.com/
[Node.js]: https://nodejs.org/
[npm]: https://www.npmjs.com/
[Shields.io]: http://shields.io/
[Travis CI]: https://travis-ci.org/

### Bootstrapping a New Project

1. Clone the master branch of this repository with

   ```
   $ git clone --single-branch https://github.com/makenew/npm-package.git new-npm-package
   $ cd new-npm-package
   ```

   Optionally, reset to the latest [release][Releases] with

   ```
   $ git reset --hard npm-package-v1.0.1
   ```

2. Run

   ```
   $ ./makenew.sh
   ```

   and follow the prompts.
   This will replace the boilerplate, delete itself,
   and stage changes for commit.
   This script assumes the project repository will be hosted on GitHub.
   For an alternative location, you must update the URLs manually.

3. Fill in the README Description section.

4. If [choosing a license][Choose a license] other than the one provided:
   update `LICENSE.txt`, the README License section,
   and `package.json` with your chosen license.

5. If `index.js` will not be the main file for this package, replace or
   remove it and update the `main` and `files` fields in `package.json`.

[Choose a license]: http://choosealicense.com/
[Releases]: https://github.com/makenew/npm-package/releases
[The Unlicense]: http://unlicense.org/UNLICENSE

### Updating

If you want to pull in future updates from this skeleton,
you can fetch and merge in changes from this repository.

If this repository is already set as `origin`,
rename it to `upstream` with

```
$ git remote rename origin upstream
```

and then configure your `origin` branch as normal.

Otherwise, add this as a new remote with

```
$ git remote add upstream https://github.com/makenew/npm-package.git
```

You can then fetch and merge changes with

```
$ git fetch upstream
$ git merge upstream/master
```

#### Changelog

Note that `CHANGELOG.md` is just a template for this skeleton.
The actual changes for this project are documented in the commit history
and summarized under [Releases].

## Installation

The recommended method is to add this as a dependency
to your project using [npm] with

```
$ npm install --save makenew-npm-package
```

Alternatively, you can download a [release][Releases]
or clone the repository directly.

[npm]: https://www.npmjs.com/
[Releases]: https://github.com/makenew/npm-package/releases

## Development and Testing

### Source Code

The [makenew-npm-package source] is hosted on GitHub.
Clone the project with

```
$ git clone https://github.com/makenew/npm-package.git
```

[makenew-npm-package source]: https://github.com/makenew/npm-package

### Requirements

You will need [Node.js] with [npm].

Install the development dependencies with

```
$ npm install
```

[Node.js]: https://nodejs.org/

## Contributing

Please submit and comment on bug reports and feature requests.

To submit a patch:

1. Fork it (https://github.com/makenew/npm-package/fork).
2. Create your feature branch (`git checkout -b my-new-feature`).
3. Make changes.
4. Commit your changes (`git commit -am 'Add some feature'`).
5. Push to the branch (`git push origin my-new-feature`).
6. Create a new Pull Request.

## License

This software can be used freely, see [The Unlicense].
The copyright text appearing below and elsewhere in this repository
is for demonstration purposes only and does not apply to this software.

This npm package is licensed under the MIT license.

## Warranty

This software is provided "as is" and without any express or
implied warranties, including, without limitation, the implied
warranties of merchantibility and fitness for a particular
purpose.
