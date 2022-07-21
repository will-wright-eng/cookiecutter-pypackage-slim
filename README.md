# cookiecutter pypackage slim

## Summary
### Background
- this project was heavily inspired by two projects:
	- [TezRomacH/python-package-template]
	- [waynerv/cookiecutter-pypackage]
- a number of repos were analyzed: [REFERENCES.md]
- cool tool used to [search cookiecutter templates on github]

[TezRomacH/python-package-template]: https://github.com/TezRomacH/python-package-template
[waynerv/cookiecutter-pypackage]: https://github.com/waynerv/cookiecutter-pypackage
[./REFERENCES.md]: ./references/REFERENCES.md
[search cookiecutter templates on github]:http://cookiecutter-templates.sebastianruml.name/

### Key components:
- docker
- makefile
- versioning
	- poetry
	- bump2version
- github actions
	- run tests
	- deploy to PyPI
	- dependabot
	- mkdocs (*TODO*)
- testing
	- black
	- tox
	- pytest
	- isort
	- mypy
	- flake8
- docs
	- bug report
	- feature request
	- questions
	- pull request
	- license
	- changelog
	- code of conduct
	- contributing
	- security

## Quick Start
- create github repo
- clone locally
- cookiecutter with defaults
- create branch in cloned repo
- copy/paste cookiecutter contents
- git add commit and push
- manually trigger `stage & preview workflow`

### Commands
```bash
git clone git@github.com:william-cass-wright/<project_name>.git
cookiecutter https://github.com/william-cass-wright/cookiecutter-pypackage-slim.git _<project_name>
# copy/paste contents
make poetry-download
make install
make pre-commit-install
git checkout -b first
git add .
git commit -m ":tada: Initial commit"
# this will run pre-commits and usually change something
git add .
git commit -m ":tada: Initial commit"
git push -u origin first
```