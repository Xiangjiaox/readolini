# Readolini

# Contributing

## Workflow
This project uses a trunk-based with short-lived feature branches, and rebase as a git strategy. Feature branches must be self-contained and tied to an issue ticket, and are squashed before rebased onto main after approved PR.

Commits are made following the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) convention: 
```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```
Where `<type>` is one from the table below. 
An optional `scope` can be added for further context, e.g `fix(server): misspelled application config key`.


| Type     | Description                                                              |
| -------- | ------------------------------------------------------------------------ |
| feat     | New feature.                                                             |
| fix      | A bug fix.                                                               |
| docs     | Documentation only changes.                                              |
| style    | Changes that do not affect meaning of code, formatting, white-space etc. |
| refactor | Changes that neither fixes a bug nor adds a feature.                     |
| perf     | Changes that improve performance.                                        |
| test     | Adding missing or correcting existing tests.                             |
| build    | Changes that affect the build system, maven, npm, gulp etc.              |
| ci       | Changes to CI configuration files and scripts.                           |
| chore    | Other changes that don't modify src or test files.                       |
| revert   | Reverts a previous commit.                                          	  |

1. Create a branch.
2. Develop feature/bugfix.
	- Create tests.
3. Clean up commit messages following the convention.
4. Create pull-request.
	- Check if build is failing.
	- Incorporate feedback.
5. Squash & rebase.