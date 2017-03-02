# tachyons-egghead

Tachyons packages edited for egghead.io

---

# Usage

```
$ yarn add 'tachyons-egghead'`
```

```
import 'tachyons-egghead'
```

Now you can use the [default tachyons class names](http://tachyons.io/docs/table-of-styles) as well as new egghead tachyons classes that you can find from the `github:eggheadio/tachyons-*` egghead modules in [the project's package.json dependencies](https://github.com/eggheadio/tachyons-egghead/blob/master/package.json).

---

# Development

## Dependencies

- Git
- Node
- Yarn

## Workflow

- create a feature branch off of `master`
- `yarn` to install latest packages
- `yarn dev` to compile with a watcher
- `yarn verify` check builds work
- use [`yarn link`](https://yarnpkg.com/lang/en/docs/cli/link/) to test using changes in another project
- if you want to publish a new library release, run `yarn bump` and type in the new version using [Semantic Versioning](http://semver.org/)
- submit a pull request for the feature branch to `master`
- once PR status passes (approved review and successful [continuous integration in Travis CI](https://travis-ci.org/eggheadio/tachyons-egghead), merge the pull request
- when `master` is updated
  - if there was a version bump, [continuous deployment in Travis CI](https://travis-ci.org/eggheadio/tachyons-egghead) publishes the new library version to [npm](https://www.npmjs.com/package/tachyons-egghead)
    - notify consumers to run `yarn upgrade tachyons-egghead` in their projects to get latest, with a list of changes
