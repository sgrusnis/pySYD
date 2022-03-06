-----

### \*\*\*\*\*\*\*\*\*\*\* We are continuously working towards our primary goal of accessible asteroseismology \*\*\*\*\*\*\*\*\*\*\*\*
 
-----

We would love for you to contribute to `pySYD` and make it even better than it is today! <br/>
For most (if not all) questions/concerns, peeping our [discussions](https://github.com/ashleychontos/pySYD/discussions) forum is an excellent place to start in order to look for solutions. If something is confusing, there is a good chance that someone else also found it confusing and hence already asked. 

As a contributor, here are the guidelines we ask you to follow:

- [Question or problem?](#question)
- [Issues & bugs](#issue)
- [New ideas](#feature)
- [Guidelines](#submit)
- [Style guide](#style)
- [Testing](#test)

-----

### <a name="question"></a> &rightarrow; Do you have a general question that is not directly related to software functionality?

**Please do *not* open 'issues' for general support questions as we want to preserve them for bug reports and new feature requests ONLY.** Therefore to save everyone time, we will be systematically closing all issues that do not follow these guidelines. Besides, you've got a much better chance of getting your question answered in our [discussion forum](stackoverflow.com/questions/tagged/angular-devtools). PLUS... we may already have the answer for you! 

Please visit our relevant [thread](https://github.com/ashleychontos/pySYD/discussions/37#discussion-3918112) first to see if your question has already been asked. You can also help us keep this space up-to-date, linking topics/issues to relevant threads and adding appropriate tags whenever/wherever possible. This is not only helpful to us but also helpful for the community! Once we have enough data points, we will establish a forum for frequently asked questions (FAQ).

If this still does not work for you and you would like to chat with someone in real-time, please contact [Ashley](achontos@hawaii.edu) to set up a call or zoom meeting.

-----

### <a name="issue"></a> &rightarrow; Are you reporting a bug?

**If the code crashes or you find a bug, please search the issue tracker first to make sure the problem (i.e. issue) does not already exist.** If and only if you do this but still don't find anything, feel free to [submit an issue](#submit-issue). And, if you're *really* brave, you can submit an issue along with a [pull request](#submit-pr) fix.

Ideally we would love to fix all issues Keep in mind that we would like to fix all issues as soon as possible, but before fixing a bug we need to reproduce and confirm it. In order to reproduce bugs we will systematically ask you to provide a minimal reproduction scenario by providing a project which breaks Angular DevTools. Also make sure that you list:

- version of Angular DevTools used
- version of Angular used
- 3rd-party libraries and their versions
- and most importantly - a use-case that fails

You can file new issues by filling out our [new issue form](https://github.com/rangle/angular-devtools/issues/new).

-----

### <a name="feature"></a> &rightarrow; Have an idea for a new feature or functionality?

You can _request_ a new feature by [submitting an issue](#submit-issue) to our GitHub
Repository. If you would like to _implement_ a new feature, please submit an issue with
a proposal for your work first, to be sure that we can use it.
Please consider what kind of change it is:

- For a **Major Feature**, first open an issue and outline your proposal so that it can be
  discussed. This will also allow us to better coordinate our efforts, prevent duplication of work,
  and help you to craft the change so that it is successfully accepted into the project.
- **Small Features** can be crafted and directly [submitted as a Pull Request](#submit-pr).

-----

### <a name="feature"></a> &rightarrow; Do you want to contribute code?

-----

## <a name="submit"></a> Submission Guidelines

### <a name="submit-issue"></a> Issues & Bugs

Before you submit an issue, please search the issue tracker, maybe an issue for your problem already exists and the discussion might inform you of workarounds readily available.

We want to fix all the issues as soon as possible, but before fixing a bug we need to reproduce and confirm it. In order to reproduce bugs we will systematically ask you to provide a minimal reproduction scenario by providing a project which breaks Angular DevTools. Also make sure that you list:

- version of Angular DevTools used
- version of Angular used
- 3rd-party libraries and their versions
- and most importantly - a use-case that fails

You can file new issues by filling out our [new issue form](https://github.com/rangle/angular-devtools/issues/new).

### <a name="submit-pr"></a> Submitting a Pull Request (PR)

#### Community Guidelines

Before you submit your Pull Request (PR), please consider the following guidelines:

- Search [GitHub](https://github.com/angular/angular) for an open or closed PR related to your submission in order to minimize duplicated efforts. 
- [Fork](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo) the rangle/angular-devtools repo.
- In your forked repository, make your changes in a new git branch:

  ```shell
  git checkout -b my-fix-branch main
  ```

- Create your patch, **including appropriate test cases**.
- Follow our [Coding Rules](#rules).
- Commit your changes using a descriptive commit message that follows our
  [commit message conventions](#commit). Adherence to these conventions
  is necessary because release notes are automatically generated from these messages.

  ```shell
  git commit -a
  ```

  Note: the optional commit `-a` command line option will automatically "add" and "rm" edited files.

- Push your branch to GitHub:

  ```shell
  git push origin my-fix-branch
  ```

- In GitHub, send a pull request to `angular-devtools:main`.
- If we suggest changes then:

  - Make the required updates.
  - Re-run the Angular DevTools test and lint suites to ensure tests are still passing and you're following the coding style.
  - Rebase your branch and force push to your GitHub repository (this will update your Pull Request):

    ```shell
    git rebase main -i
    git push -f
    ```

That's it! Thank you for your contribution!

#### After your pull request is merged

After your pull request is merged, you can safely delete your branch and pull the changes
from the main (upstream) repository:

- Delete the remote branch on GitHub either through the GitHub web UI or your local shell as follows:

  ```shell
  git push origin --delete my-fix-branch
  ```

- Check out the main branch:

  ```shell
  git checkout main -f
  ```

- Delete the local branch:

  ```shell
  git branch -D my-fix-branch
  ```

- Update your main with the latest upstream version:

  ```shell
  git pull --ff upstream main
  ```

## Pull Requests

 - PR title and description should follow [Angular Commit Message Conventions](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#-git-commit-guidelines)
 - link back to the original issue(s) whenever possible
 - new commands should be added to `docs/support_table.md` and `docs/supported.md`
 - commits should be squashed before merging
 - large pull requests should be broken into separate pull requests (or multiple logically cohesive commits), if possible

## <a name="test"></a> Testing

Local testing can be done by running the webpack-dev-server using configuration
`webpack.dev.js`. Run `yarn` to install dependencies, and then `yarn start`
to start the server.

This will host an interactive editor at
[http://localhost:7936/](http://localhost:7936/) to play around with and test
changes.

----------

### <a name="style"></a> Style guide

#### Code
 - 4 spaces for indentation
 - 80 character line length
 - commas last
 - declare variables in the outermost scope that they are used
 - camelCase for variables in JavaScript and for classes/objects in Python
 - snake_case for variables in Python

** A good rule of thumb is to try to make your code blend in with the surrounding code.

The code can be linted by running `yarn test:lint`, which lints JavaScript
files using ESLint and stylesheets using stylelint. They must pass to commit
the changes.

Some files have flowtype annotations and can be checked for type errors using
Flow by running `yarn test:flow`. See [Flow](https://flow.org/) for more details.

## <a name="rules"></a> Coding Rules

To ensure consistency throughout the source code, keep these rules in mind as you are working:

- All features or bug fixes **must be tested** by one or more specs (unit-tests).
- We follow [Google's JavaScript Style Guide][js-style-guide].

## Adding new functions

New functions should be added in [src/functions](src/functions) using
`defineFunction` from [defineFunction.js](src/defineFunction.js).  Read the
comments in this file to get started.  Look at
[phantom.js](src/functions/phantom.js) and
[delimsizing.js](src/functions/delimsizing.js) as examples of how to use
`defineFunction`.  Notice how delimsizing.js groups several related functions
together in a single call to `defineFunction`.

The new method of defining functions combines methods that were previously
spread out over three different files [functions.js](src/functions.js),
[buildHTML.js](src/buildHTML.js), [buildMathML.js](src/buildMathML.js) into a
single file.  The goal is to have all functions use this new system.

## License

`pySYD` is licenced under the [MIT License](http://opensource.org/licenses/MIT).