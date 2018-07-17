gitconfig
==========

<!---
This file is generated by ape-tmpl. Do not update manually.
--->

<!-- Badge Start -->
<a name="badges"></a>

[![Build Status][bd_travis_shield_url]][bd_travis_url]
[![Code Climate][bd_codeclimate_shield_url]][bd_codeclimate_url]
[![Code Coverage][bd_codeclimate_coverage_shield_url]][bd_codeclimate_url]
[![npm Version][bd_npm_shield_url]][bd_npm_url]
[![JS Standard][bd_standard_shield_url]][bd_standard_url]

[bd_repo_url]: https://github.com/okunishinishi/node-gitconfig
[bd_travis_url]: http://travis-ci.org/okunishinishi/node-gitconfig
[bd_travis_shield_url]: http://img.shields.io/travis/okunishinishi/node-gitconfig.svg?style=flat
[bd_travis_com_url]: http://travis-ci.com/okunishinishi/node-gitconfig
[bd_travis_com_shield_url]: https://api.travis-ci.com/okunishinishi/node-gitconfig.svg?token=
[bd_license_url]: https://github.com/okunishinishi/node-gitconfig/blob/master/LICENSE
[bd_codeclimate_url]: http://codeclimate.com/github/okunishinishi/node-gitconfig
[bd_codeclimate_shield_url]: http://img.shields.io/codeclimate/github/okunishinishi/node-gitconfig.svg?style=flat
[bd_codeclimate_coverage_shield_url]: http://img.shields.io/codeclimate/coverage/github/okunishinishi/node-gitconfig.svg?style=flat
[bd_gemnasium_url]: https://gemnasium.com/okunishinishi/node-gitconfig
[bd_gemnasium_shield_url]: https://gemnasium.com/okunishinishi/node-gitconfig.svg
[bd_npm_url]: http://www.npmjs.org/package/gitconfig
[bd_npm_shield_url]: http://img.shields.io/npm/v/gitconfig.svg?style=flat
[bd_standard_url]: http://standardjs.com/
[bd_standard_shield_url]: https://img.shields.io/badge/code%20style-standard-brightgreen.svg

<!-- Badge End -->


<!-- Description Start -->
<a name="description"></a>

Run git config command.   
Based on [okunishinishi/node-gitconfig](https://github.com/okunishinishi/node-gitconfig)

<!-- Description End -->


<!-- Overview Start -->
<a name="overview"></a>



<!-- Overview End -->


<!-- Sections Start -->
<a name="sections"></a>

<!-- Section from "doc/guides/01.Installation.md.hbs" Start -->

<a name="section-doc-guides-01-installation-md"></a>

Installation
-----

```bash
npm install gitconfig --save
```


<!-- Section from "doc/guides/01.Installation.md.hbs" End -->

<!-- Section from "doc/guides/02.Usage.md.hbs" Start -->

<a name="section-doc-guides-02-usage-md"></a>

Usage
---------

```javascript
'use strict'

const gitconfig = require('@teambit/gitconfig')

// Set git config values.
gitconfig.set({
  'user.mail': 'foo@example.com'
}, {
  location: 'local'
}).then(() => {
  /* ... */
})

// Unset git config values.
gitconfig.unset([ 'user.mail' ], {
  location: 'local'
}).then(() => {
  /* ... */
})

// Git all config values.
gitconfig.get({
  location: 'global'
}).then((config) => {
  /* ... */
})

// Get git origin url.
gitconfig.getUrl().then((config) => {
  /* ... */
})
```



<!-- Section from "doc/guides/02.Usage.md.hbs" End -->

<!-- Section from "doc/guides/03.API.md.hbs" Start -->

<a name="section-doc-guides-03-a-p-i-md"></a>

API
---

| Signature | Description |
| --------- | ----------- |
| gitconfig.get(options, callback) | Get all git config. |
| gitconfig.get(key, options, callback) | Get config with key. |
| gitconfig.set(key, val, options, callback) | Set a config value. |
| gitconfig.set(values, options, callback) | Set mutliple config values. |
| gitconfig.unset(keys, options, callback) | Un set config value(s). |


Options
-------

| Name | Description |
| ---- | ----- |
| location | Config file location. (global, system, or local) |



<!-- Section from "doc/guides/03.API.md.hbs" End -->


<!-- Sections Start -->


<!-- LICENSE Start -->
<a name="license"></a>

License
-------
This software is released under the [MIT License](https://github.com/okunishinishi/node-gitconfig/blob/master/LICENSE).

<!-- LICENSE End -->


<!-- Links Start -->
<a name="links"></a>

Links
------

+ [git-config][git_config_url]

[git_config_url]: https://git-scm.com/docs/git-config

<!-- Links End -->
