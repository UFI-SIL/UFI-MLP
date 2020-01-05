# Contributing to oneVPL

The following is a set of guidelines for contributing to oneVPL and its packages,
which are hosted in the [Intel® oneAPI Video Processing Library
Group](https://gitlab.devtools.intel.com/video-processing-lib) on GitLab. Feel
free to propose changes to this document in a merge request.

## Table of Contents

*   [Important Resources](#important-resources)
*   [Contributing Code](#contributing-code)
    *   [Expectations](#expectations)
    *   [Merge Requests](#merge-requests)
    *   [How to Test](#how-to-test)
    *   [Development Environment Setup](#development-environment-setup)
    *   [Development Process](#development-process)
*   [Style Guides](#styleguides)
    *   [Git Commit Messages](#git-commit-message-style)
    *   [Markdown](#markdown-style-guide)
    *   [Documentation](#documentation-style)
    *   [C](#c-style)
    *   [Python](#python-style)

# Important Resources

*   [Feature tracking](https://rally1.rallydev.com/#/304579368208d/)
*   [Defect tracking](https://rally1.rallydev.com/#/304579368208d/defects)

# Contributing Code

## Expectations

When submitting a merge request the developer is expected to have done
a due diligence effort to ensure the code submitted will not break the
build or add undue burden on other developers. To do this there are
certain actions developers should do before submitting code for review.

* full project builds on at least one platform
```bash
# mkdir build
# cd build
# cmake ..
# cmake --build .
```
* project build does not have any known fails (i.e. it is not sufficient
to have a platform where the builds pass if the developer knows of a
system where build fails)
* Unit tests pass
```bash
# vpl-utest
```
* An effort has been made to ensure content checked in align to the style
guides in this document.

# Style Guides

## Git Commit Message Style

1.  Separate subject from body with a blank line
2.  Limit the subject line to 50 characters
3.  Capitalize the subject line
4.  Do not end the subject line with a period
5.  Use the imperative mood in the subject line
6.  Wrap the body at 72 characters
7.  Use the body to explain what and why vs. how

Further reading:
[How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/)

## Markdown Style

Markdown documents should follow [Google markdown
style](https://github.com/google/styleguide/blob/gh-pages/docguide/style.md). 

The project has an 80 character line limit.

## Documentation Style

*   [Best practices](https://github.com/google/styleguide/blob/gh-pages/docguide/best_practices.md)

## C Style

C code should follow the 
[Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html).

## Python Style

Python code should follow [PEP 8](https://www.python.org/dev/peps/pep-0008/).
