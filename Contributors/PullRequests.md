# Submitting Pull Requests

Pull requests are a way to ask for an open source project to merge your changes. There are some things to be mindful of when submitting pull requests:

- [ ] Read CONTRIBUTING.md before you get started
- [ ] Fill out the pull request template
- [ ] Fill out the pull request description
- [ ] Use good commit messages
- [ ] Fix one thing at a time
- [ ] Match repo style / use linters
- [ ] Squash related commits
- [ ] Run all tests.
- [ ] Add more tests.

Taking these steps ensure you ***respect maintainers time***.

## What's in CONTRIBUTING.md

- [ ] PR Process
- [ ] Coding Style Guides
- [ ] Autodocs Info
- [ ] Running Tests
- [ ] Commit Message Guidelines
- [ ] Rules for Filing Bugs

RxJS has a great example for [`CONTRIBUTING.md`](https://github.com/ReactiveX/rxjs/tree/master/CONTRIBUTING.md).

## Example rull request template

*TODO:* PR template image

## Example commit messages

**Bad:** Made some changes to the docs.

**Good:** Adds details for CLI commands to install dependencies.

## Reasons to fix one thing at a time

- Easier to review
- Smaller diff
- Revert isolation
- Easier to document in release notes

## What to do with styles in absence of CONTRIBUTING.md

*TODO:* tabs vs spaces meme
*TODO:* JavaScript semicolon meme

## Squashing commits

Squashing commits is something you should do before submitting pull requests. Incremental commits are great for private workflows, and indeed recommended, but when it comes time to merge, put a bow on it by squashing. Depending on the project, the committer may squash your commits for you anyway, wouldn't you rather be in control?

### How to squash

You can squash commits using an interactive rebase operation:

```sh
git checkout myFeature
git rebase -i HEAD~N # replace N with the number of commits to squash
```

When the editor pops up, use either the `squash` or `fixup` options for commits you want to squash.

### When not to squash

- Multiple authors
- Isolated, but tightly coupled features
- Code review has taken place
