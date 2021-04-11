# Commit Messages (in Pull Request) Checker with regex

![Version](https://img.shields.io/github/v/release/axe007/commit-message-checker?style=flat-square)
![Test](https://github.com/gsactions/commit-message-checker/workflows/build-test/badge.svg)

A GitHub action that checks that commit messages match a regex pattern. The
action is able to act on pull request and push events and check the pull
request title and body or the commit message of the commits of a push.

On pull requests the title and body are concatenated delimited by two line
breaks.

Designed to be very flexible in usage: you can split checks into various
workflows, using action types on pull request to listen on, define branches
for pushes etc. et some more thing 2 3 4 5 6 7 8 9 10 11 12 13 14

## Configuration

More information about `pattern` and `flags` can be found in the
[JavaScript reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp).

`flags` is optional and defaults to `gm`.

### Example Workflow

```yml
name: 'Commit Message Checker'

```

## Development

### Quick Start

```sh
git clone https://github.com/gsactions/commit-message-checker.git
npm install
npm run build
```

That's it, just start editing the sources...

### Commands

Below is a list of commands you will probably find useful during the development
cycle.

#### `npm run build`

Builds the package to the `lib` folder.

#### `npm run format`

Runs Prettier on .ts and .tsx files and fixes errors.

#### `npm run format-check`

Runs Prettier on .ts and .tsx files without fixing errors.

#### `npm run lint`

Runs Eslint on .ts and .tsx files.

#### `npm run pack`

Bundles the package to the `dist` folder.

#### `npm run test`

Runs Jest test suites.

#### `npm run all`

Runs all of the above commands.

## License

Based on previous work on https://github.com/GsActions/commit-message-checker.
This project is released under the terms of the [MIT License](LICENSE)
