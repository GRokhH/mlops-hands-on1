[![Python application test with GitHub Actions](https://github.com/GRokhH/mlops-hands-on1/actions/workflows/testing-ci.yml/badge.svg)](https://github.com/GRokhH/mlops-hands-on1/actions/workflows/testing-ci.yml)

1. create a venv
1. Makefile -> keep a lot of complex commands (like a cookbook)
1. requirements.txt

**Makefile:**
- print make + tab in terminal lists the commands in the makefile.
- in linting, we disable convention and refactor messages with --disable=C,R because we want to only see warnings and errors
- calling "make format" cleans up the code
- the "all" command chains the commans in our desired order
- before check-in the code into github we would run "make all"
- a good order for "all" would be: install, lint, test, format

**Installing Packages**
- we run "make install"
- installation is an important component of CI
- we would test the installation of the packages in the build system

**ipython**
- a command shell for interactive computing
- good for debugging code and playing around with things
- we type "ipython" in the terminal and we would be able to use the interactive shell


**Run the test**
- to make the test extra verbous we use the "-vv" flag
- we run "make test"
- pytest-cov shows us what percentage of the tests have passed


**pylint**
- Pylint is a static code analyser 
- works very well with pytest and is its complimentory

