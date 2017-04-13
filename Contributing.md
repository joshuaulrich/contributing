# Have a question?

Please do not open an issue to ask a question about how to use the package.
Instead, ask your question on [Stack Overflow](http://stackoverflow.com/questions/tagged/r)
or the [R-SIG-Finance](https://stat.ethz.ch/mailman/listinfo/r-sig-finance)
mailing list (you must subscribe to post).

# Have a bug report or feature request?

1. Determine which repository the bug/feature should be reported in. The process
   of creating a [*minimal*, reproducible example](http://stackoverflow.com/q/5963269/271616)
   should identify the package that contains the bug or should contain the
   feature. Email me if you're unsure where to create an issue.
2. Search current open GitHub [issues]() to check if the bug/feature has already
   been reported/requested.
[//]: # "FIXME: Should there be a bug/feature split here?"
3. Ensure your local copy is up-to-date, and verify the bug still exists in the
   HEAD of the master branch.
4. If the bug exists in the HEAD of master, and you can't find an open issue,
   then [open a new issue](). Please be sure to:
  * Use an informative and descriptive title,
  * Include as much relevant information as possible; at minimum:
    * a [minimal, reproducible example](http://stackoverflow.com/q/5963269/271616)
    * the output from `sessionInfo()`.
  * Describe the expected behavior and why you think the current behavior is
    a bug.

# Want to submit a pull request?

1. Changes that are purely cosmetic in nature (e.g. whitespace changes, code
   formatting, etc) will generally not be accepted because they do not add to
   the stability, functionality, or testability of the project.
2. Unless the change is extremely trivial (e.g. typos), please
   [create an issue](#have-a-bug-report-or-feature-request) and wait for
   feedback *before* you start work on a pull request. That will avoid the
   possibility you spend time on a patch that won't be merged.
3. Create a branch for the feature/bug fix reported in the issue. Please use a
   short and descriptive branch name that starts with the issue number (e.g.
   123_custom_function). Use that branch as the base for your pull request.
   Pull requests on your version of `master` will not be accepted, because
   they can make it difficult for you to update your fork if your pull request
   isn't incorporated verbatim.
4. A pull request should only be for one issue, so please `git rebase -i` and
   squash the commits on your feature branch into one commit before creating
   the pull request. Please use `git commit --amend` to amend your commit if
   you are asked to make changes. It's okay to force update your pull request
   with `git push --force`.
5. Please write a great [commit message](#commit-messages).
6. It would be much appreciated if you also add tests that cover your changes.

----

# Commits
* don't mix functional and non-functional changes (you didn't make
  non-funcitonal changes, did you? :P)
* try to make each commit a logically separate changeset
  * use `git add --patch` to interactively stage changes
* style guide...
  * in `if` statments, use `&&`, `||`, `isTRUE`

# Commit Messages

Follow the [The Seven Rules](http://chris.beams.io/posts/git-commit/#seven-rules)
of [How to Write a Git Commit Message](http://chris.beams.io/posts/git-commit/).
Pay particular attention to rule 7: [Use the body to explain what and why
versus how](http://chris.beams.io/posts/git-commit/#why-not-how). The body
should also include the motivation for the change and how it compares to prior
behavior.

If the commit is to fix a bug or add a feature, the commit message should
contain enough information to understand the bug/feature without having to
reference an external tracker (e.g. GitHub issues). But please *do reference
the GitHub issue* on the last line of your commit message body. Look at [this
commit](https://github.com/joshuaulrich/xts/commit/ce1b667ab7c38cb2633fca0075652a69e5d2a343)
for an example.

# References:
1. The [data.table Contributing Guide](https://github.com/Rdatatable/data.table/blob/master/Contributing.md).
2. The [Atom Contributing Guide](https://github.com/atom/atom/blob/master/CONTRIBUTING.md).
3. How to create a [minimal, reproducible example](http://stackoverflow.com/q/5963269/271616).
4. [How to Write a Git Commit Message](http://chris.beams.io/posts/git-commit/).
