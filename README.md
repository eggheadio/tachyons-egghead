# tachyons-egghead

Tachyons packages edited for egghead.io

---

# Usage

## Install the dependencies in your project

```
$ yarn add tachyons-egghead egghead-ui`
```

## Include the `tachyons-egghead` CSS classes

```
import 'tachyons-egghead'
```

Now you can use the [default tachyons class names](http://tachyons.io/docs/table-of-styles) as well as new egghead tachyons classes that you can find from the `github:eggheadio/tachyons-*` egghead modules in [the project's package.json dependencies](https://github.com/eggheadio/tachyons-egghead/blob/master/package.json).

If using React, you'll probably want to use `egghead-ui` as well; it is a library of React components used across egghead projects (it uses both `tachyons-egghead` classes and custom styles and exports React components).

---

# Development

## Dependencies

- Git
- Node
- Yarn

## Workflow

- `yarn` to install latest packages
- `yarn dev` to compile with a watcher
- `yarn verify` check builds work
- use [`yarn link`](https://yarnpkg.com/lang/en/docs/cli/link/) to test using changes in another project
    
## Deployment

After you have create a `feature-branch` off of `master`:
- create a `feature-branch` off of `master`
- commit the changes
- `git push --set-upstream origin feature_branch`
- `git push --tags`
- `yarn bump` and type in the new version using [Semantic Versioning](http://semver.org/)
- submit a pull request for the feature branch to `master`
- once PR status passes (approved review and successful [continuous integration in Travis CI](https://travis-ci.org/eggheadio/tachyons-egghead), merge the pull request and [continuous deployment in Travis CI](https://travis-ci.org/eggheadio/tachyons-egghead) publishes the new library version to [npm](https://www.npmjs.com/package/tachyons-egghead)
- notify consumers to run `yarn upgrade tachyons-egghead` in their projects to get latest, with a list of changes


## Debugging

In `src/tachyons.css` are imports you can uncomment for debugging.
