# How to contribute

Contributions welcome!

## How to prepare

* You will need a [GitHub account](https://github.com/signup/free)
* Create an issue in this GitHub repo for your issue, if one does not yet exist
    * Describe the issue and include steps to reproduce if it's a bug.
    * Ensure to mention the earliest version that you know it affects.
* If you are able and want to fix this, [fork the repository on GitHub](https://docs.github.com/en/get-started/quickstart/fork-a-repo)

## Make Changes

* In your forked repository, create a feature branch for your upcoming patch. (e.g. `feature/issue-22-enhance-four-candles` or `bugfix/issue-42-crash-when-laughing`)
   * Usually this is based on the main branch.
   * Create a branch based on main;
     * `git checkout main`
     * `git checkout -b feature/issue-22-enhance-four-candles`
   * Please avoid working directly on the `main` branch.
* Make sure you stick to the coding style that is used already.
  * The project uses [Spotless](https://github.com/diffplug/spotless) to maintain a consistent code styling.
  * Run `./gradlew format` to format the code.
* Make commits of logical units and describe them properly.
* Submit tests to your patch / new feature, so it can be tested easily.

## Submit Changes

* Before submitting run `./gradlew format static test coverage`:
  * Running `./gradlew format` will ensure the code is correctly formatted. 
  * Running `./gradlew static` will run static code analysis.
  * Running `./gradlew test` will run all the tests.
  * Running `./gradlew coverage` will produce a code coverage report in 
    [`<project-roo>/build/reports/jacoco/coverage/html/index.html>`](build/reports/jacoco/coverage/html/index.html)
* Push your changes to a feature branch in your fork of the repository.
* [Open a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork), also known as a PR, to merge the changes from your branch into the main branch.
* Don't forget to [link your PR to the issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue) if you are solving one.
* Enable the checkbox to [allow maintainer edits](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/allowing-changes-to-a-pull-request-branch-created-from-a-fork) so the branch can be updated for a merge.
* Ensure all checks pass on the pull request.
* Once you submit your PR, a team member will review your proposal. We may ask questions or request additional information. We may ask for changes to be made before a PR can be merged, either using [suggested changes](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/incorporating-feedback-in-your-pull-request) or pull request comments.
* As you update your PR and apply changes, mark each conversation as [resolved](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/commenting-on-a-pull-request#resolving-conversations).

