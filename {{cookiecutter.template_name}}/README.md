# {{cookiecutter.template_name}}

{{cookiecutter.author}}  
{{cookiecutter.email}}  

* [Documentation](https://{{cookiecutter.github_user}}.github.io/{{cookiecutter.template_name}})

{{cookiecutter.template_description}}

[![npm version](https://badge.fury.io/js/{{cookiecutter.template_name}}.svg)](https://badge.fury.io/js/{{cookiecutter.template_name}})
[![Build Status](https://travis-ci.org/{{cookiecutter.github_short}}.svg?branch=master)](https://travis-ci.org/{{cookiecutter.github_short}})
[![Coverage Status](https://coveralls.io/repos/github/{{cookiecutter.github_short}}/badge.svg?branch=master)](https://coveralls.io/github/{{cookiecutter.github_short}}?branch=master)
[![npm](https://img.shields.io/npm/dt/{{cookiecutter.template_name}}.svg)](https://www.npmjs.com/package/{{cookiecutter.template_name}})
[![GitHub license](https://img.shields.io/github/license/{{cookiecutter.github_short}}.svg)](https://github.com/{{cookiecutter.github_short}}/blob/master/LICENSE)
[![Donate](https://img.shields.io/badge/donate-{{cookiecutter.donate_name}}-yellow.svg)]({{cookiecutter.donate_url}})
[![Twitter](https://img.shields.io/twitter/url/https/github.com/{{cookiecutter.github_short}}.svg?style=social)](https://twitter.com/intent/tweet?text={{cookiecutter.template_description.replace(' ','%20')}}:%20https%3A%2F%2Fgithub.com%2F{{cookiecutter.github_user}}%2F{{cookiecutter.template_name}}%20%23nodejs%20%23npm)

## Install

1. Install [Node.js](https://nodejs.org/en/)
2. Install [{{cookiecutter.template_name}}](https://www.npmjs.com/package/{{cookiecutter.template_name}}) via `npm`

```
npm install --save {{cookiecutter.template_name}}
```

For the latest developer version, see [Developer Install](#developer-install).

## Usage

An example usage of {{cookiecutter.template_name}}:

```javascript
var {{cookiecutter.template_name.replace('-', '').replace(' ', '')}} = require('{{cookiecutter.template_name}}');
```

See [Documentation](https://{{cookiecutter.github_user}}.github.io/{{cookiecutter.template_name}}) for more details.


## Contributions

1. Reports for issues and suggestions can be made using the [issue submission]({{cookiecutter.github_url}}/issues) interface.
2. Code contributions are submitted via [pull requests]({{cookiecutter.github_url}}/pulls)

See [CONTRIBUTING.md](CONTRIBUTING.md) for more details.

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
cd {{cookiecutter.template_name}}
npm install
```

### Tests

1. Clone into current path `git clone {{cookiecutter.github_url}}`
2. Enter into folder `cd {{cookiecutter.template_name}}`
3. Ensure [devDependencies](https://docs.npmjs.com/files/package.json#devdependencies) are installed and available
4. Run tests
5. Results are saved to [tests/log](tests/log) with each file corresponding to a version tested

```
npm install
npm test
```

### Documentation

Use [documentationjs](https://www.npmjs.com/package/documentation) to generate html documentation in the `docs` folder:

```
npm run docs
```

See [JSDoc style](http://usejsdoc.org/) for formatting syntax.

### Upload to Github

1. Ensure [git](https://git-scm.com/) is installed
2. Inside the `{{cookiecutter.template_name}}` folder, add all files and commit changes
3. Push to github

```
git add .
git commit -a -m "Generic update"
git push
```

### Upload to npm

1. Update the version in `package.json`
2. Run tests and check for OK status
3. Generate documentation
4. Login to npm
5. Publish to npm

```
npm test
npm run docs
npm login
npm publish
```

### Implementation

The module [{{cookiecutter.template_name}}](https://www.npmjs.com/package/{{cookiecutter.template_name}}) uses the following npm packages for its implementation:

npm | Purpose
--- | ---
component | description
component | description
component | description
component | description

```
component   <-- detail
    |
component   <-- detail
    |
component   <-- detail
    |
component   <-- detail
```
