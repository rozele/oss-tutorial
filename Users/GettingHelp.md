# Asking for Help

People are fallible, docs are fallible, and sometimes you just get stuck. Be aware of the many paths to getting unstuck.

- [ ] Avoid using *Issues*
- [ ] Use `git blame`
- [ ] Use Code Owners
- [ ] Leverage the developer communities

Remember, ***be respectful of maintainers time*** by leveraging the community-at-large when seeking help.

## Avoid using *Issues*

Unless explicitly stated, the *Issues* section on GitHub should be reserved for bugs. Unless you are reasonably certain you've encountered a bug, find other ways to ask for help.

## Use `git blame`

If you are hitting an issue with a specific piece of source code, it may be useful to contact the author of that code. `git blame` and commit history can help with that.

*Aside:* Tweeting to a community influencer about a feature or issue great way to both get help and boost your following.

### From History

*TODO:* image

### From GitHub.com

*TODO:* image

### From Visual Studio Team Services

*TODO:* image

### From CLI

Check the author of a line number for a given file:

```sh
git blame -L 8,10 ./Users/README.md
```

Check the author of a file before a given commit:

```sh
git blame f2214e84 ./Users/README.md
```

Other usage:

```sh
git blame -help
# usage: git blame [<options>] [<rev-opts>] [<rev>] [--] <file>
#
#    <rev-opts> are documented in git-rev-list(1)
#
#    --incremental         Show blame entries as we find them, incrementally
#    -b                    Show blank SHA-1 for boundary commits (Default: off)
#    --root                Do not treat root commits as boundaries (Default: off)
#    --show-stats          Show work cost statistics
#    --progress            Force progress reporting
#    --score-debug         Show output score for blame entries
#    -f, --show-name       Show original filename (Default: auto)
#    -n, --show-number     Show original linenumber (Default: off)
#    -p, --porcelain       Show in a format designed for machine consumption
#    --line-porcelain      Show porcelain format with per-line commit information
#    -c                    Use the same output mode as git-annotate (Default: off)
#    -t                    Show raw timestamp (Default: off)
#    -l                    Show long commit SHA1 (Default: off)
#    -s                    Suppress author name and timestamp (Default: off)
#    -e, --show-email      Show author email instead of name (Default: off)
#    -w                    Ignore whitespace differences
#    --minimal             Spend extra cycles to find better match
#    -S <file>             Use revisions from <file> instead of calling git-rev-list
#    --contents <file>     Use <file>'s contents as the final image
#    -C[<score>]           Find line copies within and across files
#    -M[<score>]           Find line movements within and across files
#    -L <n,m>              Process only line range n,m, counting from 1
#    --abbrev[=<n>]        use <n> digits to display SHA-1s
```

## Use Code Owners

GitHub allows you to specify code owners for files, directories, or various kinds of file matching patterns. Repos may decide to protect branches by requiring a review from a code owner. For more information, see [the GitHub blog](https://blog.github.com/2017-07-06-introducing-code-owners/).

## Where Developer Communities Lurk

Large open source projects often include information on where the developer communities exist

- StackOverflow
- Slack
- Discord
- Facebook Groups
