---
layout: page
title: Contributions
---

Contributions to the project are greatly appreciated. But please read the requirements below before submitting a pull request.

Bug fixes and new features are great, but there are also many other ways to contribute. Contributions on documentation and examples are highly appreciated!

New features and bugs should always be added in the [issue tracker][issues]. It might be a good idea to discuss in the [forum][forum] first if you are not sure if it is a bug.

// TODO: information about branching and pull requests

### Requirements for pull requests

- Include examples or unit tests for the change / new feature
- Make sure the code builds on all platforms
- Make sure all unit tests are passing
- The new code should be StyleCop compliant (see [CodingStyle|coding style])

And please:

- commit clean change lists, make it easy to review
- define full name and e-mail address in the change list user information (to be used in the AUTHORS and CONTRIBUTORS files)
- include the issue number in the description, e.g. "#9945"
- do not mix multiple issues in the same change list
- do not clean code in the same change list as fixing an issue, do it in a separate change list

### Set user information in SourceTree

Tools | Options | General | Default user information

{Images/SourceTree_UserInformation.png}

### Set user information in TortoiseGit

Settings | Commit | Username: "First Last <email@address.com>"

{Images/TortoiseHg_UserInformation.png}

### Set user information in Git

See [first time Git setup](http://git-scm.com/book/en/Getting-Started-First-Time-Git-Setup).

[issues]: https://github.com/oxyplot/oxyplot/issues
[forum]: http://discussion.oxyplot.org