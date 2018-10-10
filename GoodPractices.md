# Do not store secrets in GIT

Do not commit an API key, user/password, tokens, or hardcoded private URLs.
Load secrets through **environment variables** or mount a file (for example, with docker volumes), put a secret file outside repository or add a secret file to ignored your .gitignore.

If a external secret is requiered to run an application, mention that the README.md of the application.

# How to versioning an application

Use version standards from [SemVer](https://semver.org/).

# Lint your code

Add a linter to your applications. Add a lint command in your CI/CD test jobs.

Suggested linters:
*  [ESLint for Javascript](https://eslint.org/)
*  [Pylint for Python](https://www.pylint.org/)

# Time treatment

It is suggested to **store all the dates and times in UTC** at backend level, and then transform to the time zone only when displaying the date when necessary (for example in a frontend application).
