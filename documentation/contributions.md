---
layout: page
title: Contributions
---

Contributions to the project are greatly appreciated. But please read the requirements below before submitting a pull request.

Bug fixes and new features are great, but there are also many other ways to contribute. Contributions on documentation and examples are highly appreciated!

New features and bugs should always be added in the [issue tracker][issues]. It might be a good idea to discuss in the [forum][forum] first if you are not sure if it is a bug or a feature we want to include in the library.

### Branching

1. Log in to GitHub and open the [OxyPlot origin][origin] repository. Click the "Fork" button to create your own fork of the repository.
2. Create a clone on your local system: `git clone https://github.com/yourusername/oxyplot.git`
3. Create a branch for the bugfix/feature you want to work on: `git branch bugfix-some-error`
4. Checkout the branch: `git checkout bugfix-some-error`
5. Commit your changes
6. Push to your fork
7. Open the GitHub page for your fork and create a "Pull Request"

### Requirements for pull requests

- The pull request should be based on the latest commit on the `develop` branch of the OxyPlot origin repository
- Include examples or unit tests for the change / new feature
- Make sure the code builds on all platforms
- Make sure all unit tests are passing
- The new code should be StyleCop compliant (see [coding style](./coding-style))

And please:

- create a branch/pull request for each issue, do not combine multiple issues
- commit clean change lists, make it easy to review
- define full name and e-mail address in the change list user information
- update the AUTHORS and CONTRIBUTORS files if you are not already listed there
- include the issue number in the description, e.g. "#9945"
- do not clean code in the same commit as fixing an issue, do it in a separate commit

[origin]: https://github.com/oxyplot/oxyplot/
[issues]: https://github.com/oxyplot/oxyplot/issues
[forum]: http://discussion.oxyplot.org/
[git-setup]: http://git-scm.com/book/en/Getting-Started-First-Time-Git-Setup
[git-branching-model]: http://nvie.com/posts/a-successful-git-branching-model/
