Template for [dum](//dum-build.org) web projects.
Just `git clone https://github.com/dum-build/dum-web-template.git` and run!


## Run

(You might want to keep this section in your own `README.md`)

Requires [node.js](//nodejs.org).

	npm install -g bower
	bower install
	npm install
	npm start

Then see <http://localhost:8000>.


## Modify the template

### Libraries

Add new entries to `bower.json` and run `bower install`.
You may also want to modify the [require.js](https://requirejs.org) paths in `_layout.jade`.


### Scripting language

#### [Mason](//mason-lang.org)

In `package.json`, replace `"jstransformer-babel": ""` with `"jstransformer-mason": "mason-lang/jstransformer-mason"`.

Add `"msl": "mason-lang/msl"` to `bower.json` dependencies and run `bower install`.

In `_layout.jade`, add `msl: 'msl/dist'` to `paths`.


#### [CoffeeScript](//coffeescript.org)

In `package.json`, replace `"jstransformer-babel": ""` with `"jstransformer-coffee-script": ""`.


#### JavaScript

Just remove `"jstransformer-babel": ""` from `package.json` and use the `.js` extension.