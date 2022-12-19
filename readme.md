# Typescript Boilerplate

A simple and ready to use Node.Js Typescript Boilerplate with some custom configs for ME.

This boilerplate includes some basic tools as:

- [ESlint][eslint] for code linting.
- [Jest][jest] for unit testing and coverage.
- [Husky][husky] to run scripts based on git hooks.
- [CommitMessageLinter][msg-linter] to prevent commits outside the conventional format.
- [LintStaged][lint-staged] to run tests only on staged files.
- [FakerJs][faker-js] to create random values for tests.

## Getting Started

To clone the repository, use the following commands:

```sh
git clone https://github.com/gabriel-fabian/typescript-boilerplate
cd typescript-boilerplate
npm install && npm run prepare
```

## Additional Information

This boilerplate will prevent commits outside the [ConventionalCommits][conventional-commits] format, if you don't know what that is read the linked DOC.

Husky is configured to run two scripts, one for pre commit and other for pre push, the first one will execute [LintStaged][lint-staged] which will run all the commands in `.lintstagedrc.json` config file for the specified file extensions. The second one will run Jest with coverage option.

If Husky isn't working make sure to run `npm run prepare` and have files matching the LintStaged config.

Licensed under the GNU GPL v3.0. See the [LICENSE](https://github.com/gabriel-fabian/typescript-boilerplate/blob/master/LICENSE) file for details.

[eslint]: https://github.com/eslint/eslint
[jest]: https://github.com/facebook/jest
[husky]: https://github.com/typicode/husky
[msg-linter]: https://github.com/legend80s/commit-msg-linter
[lint-staged]: https://github.com/okonet/lint-staged
[faker-js]: https://github.com/faker-js/faker
[conventional-commits]: https://www.conventionalcommits.org/
