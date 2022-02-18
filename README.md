# A Skeleton Project for Python

This project tries to capture and represent the current best practice
for Python project layout.

Because best practices change over time and this project runs in
low-maintenance mode, we try to keep it minimalistic... to minimize
the impact of any errors or false suggestions presented here, and to
make them easier to fix.

# Basic Project Elements

## License

This project comes with a permissive [license](LICENSE). For your
own project, you may want to replace that file with something better
suited.

## Pipfile

This project uses the `pipenv` tool for project management, and
[Pipfile](Pipfile) is its masterfile. `Pipfile` is also a replacement
for `requirements.txt` when `pipenv` is used.

The `pipenv`/`Pipfile` take care of
- dependency specification (wildcard or fixed) and tracking
  (using an additional `Pipfile.lock` file)
- setting up a `venv` virtual environment with required packages
- shortcuts to run scripts in that environment (useful for build
  targets like `test`)

Note:

- if you don't continue from this project but want to setup a pristine
  project, `pipenv --python 3.9` (or whatever the target version is)
  will create a `Pipfile` in your present folder

# Reading Material

Some ressources and reading material has been taken into consideration,
you may want to check for yourself. Some things may be outdated, others may still be up-to-date.

- <https://docs.python-guide.org/writing/structure/> presents some basic
principles also used here. Some content may be outdated, eg., the article
still suggests using `requirements.txt` instead of the newer `Pipfile`.
