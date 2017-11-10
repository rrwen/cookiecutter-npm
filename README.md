# cookiecutter-npm

Richard Wen  
rrwen.dev@gmail.com  

Personal template for npm packages using cookiecutter.

## Install

1. Install [Python](https://www.python.org/downloads/)
2. Install [cookiecutter](https://pypi.python.org/pypi/cookiecutter) via `pip`
3. Install [Node.js](https://nodejs.org/en/)

```
pip install cookiecutter
```

## Usage

1. Create a template for a [npm](https://www.npmjs.com/) package using the cookiecutter command line interface
2. Change the directory to the folder with the same name as the `package_name` input
3. Update and install the developer dependencies using the [npm command](https://docs.npmjs.com/cli/npm)

```
cookiecutter gh:rrwen/cookiecutter-npm
cd <package_name>
npm update --dev
```

## Developer Notes

### Useful Commands

**Edit** the basic keys in `package.json`:

```
npm init
```

**Install all** dependencies in `package.json`:

```
npm install
```

**Install** a package and add it as a dependency with `--save`:

```
npm install --save <package-name>
```

**Uninstall** a package and dependency:

```
npm uninstall --save <package-name>
```

**Update all** dependencies in `package.json`:

```
npm update --dev
```

**Test** the package with [tape](https://www.npmjs.com/package/tape):

```
npm test
```

### Implementation

This template uses [cookiecutter](https://pypi.python.org/pypi/cookiecutter) to create folders and files for [npm](https://www.npmjs.com/) packages in [Node.js](https://nodejs.org/en/).

* The main file is [cookiecutter.json](https://github.com/rrwen/cookiecutter-npm/blob/master/cookiecutter.json) which defines the inputs for the command line interface
* The inputs then replace any values surrounded with `{{}}` inside the folder [{{cookiecutter.package_name}}](https://github.com/rrwen/cookiecutter-npm/tree/master/%7B%7Bcookiecutter.package_name%7D%7D)

```
        cookiecutter             <-- template tool
             |
      cookiecutter.json          <-- template inputs
             |
{{cookiecutter.package_name}}    <-- generated template
```

The following files will be created inside a folder with the same name as the `package_name` input:

* **tests/test.js**: a file that uses [tape]() to test the `index.js` module and logs results into `tests/log/` for the package version specified in `package.json`
* **.gitignore**: a Node [.gitignore](https://git-scm.com/docs/gitignore) automatically generated from github
* **.npmignore**: a file to specify ignoring `tests/logs/*`
* **.travis.yml**: a [.travis.yml](https://docs.travis-ci.com/user/languages/javascript-with-nodejs/) file for automatic builds and tests
* **LICENSE**: MIT [license file](https://help.github.com/articles/licensing-a-repository/) automatically created from github
* **README.md**: a readme [Mardown](https://daringfireball.net/projects/markdown/) file with header, install, usage, and developer notes sections
* **package.json**: the [npm package.json](https://docs.npmjs.com/files/package.json) specifications with [tape](https://www.npmjs.com/package/tape), [moment](https://www.npmjs.com/package/moment), [istanbul](https://www.npmjs.com/package/istanbul), and [coveralls](https://www.npmjs.com/package/coveralls) developer dependencies
* **index.js**: the main entry file for the npm package with an exported function consuming `options` as the main module

