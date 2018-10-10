# Do not store secrets in GIT

Do not commit an API key, user/password, tokens, or hardcoded private URLs.
Load secrets through **environment variables** or mount a file ignored by git (.gitignore).

# How to versioning an application

Use version standards from [SemVer](https://semver.org/)

# Time treatment

It is suggested to **store all the dates and times in UTC** at backend level, and then transform to the time zone only when displaying the date when necessary (for example in a frontend application).
