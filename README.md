# python-project-template

### Pre-requisites

Things that you need to have installed to use this template:

- `python@3.12`
- `poetry`
- `pre-commit`

It is also worth nothing that in order for the `pre-commit` hook to work, you will have to run:
```
foo@bar~: pre-commit install
```


### What's included?

> [!NOTE]
> Please look at the pre-requisites section before trying to set up a project with this
> template

- Automatically provides a starting point for a GitHub action which will lint and make sure that the
  code quality is being held in line
- Provides pre-commit-config which will: check the state of your poetry config, check various file formats,
  fix whitespace and end of files, and it will also run black
- Sets up an ordinary folder structure which is made up of just `src/*` and `tests/*` alongside a file at the root
  of the `src` directory.
- Sets up `.pylintrc` which only configures a longer line limit and ignores some annoying errors to do
  with module and method docstrings
- `.gitignore` is mostly default that is provided by GitHub, but it also ignores the `.DS_Store` as I am on a mac and
  `.idea/` as I am using pycharm
