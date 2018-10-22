# Version Control System

We use git.

## Use SSH key pairs instead of user/password over http

To generate your keys use the following guide provided by github:

https://help.github.com/enterprise/2.14/user/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/

## Git Flow and branching strategy

Git flow is a set of extensions for git at CLI and GUI for branching strategy.

See [Gitflow Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow) and [Gitflow Cheatsheet](https://danielkummer.github.io/git-flow-cheatsheet/)

Smartgit (GUI git client) has built-in support


For terminal, install git-flow in:

Debian/Ubuntu:

```
sudo apt install git-flow
```

MacOS:
```
brew install git-flow
``` 


## Do not store secrets in GIT

Do not commit an API key, user/password, tokens, or hardcoded private URLs.
Load secrets through **environment variables** or mount a file (for example, with docker volumes), put a secret file outside repository or add a secret file to ignored your .gitignore.

If a external secret is requiered to run an application, mention that the README.md of the application.

# Deterministic dependencies

Always prefere use a deterministic package manager, use something like lock-files. For example (in nodejs ecosystem), **yarn** and modern **npm** have lock-files.

In Docker, always set version tag of your base images.

Update your dependencies manually, and then test. Finally deploy.

# How to versioning an application

Use version standards from [SemVer](https://semver.org/).

# Lint your code

Add a linter to your applications. Add a lint command in your CI/CD test jobs.

Suggested linters:
*  [ESLint for Javascript](https://eslint.org/)
*  [Pylint for Python](https://www.pylint.org/)

# Time treatment

It is suggested to **store all the dates and times in UTC** at backend level, and then transform to the time zone only when displaying the date when necessary (for example in a frontend application).
