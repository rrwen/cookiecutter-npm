# {{cookiecutter.package_name}}

{{cookiecutter.author}}  
{{cookiecutter.email}}  

{{cookiecutter.package_description}}

[![npm version](https://badge.fury.io/js/{{cookiecutter.package_name}}.svg)](https://badge.fury.io/js/{{cookiecutter.package_name}})
[![Build Status](https://travis-ci.org/rrwen/{{cookiecutter.github_short}}.svg?branch=master)](https://travis-ci.org/{{cookiecutter.github_short}})
[![Coverage Status](https://coveralls.io/repos/github/{{cookiecutter.github_short}}/badge.svg?branch=master)](https://coveralls.io/github/{{cookiecutter.github_short}}?branch=master)
[![npm](https://img.shields.io/npm/dt/{{cookiecutter.package_name}}.svg)](https://www.npmjs.com/package/{{cookiecutter.package_name}})
[![GitHub license](https://img.shields.io/github/license/{{cookiecutter.github_short}}.svg)](https://github.com/{{cookiecutter.github_short}}/blob/master/LICENSE)
[![Twitter](https://img.shields.io/twitter/url/https/github.com/{{cookiecutter.github_short}}.svg?style=social)](https://twitter.com/intent/tweet?text={{cookiecutter.package_description.replace(' ','%20')}}:%20https%3A%2F%2Fgithub.com%2F{{cookiecutter.github.split('/')[0]}}%2F{{cookiecutter.package_name}}%20%23nodejs%20%23npm)

## Install

1. Install [Node.js](https://nodejs.org/en/)
2. Install [{{cookiecutter.package_name}}](https://www.npmjs.com/package/{{cookiecutter.package_name}}) via `npm`

```
npm install --save {{cookiecutter.package_name}}
```

For the latest developer version, see [Developer Install](#developer-install).

## Usage

An example usage of {{cookiecutter.package_name}}:

```
example
```

## Developer Notes

### Developer Install

Install the latest developer version with `npm` from github:

```
npm install git+{{cookiecutter.github_url}}
```
  
Install from `git` cloned source:

1. Ensure [git](https://git-scm.com/) is installed
2. Clone into current path
3. Install via `npm`

```
git clone {{cookiecutter.github_url}}
cd {{cookiecutter.package_name}}
npm install
```

### Tests

1. Clone into current path `git clone {{cookiecutter.github_url}}`
2. Enter into folder `cd {{cookiecutter.package_name}}`
3. Ensure [tape](https://www.npmjs.com/package/tape) and [moment](https://www.npmjs.com/package/moment) are available
4. Run tests
5. Results are saved to `./tests/log` with each file corresponding to a version tested

```
npm install
npm test
```

### Upload to Github

1. Ensure [git](https://git-scm.com/) is installed
2. Inside the `{{cookiecutter.package_name}}` folder, add all files and commit changes
3. Push to github

```
git add .
git commit -a -m "Generic update"
git push
```

### Upload to npm

1. Update the version in `package.json`
2. Run tests and check for OK status
3. Login to npm
4. Publish to npm

```
npm test
npm login
npm publish
```

### Implementation

A description of the overall implementation of {{cookiecutter.package_name}}.

```
component   <-- detail
        |
component   <-- detail
        |
component   <-- detail
        |
component   <-- detail
```
