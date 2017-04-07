# api documentation for  [schema-inspector (v1.6.8)](http://atinux.github.io/schema-inspector/)  [![npm package](https://img.shields.io/npm/v/npmdoc-schema-inspector.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-schema-inspector) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-schema-inspector.svg)](https://travis-ci.org/npmdoc/node-npmdoc-schema-inspector)
#### Schema-Inspector is a powerful tool to sanitize and validate JS objects.

[![NPM](https://nodei.co/npm/schema-inspector.png?downloads=true)](https://www.npmjs.com/package/schema-inspector)

[![apidoc](https://npmdoc.github.io/node-npmdoc-schema-inspector/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-schema-inspector_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-schema-inspector/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-schema-inspector/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-schema-inspector/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Sebastien Chopin",
        "url": "https://twitter.com/atinux"
    },
    "bugs": {
        "url": "https://github.com/Atinux/schema-inspector/issues"
    },
    "dependencies": {
        "async": "^1.5.0"
    },
    "description": "Schema-Inspector is a powerful tool to sanitize and validate JS objects.",
    "devDependencies": {
        "mocha": "^2.3.3",
        "should": "^7.1.1"
    },
    "directories": {},
    "dist": {
        "shasum": "b9e53983cc55ff2dbd7b65e3dbe085d9d1285f2a",
        "tarball": "https://registry.npmjs.org/schema-inspector/-/schema-inspector-1.6.8.tgz"
    },
    "gitHead": "66464e8659923401886a624d20e315b2898d888f",
    "homepage": "http://atinux.github.io/schema-inspector/",
    "keywords": [
        "validation",
        "sanitization",
        "inspector",
        "validator",
        "json",
        "validate",
        "sanitize"
    ],
    "licenses": [
        {
            "type": "MIT",
            "url": "https://github.com/Atinux/schema-inspector/raw/master/LICENSE"
        }
    ],
    "main": "index.js",
    "maintainers": [
        {
            "name": "atinux",
            "email": "atinux@gmail.com"
        }
    ],
    "name": "schema-inspector",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/Atinux/schema-inspector.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "1.6.8"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module schema-inspector](#apidoc.module.schema-inspector)
1.  [function <span class="apidocSignatureSpan">schema-inspector.</span>Sanitization (schema, custom)](#apidoc.element.schema-inspector.Sanitization)
1.  [function <span class="apidocSignatureSpan">schema-inspector.</span>Validation (schema, custom)](#apidoc.element.schema-inspector.Validation)
1.  [function <span class="apidocSignatureSpan">schema-inspector.</span>generate (schema, n)](#apidoc.element.schema-inspector.generate)
1.  [function <span class="apidocSignatureSpan">schema-inspector.</span>newSanitization (schema, custom)](#apidoc.element.schema-inspector.newSanitization)
1.  [function <span class="apidocSignatureSpan">schema-inspector.</span>newValidation (schema, custom)](#apidoc.element.schema-inspector.newValidation)
1.  [function <span class="apidocSignatureSpan">schema-inspector.</span>sanitize (schema, post, custom, callback)](#apidoc.element.schema-inspector.sanitize)
1.  [function <span class="apidocSignatureSpan">schema-inspector.</span>validate (schema, candidate, custom, callback)](#apidoc.element.schema-inspector.validate)
1.  object <span class="apidocSignatureSpan">schema-inspector.</span>Sanitization.prototype
1.  object <span class="apidocSignatureSpan">schema-inspector.</span>Validation.custom
1.  object <span class="apidocSignatureSpan">schema-inspector.</span>Validation.prototype

#### [module schema-inspector.Sanitization](#apidoc.module.schema-inspector.Sanitization)
1.  [function <span class="apidocSignatureSpan">schema-inspector.</span>Sanitization (schema, custom)](#apidoc.element.schema-inspector.Sanitization.Sanitization)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.</span>extend (custom)](#apidoc.element.schema-inspector.Sanitization.extend)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.</span>remove (fields)](#apidoc.element.schema-inspector.Sanitization.remove)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.</span>reset ()](#apidoc.element.schema-inspector.Sanitization.reset)
1.  object <span class="apidocSignatureSpan">schema-inspector.Sanitization.</span>custom

#### [module schema-inspector.Sanitization.prototype](#apidoc.module.schema-inspector.Sanitization.prototype)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>_asyncSanitize (schema, post, callback)](#apidoc.element.schema-inspector.Sanitization.prototype._asyncSanitize)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>_sanitize (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype._sanitize)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>asyncExec (schema, post, callback)](#apidoc.element.schema-inspector.Sanitization.prototype.asyncExec)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>asyncItems (schema, post, callback)](#apidoc.element.schema-inspector.Sanitization.prototype.asyncItems)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>asyncProperties (schema, post, callback)](#apidoc.element.schema-inspector.Sanitization.prototype.asyncProperties)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>exec (schema, post, callback)](#apidoc.element.schema-inspector.Sanitization.prototype.exec)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>items (schema, post, callback)](#apidoc.element.schema-inspector.Sanitization.prototype.items)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>max (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype.max)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>maxLength (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype.maxLength)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>min (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype.min)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>minLength (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype.minLength)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>optional (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype.optional)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>properties (schema, post, callback)](#apidoc.element.schema-inspector.Sanitization.prototype.properties)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>rules (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype.rules)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>sanitize (post, callback)](#apidoc.element.schema-inspector.Sanitization.prototype.sanitize)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>strict (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype.strict)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>type (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype.type)

#### [module schema-inspector.Validation](#apidoc.module.schema-inspector.Validation)
1.  [function <span class="apidocSignatureSpan">schema-inspector.</span>Validation (schema, custom)](#apidoc.element.schema-inspector.Validation.Validation)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.</span>extend (custom)](#apidoc.element.schema-inspector.Validation.extend)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.</span>remove (fields)](#apidoc.element.schema-inspector.Validation.remove)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.</span>reset ()](#apidoc.element.schema-inspector.Validation.reset)
1.  object <span class="apidocSignatureSpan">schema-inspector.Validation.</span>custom

#### [module schema-inspector.Validation.custom](#apidoc.module.schema-inspector.Validation.custom)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.custom.</span>type (schema, candidate)](#apidoc.element.schema-inspector.Validation.custom.type)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.custom.</span>unique (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.custom.unique)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.custom.</span>validDate (schema, date)](#apidoc.element.schema-inspector.Validation.custom.validDate)

#### [module schema-inspector.Validation.prototype](#apidoc.module.schema-inspector.Validation.prototype)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>_asyncValidate (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype._asyncValidate)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>_validate (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype._validate)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>asyncExec (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype.asyncExec)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>asyncItems (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype.asyncItems)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>asyncProperties (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype.asyncProperties)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>eq (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.eq)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>exactLength (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.exactLength)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>exec (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype.exec)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>gt (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.gt)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>gte (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.gte)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>items (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype.items)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>lt (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.lt)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>lte (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.lte)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>maxLength (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.maxLength)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>minLength (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.minLength)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>ne (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.ne)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>optional (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.optional)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>pattern (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.pattern)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>properties (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype.properties)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>someKeys (schema, candidat)](#apidoc.element.schema-inspector.Validation.prototype.someKeys)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>strict (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.strict)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>type (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.type)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>uniqueness (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.uniqueness)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>validDate (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.validDate)
1.  [function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>validate (candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype.validate)



# <a name="apidoc.module.schema-inspector"></a>[module schema-inspector](#apidoc.module.schema-inspector)

#### <a name="apidoc.element.schema-inspector.Sanitization"></a>[function <span class="apidocSignatureSpan">schema-inspector.</span>Sanitization (schema, custom)](#apidoc.element.schema-inspector.Sanitization)
- description and source-code
```javascript
function Sanitization(schema, custom) {
		Inspection.prototype.constructor.call(this, schema, _merge(Sanitization.custom, custom));
		var _reporting = [];

		this._basicFields = Object.keys(_sanitizationAttribut);
		this._customFields = Object.keys(this._custom);
		this.origin = null;

		this.report = function (message) {
			var newNot = {
					message: message || 'was sanitized',
					property: this.userAlias ? (this.userAlias + ' (' + this._dumpStack() + ')') : this._dumpStack()
			};
			if (!_reporting.some(function (e) { return e.property === newNot.property; })) {
				_reporting.push(newNot);
			}
		};

		this.result = function (data) {
			return {
				data: data,
				reporting: _reporting,
				format: function () {
					return this.reporting.map(function (i) {
						return 'Property ' + i.property + ' ' + i.message;
					}).join('\n');
				}
			};
		};
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation"></a>[function <span class="apidocSignatureSpan">schema-inspector.</span>Validation (schema, custom)](#apidoc.element.schema-inspector.Validation)
- description and source-code
```javascript
function Validation(schema, custom) {
		Inspection.prototype.constructor.call(this, schema, _merge(Validation.custom, custom));
		var _error = [];

		this._basicFields = Object.keys(_validationAttribut);
		this._customFields = Object.keys(this._custom);
		this.origin = null;

		this.report = function (message, code, reason) {
			var newErr = {
				code: code || this.userCode || null,
				reason: reason || 'unknown',
				message: this.userError || message || 'is invalid',
				property: this.userAlias ? (this.userAlias + ' (' + this._dumpStack() + ')') : this._dumpStack()
			};
			_error.push(newErr);
			return this;
		};

		this.result = function () {
			return {
				error: _error,
				valid: _error.length === 0,
				format: function () {
					if (this.valid === true) {
						return 'Candidate is valid';
					}
					return this.error.map(function (i) {
						return 'Property ' + i.property + ': ' + i.message;
					}).join('\n');
				}
			};
		};
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.generate"></a>[function <span class="apidocSignatureSpan">schema-inspector.</span>generate (schema, n)](#apidoc.element.schema-inspector.generate)
- description and source-code
```javascript
generate = function (schema, n) {
		if (typeof n === 'number') {
			var r = new Array(n);
			for (var i = 0; i < n; i++) {
				r[i] = CandidateGenerator.instance().generate(schema);
			}
			return r;
		}
		return CandidateGenerator.instance().generate(schema);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.newSanitization"></a>[function <span class="apidocSignatureSpan">schema-inspector.</span>newSanitization (schema, custom)](#apidoc.element.schema-inspector.newSanitization)
- description and source-code
```javascript
newSanitization = function (schema, custom) {
		return new Sanitization(schema, custom);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.newValidation"></a>[function <span class="apidocSignatureSpan">schema-inspector.</span>newValidation (schema, custom)](#apidoc.element.schema-inspector.newValidation)
- description and source-code
```javascript
newValidation = function (schema, custom) {
		return new Validation(schema, custom);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.sanitize"></a>[function <span class="apidocSignatureSpan">schema-inspector.</span>sanitize (schema, post, custom, callback)](#apidoc.element.schema-inspector.sanitize)
- description and source-code
```javascript
sanitize = function (schema, post, custom, callback) {
		if (arguments.length === 3 && typeof custom === 'function') {
			callback = custom;
			custom = null;
		}
		return new Sanitization(schema, custom).sanitize(post, callback);
	}
```
- example usage
```shell
...
			splitWith: ',',
			items: { type: 'string', rules: ['trim', 'title'] }
		},
		email: { type: 'string', rules: ['trim', 'lower'] }
	}
};
// Let's update the data
inspector.sanitize(sanitization, data);
/*
data is now:
{
	firstname: 'Sterling',
	lastname: 'Archer',
	jobs: ['Special Agent', 'Cocaine Dealer'],
	email: 'never!'
...
```

#### <a name="apidoc.element.schema-inspector.validate"></a>[function <span class="apidocSignatureSpan">schema-inspector.</span>validate (schema, candidate, custom, callback)](#apidoc.element.schema-inspector.validate)
- description and source-code
```javascript
validate = function (schema, candidate, custom, callback) {
		if (arguments.length === 3 && typeof custom === 'function') {
			callback = custom;
			custom = null;
		}
		return new Validation(schema, custom).validate(candidate, callback);
	}
```
- example usage
```shell
...
		jobs: {
			type: 'array',
			items: { type: 'string', minLength: 1 }
		},
		email: { type: 'string', pattern: 'email' }
	}
};
var result = inspector.validate(validation, data);
if (!result.valid)
	console.log(result.format());
/*
	Property @.email: must match [email], but is equal to "never!"
*/
'''
...
```



# <a name="apidoc.module.schema-inspector.Sanitization"></a>[module schema-inspector.Sanitization](#apidoc.module.schema-inspector.Sanitization)

#### <a name="apidoc.element.schema-inspector.Sanitization.Sanitization"></a>[function <span class="apidocSignatureSpan">schema-inspector.</span>Sanitization (schema, custom)](#apidoc.element.schema-inspector.Sanitization.Sanitization)
- description and source-code
```javascript
function Sanitization(schema, custom) {
		Inspection.prototype.constructor.call(this, schema, _merge(Sanitization.custom, custom));
		var _reporting = [];

		this._basicFields = Object.keys(_sanitizationAttribut);
		this._customFields = Object.keys(this._custom);
		this.origin = null;

		this.report = function (message) {
			var newNot = {
					message: message || 'was sanitized',
					property: this.userAlias ? (this.userAlias + ' (' + this._dumpStack() + ')') : this._dumpStack()
			};
			if (!_reporting.some(function (e) { return e.property === newNot.property; })) {
				_reporting.push(newNot);
			}
		};

		this.result = function (data) {
			return {
				data: data,
				reporting: _reporting,
				format: function () {
					return this.reporting.map(function (i) {
						return 'Property ' + i.property + ' ' + i.message;
					}).join('\n');
				}
			};
		};
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Sanitization.extend"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.</span>extend (custom)](#apidoc.element.schema-inspector.Sanitization.extend)
- description and source-code
```javascript
extend = function (custom) {
			return _extend(this.custom, custom);
		}
```
- example usage
```shell
...
---------------------------------------

<a name="cf_extension" />
### extension

Sometime you want to use a custom field everywhere in your program, so you may
extend Schema-Inspector to do so. Just call the method
_inspector.Validation.extend(customFieldObject)_ or
_inspector.Sanitization.extend(customFieldObject)_. If you want to reset, simply call
_inspector.Validation.reset()_ or _inspector.Sanitization.reset()_. You also can remove a
specific field by calling _inspector.Validation.remove(field)_ or
_inspector.Sanitization.remove(field)_.

__Example__
...
```

#### <a name="apidoc.element.schema-inspector.Sanitization.remove"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.</span>remove (fields)](#apidoc.element.schema-inspector.Sanitization.remove)
- description and source-code
```javascript
remove = function (fields) {
			if (!_typeIs.array(fields)) {
				fields = [fields];
			}
			fields.forEach(function (field) {
				delete this.custom[field];
			}, this);
		}
```
- example usage
```shell
...
### extension

Sometime you want to use a custom field everywhere in your program, so you may
extend Schema-Inspector to do so. Just call the method
_inspector.Validation.extend(customFieldObject)_ or
_inspector.Sanitization.extend(customFieldObject)_. If you want to reset, simply call
_inspector.Validation.reset()_ or _inspector.Sanitization.reset()_. You also can remove a
specific field by calling _inspector.Validation.remove(field)_ or
_inspector.Sanitization.remove(field)_.

__Example__

'''javascript
var inspector = require('schema-inspector');
...
```

#### <a name="apidoc.element.schema-inspector.Sanitization.reset"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.</span>reset ()](#apidoc.element.schema-inspector.Sanitization.reset)
- description and source-code
```javascript
reset = function () {
			this.custom = {};
		}
```
- example usage
```shell
...
<a name="cf_extension" />
### extension

Sometime you want to use a custom field everywhere in your program, so you may
extend Schema-Inspector to do so. Just call the method
_inspector.Validation.extend(customFieldObject)_ or
_inspector.Sanitization.extend(customFieldObject)_. If you want to reset, simply call
_inspector.Validation.reset()_ or _inspector.Sanitization.reset()_. You also can remove a
specific field by calling _inspector.Validation.remove(field)_ or
_inspector.Sanitization.remove(field)_.

__Example__

'''javascript
var inspector = require('schema-inspector');
...
```



# <a name="apidoc.module.schema-inspector.Sanitization.prototype"></a>[module schema-inspector.Sanitization.prototype](#apidoc.module.schema-inspector.Sanitization.prototype)

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype._asyncSanitize"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>_asyncSanitize (schema, post, callback)](#apidoc.element.schema-inspector.Sanitization.prototype._asyncSanitize)
- description and source-code
```javascript
_asyncSanitize = function (schema, post, callback) {
		var self = this;
		this.userAlias = schema.alias || null;

		async.waterfall([
			function (next) {
				async.reduce(self._basicFields, post, function (value, i, next) {
					async.nextTick(function () {
						if ((i in schema || i === 'optional') && typeof self[i] === 'function') {
							if (self[i].length > 2) {
								return self[i](schema, value, next);
							}
							value = self[i](schema, value);
						}
						next(null, value);
					});
				}, next);
			},
			function (inter, next) {
				async.reduce(self._customFields, inter, function (value, i, next) {
					async.nextTick(function () {
						if (i in schema && typeof self._custom[i] === 'function') {
							if (self._custom[i].length > 2) {
								return self._custom[i].call(self, schema, value, next);
							}
							value = self._custom[i].call(self, schema, value);
						}
						next(null, value);
					});
				}, next);
			}
		], callback);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype._sanitize"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>_sanitize (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype._sanitize)
- description and source-code
```javascript
_sanitize = function (schema, post) {
		this.userAlias = schema.alias || null;
		this._basicFields.forEach(function (i) {
			if ((i in schema || i === 'optional') && typeof this[i] === 'function') {
				post = this[i](schema, post);
			}
		}, this);
		this._customFields.forEach(function (i) {
			if (i in schema && typeof this._custom[i] === 'function') {
				post = this._custom[i].call(this, schema, post);
			}
		}, this);
		return post;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype.asyncExec"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>asyncExec (schema, post, callback)](#apidoc.element.schema-inspector.Sanitization.prototype.asyncExec)
- description and source-code
```javascript
asyncExec = function (schema, post, callback) {
			var self = this;
			var execs = _typeIs.array(schema.exec) ? schema.exec : [schema.exec];

			async.eachSeries(execs, function (exec, done) {
				if (typeof exec === 'function') {
					if (exec.length > 2) {
						return exec.call(self, schema, post, function (err, res) {
							if (err) {
								return done(err);
							}
							post = res;
							done();
						});
					}
					post = exec.call(self, schema, post);
				}
				done();
			}, function (err) {
				callback(err, post);
			});
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype.asyncItems"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>asyncItems (schema, post, callback)](#apidoc.element.schema-inspector.Sanitization.prototype.asyncItems)
- description and source-code
```javascript
asyncItems = function (schema, post, callback) {
			if (!(schema.items instanceof Object) || !(post instanceof Object)) {
				return callback(null, post);
			}
			var self = this;
			var items = schema.items;
			if (_typeIs.array(items) && _typeIs.array(post)) {
				var minLength = items.length < post.length ? items.length : post.length;
				async.timesSeries(minLength, function (i, next) {
					self._deeperArray(i);
					self._asyncSanitize(items[i], post[i], function (err, res) {
						if (err) {
							return next(err);
						}
						post[i] = res;
						self._back();
						next();
					});
				}, function (err) {
					callback(err, post);
				});
			}
			else {
				async.eachSeries(Object.keys(post), function (key, next) {
					self._deeperArray(key);
					self._asyncSanitize(items, post[key], function (err, res) {
						if (err) {
							return next();
						}
						post[key] = res;
						self._back();
						next();
					});
				}, function (err) {
					callback(err, post);
				});
			}
			return post;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype.asyncProperties"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>asyncProperties (schema, post, callback)](#apidoc.element.schema-inspector.Sanitization.prototype.asyncProperties)
- description and source-code
```javascript
asyncProperties = function (schema, post, callback) {
			if (!post || typeof post !== 'object') {
				return callback(null, post);
			}
			var self = this;
			var properties = schema.properties;

			async.series([
				function (next) {
					if (properties['*'] == null) {
						return next();
					}
					var globing = properties['*'];
					async.eachSeries(Object.keys(post), function (i, next) {
						if (i in properties) {
							return next();
						}
						self._deeperObject(i);
						self._asyncSanitize(globing, post[i], function (err, res) {
							if (err) { /* Error can safely be ignored here */ }
							if (typeof res !== 'undefined') {
								post[i] = res;
							}
							self._back();
							next();
						});
					}, next);
				},
				function (next) {
					async.eachSeries(Object.keys(properties), function (i, next) {
						if (i === '*') {
							return next();
						}
						self._deeperObject(i);
						self._asyncSanitize(properties[i], post[i], function (err, res) {
							if (err) {
								return next(err);
							}
							if (typeof res !== 'undefined') {
								post[i] = res;
							}
							self._back();
							next();
						});
					}, next);
				}
			], function (err) {
				return callback(err, post);
			});
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype.exec"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>exec (schema, post, callback)](#apidoc.element.schema-inspector.Sanitization.prototype.exec)
- description and source-code
```javascript
exec = function (schema, post, callback) {
			if (typeof callback === 'function') {
				return this.asyncExec(schema, post, callback);
			}
			var execs = _typeIs.array(schema.exec) ? schema.exec : [schema.exec];

			execs.forEach(function (exec) {
				if (typeof exec === 'function') {
					post = exec.call(this, schema, post);
				}
			}, this);
			return post;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype.items"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>items (schema, post, callback)](#apidoc.element.schema-inspector.Sanitization.prototype.items)
- description and source-code
```javascript
items = function (schema, post, callback) {
			if (typeof callback === 'function') {
				return this.asyncItems(schema, post, callback);
			}
			if (!(schema.items instanceof Object) || !(post instanceof Object)) {
				return post;
			}
			var i;
			if (_typeIs.array(schema.items) && _typeIs.array(post)) {
				var minLength = schema.items.length < post.length ? schema.items.length : post.length;
				for (i = 0; i < minLength; i++) {
					this._deeperArray(i);
					post[i] = this._sanitize(schema.items[i], post[i]);
					this._back();
				}
			}
			else {
				for (i in post) {
					if(post.hasOwnProperty(i)){
						this._deeperArray(i);
						post[i] = this._sanitize(schema.items, post[i]);
						this._back();
					}
				}
			}
			return post;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype.max"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>max (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype.max)
- description and source-code
```javascript
max = function (schema, post) {
			var postTest = Number(post);
			if (isNaN(postTest)) {
				return post;
			}
			var max = Number(schema.max);
			if (isNaN(max)) {
				return post;
			}
			if (postTest > max) {
				this.report();
				return max;
			}
			return post;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype.maxLength"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>maxLength (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype.maxLength)
- description and source-code
```javascript
maxLength = function (schema, post) {
			var limit = Number(schema.maxLength);
			if (typeof post !== 'string' || isNaN(limit) || limit < 0) {
				return post;
			}
			if (post.length > limit) {
				this.report();
				return post.slice(0, limit);
			}
			return post;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype.min"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>min (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype.min)
- description and source-code
```javascript
min = function (schema, post) {
			var postTest = Number(post);
			if (isNaN(postTest)) {
				return post;
			}
			var min = Number(schema.min);
			if (isNaN(min)) {
				return post;
			}
			if (postTest < min) {
				this.report();
				return min;
			}
			return post;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype.minLength"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>minLength (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype.minLength)
- description and source-code
```javascript
minLength = function (schema, post) {
			var limit = Number(schema.minLength);
			if (typeof post !== 'string' || isNaN(limit) || limit < 0) {
				return post;
			}
			var str = '';
			var gap = limit - post.length;
			if (gap > 0) {
				for (var i = 0; i < gap; i++) {
					str += '-';
				}
				this.report();
				return post + str;
			}
			return post;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype.optional"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>optional (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype.optional)
- description and source-code
```javascript
optional = function (schema, post) {
			var opt = typeof schema.optional === 'boolean' ? schema.optional : (schema.optional !== 'false'); // Default: true
			if (opt === true) {
				return post;
			}
			if (typeof post !== 'undefined') {
				return post;
			}
			this.report();
			if (schema.def === Date) {
				return new Date();
			}
			return schema.def;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype.properties"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>properties (schema, post, callback)](#apidoc.element.schema-inspector.Sanitization.prototype.properties)
- description and source-code
```javascript
properties = function (schema, post, callback) {
			if (typeof callback === 'function') {
				return this.asyncProperties(schema, post, callback);
			}
			if (!post || typeof post !== 'object') {
				return post;
			}
			var properties = schema.properties;
			var tmp;
			var i;
			if (typeof properties['*'] !== 'undefined') {
				for (i in post) {
					if (i in properties) {
						continue;
					}
					this._deeperObject(i);
					tmp = this._sanitize(schema.properties['*'], post[i]);
					if (typeof tmp !== 'undefined') {
						post[i]= tmp;
					}
					this._back();
				}
			}
			for (i in schema.properties) {
				if (i !== '*') {
					this._deeperObject(i);
					tmp = this._sanitize(schema.properties[i], post[i]);
					if (typeof tmp !== 'undefined') {
						post[i]= tmp;
					}
					this._back();
				}
			}
			return post;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype.rules"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>rules (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype.rules)
- description and source-code
```javascript
rules = function (schema, post) {
			var rules = schema.rules;
			if (typeof post !== 'string' || (typeof rules !== 'string' && !_typeIs.array(rules))) {
				return post;
			}
			var modified = false;
			(_typeIs.array(rules) ? rules : [rules]).forEach(function (rule) {
				if (typeof _applyRules[rule] === 'function') {
					post = _applyRules[rule](post);
					modified = true;
				}
			});
			if (modified) {
				this.report();
			}
			return post;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype.sanitize"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>sanitize (post, callback)](#apidoc.element.schema-inspector.Sanitization.prototype.sanitize)
- description and source-code
```javascript
sanitize = function (post, callback) {
		this.origin = post;
		if (typeof callback === 'function') {
			var self = this;
			return this._asyncSanitize(this._schema, post, function (err, data) {
				self.origin = null;
				callback(err, self.result(data));
			});
		}
		var data = this._sanitize(this._schema, post);
		this.origin = null;
		return this.result(data);
	}
```
- example usage
```shell
...
			splitWith: ',',
			items: { type: 'string', rules: ['trim', 'title'] }
		},
		email: { type: 'string', rules: ['trim', 'lower'] }
	}
};
// Let's update the data
inspector.sanitize(sanitization, data);
/*
data is now:
{
	firstname: 'Sterling',
	lastname: 'Archer',
	jobs: ['Special Agent', 'Cocaine Dealer'],
	email: 'never!'
...
```

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype.strict"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>strict (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype.strict)
- description and source-code
```javascript
strict = function (schema, post) {
			if (typeof schema.strict === 'string') { schema.strict = (schema.strict === 'true'); }
			if (schema.strict !== true)
				return post;
			if (!_typeIs.object(schema.properties))
				return post;
			if (!_typeIs.object(post))
				return post;
			var that = this;
			Object.keys(post).forEach(function (key) {
				if (!(key in schema.properties)) {
					delete post[key];
				}
			});
			return post;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Sanitization.prototype.type"></a>[function <span class="apidocSignatureSpan">schema-inspector.Sanitization.prototype.</span>type (schema, post)](#apidoc.element.schema-inspector.Sanitization.prototype.type)
- description and source-code
```javascript
type = function (schema, post) {
			// if (_typeIs['object'](post) || _typeIs.array(post)) {
			// 	return post;
			// }
			if (typeof schema.type !== 'string' || typeof _forceType[schema.type] !== 'function') {
				return post;
			}
			var n;
			var opt = typeof schema.optional === 'boolean' ? schema.optional : true;
			if (typeof _forceType[schema.type] === 'function') {
				n = _forceType[schema.type](post, schema);
				if ((n === null && !opt) || (!n && isNaN(n)) || (n === null && schema.type === 'string')) {
					n = schema.def;
				}
			}
			else if (!opt) {
				n = schema.def;
			}
			if ((n != null || (typeof schema.def !== 'undefined' && schema.def === n)) && n !== post) {
				this.report();
				return n;
			}
			return post;
		}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.schema-inspector.Validation"></a>[module schema-inspector.Validation](#apidoc.module.schema-inspector.Validation)

#### <a name="apidoc.element.schema-inspector.Validation.Validation"></a>[function <span class="apidocSignatureSpan">schema-inspector.</span>Validation (schema, custom)](#apidoc.element.schema-inspector.Validation.Validation)
- description and source-code
```javascript
function Validation(schema, custom) {
		Inspection.prototype.constructor.call(this, schema, _merge(Validation.custom, custom));
		var _error = [];

		this._basicFields = Object.keys(_validationAttribut);
		this._customFields = Object.keys(this._custom);
		this.origin = null;

		this.report = function (message, code, reason) {
			var newErr = {
				code: code || this.userCode || null,
				reason: reason || 'unknown',
				message: this.userError || message || 'is invalid',
				property: this.userAlias ? (this.userAlias + ' (' + this._dumpStack() + ')') : this._dumpStack()
			};
			_error.push(newErr);
			return this;
		};

		this.result = function () {
			return {
				error: _error,
				valid: _error.length === 0,
				format: function () {
					if (this.valid === true) {
						return 'Candidate is valid';
					}
					return this.error.map(function (i) {
						return 'Property ' + i.property + ': ' + i.message;
					}).join('\n');
				}
			};
		};
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.extend"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.</span>extend (custom)](#apidoc.element.schema-inspector.Validation.extend)
- description and source-code
```javascript
extend = function (custom) {
			return _extend(this.custom, custom);
		}
```
- example usage
```shell
...
---------------------------------------

<a name="cf_extension" />
### extension

Sometime you want to use a custom field everywhere in your program, so you may
extend Schema-Inspector to do so. Just call the method
_inspector.Validation.extend(customFieldObject)_ or
_inspector.Sanitization.extend(customFieldObject)_. If you want to reset, simply call
_inspector.Validation.reset()_ or _inspector.Sanitization.reset()_. You also can remove a
specific field by calling _inspector.Validation.remove(field)_ or
_inspector.Sanitization.remove(field)_.

__Example__
...
```

#### <a name="apidoc.element.schema-inspector.Validation.remove"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.</span>remove (fields)](#apidoc.element.schema-inspector.Validation.remove)
- description and source-code
```javascript
remove = function (fields) {
			if (!_typeIs.array(fields)) {
				fields = [fields];
			}
			fields.forEach(function (field) {
				delete this.custom[field];
			}, this);
		}
```
- example usage
```shell
...
### extension

Sometime you want to use a custom field everywhere in your program, so you may
extend Schema-Inspector to do so. Just call the method
_inspector.Validation.extend(customFieldObject)_ or
_inspector.Sanitization.extend(customFieldObject)_. If you want to reset, simply call
_inspector.Validation.reset()_ or _inspector.Sanitization.reset()_. You also can remove a
specific field by calling _inspector.Validation.remove(field)_ or
_inspector.Sanitization.remove(field)_.

__Example__

'''javascript
var inspector = require('schema-inspector');
...
```

#### <a name="apidoc.element.schema-inspector.Validation.reset"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.</span>reset ()](#apidoc.element.schema-inspector.Validation.reset)
- description and source-code
```javascript
reset = function () {
			this.custom = {};
		}
```
- example usage
```shell
...
<a name="cf_extension" />
### extension

Sometime you want to use a custom field everywhere in your program, so you may
extend Schema-Inspector to do so. Just call the method
_inspector.Validation.extend(customFieldObject)_ or
_inspector.Sanitization.extend(customFieldObject)_. If you want to reset, simply call
_inspector.Validation.reset()_ or _inspector.Sanitization.reset()_. You also can remove a
specific field by calling _inspector.Validation.remove(field)_ or
_inspector.Sanitization.remove(field)_.

__Example__

'''javascript
var inspector = require('schema-inspector');
...
```



# <a name="apidoc.module.schema-inspector.Validation.custom"></a>[module schema-inspector.Validation.custom](#apidoc.module.schema-inspector.Validation.custom)

#### <a name="apidoc.element.schema-inspector.Validation.custom.type"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.custom.</span>type (schema, candidate)](#apidoc.element.schema-inspector.Validation.custom.type)
- description and source-code
```javascript
type = function (schema, candidate) {
		var result;
		// Custom type
		if (schema.$type === 'person')
			result = inspector.validate(personValidation, candidate);
		// Basic type
		else
			result = inspector.validate({ type: schema.$type }, candidate);
		if (!result.valid)
			return this.report(result.format());
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.custom.unique"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.custom.</span>unique (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.custom.unique)
- description and source-code
```javascript
unique = function (schema, candidate, callback) {
		console.log(this.origin._connection);
    callback();
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.custom.validDate"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.custom.</span>validDate (schema, date)](#apidoc.element.schema-inspector.Validation.custom.validDate)
- description and source-code
```javascript
validDate = function (schema, date) {
    if (schema.$validDate === true
       && Object.prototype.toString.call(date) === "[object Date]"
       && isNaN(date.getTime())) {
        this.report('must be a valid date');
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.schema-inspector.Validation.prototype"></a>[module schema-inspector.Validation.prototype](#apidoc.module.schema-inspector.Validation.prototype)

#### <a name="apidoc.element.schema-inspector.Validation.prototype._asyncValidate"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>_asyncValidate (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype._asyncValidate)
- description and source-code
```javascript
_asyncValidate = function (schema, candidate, callback) {
		var self = this;
		this.userCode = schema.code || null;
		this.userError = schema.error || null;
		this.userAlias = schema.alias || null;

		async.series([
			function (next) {
				async.eachSeries(Object.keys(_validationAttribut), function (i, done) {
					async.nextTick(function () {
						if ((i in schema || i === 'optional') && typeof self[i] === 'function') {
							if (self[i].length > 2) {
								return self[i](schema, candidate, done);
							}
							self[i](schema, candidate);
						}
						done();
					});
				}, next);
			},
			function (next) {
				async.eachSeries(Object.keys(self._custom), function (i, done) {
					async.nextTick(function () {
						if (i in schema && typeof self._custom[i] === 'function') {
							if (self._custom[i].length > 2) {
								return self._custom[i].call(self, schema, candidate, done);
							}
							self._custom[i].call(self, schema, candidate);
						}
						done();
					});
				}, next);
			}
		], callback);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype._validate"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>_validate (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype._validate)
- description and source-code
```javascript
_validate = function (schema, candidate, callback) {
		this.userCode = schema.code || null;
		this.userError = schema.error || null;
		this.userAlias = schema.alias || null;
		this._basicFields.forEach(function (i) {
			if ((i in schema || i === 'optional') && typeof this[i] === 'function') {
				this[i](schema, candidate);
			}
		}, this);
		this._customFields.forEach(function (i) {
			if (i in schema && typeof this._custom[i] === 'function') {
				this._custom[i].call(this, schema, candidate);
			}
		}, this);
		return this;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.asyncExec"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>asyncExec (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype.asyncExec)
- description and source-code
```javascript
asyncExec = function (schema, candidate, callback) {
			var self = this;
			async.eachSeries(_typeIs.array(schema.exec) ? schema.exec : [schema.exec], function (exec, done) {
				if (typeof exec === 'function') {
					if (exec.length > 2) {
						return exec.call(self, schema, candidate, done);
					}
					exec.call(self, schema, candidate);
				}
				async.nextTick(done);
			}, callback);
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.asyncItems"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>asyncItems (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype.asyncItems)
- description and source-code
```javascript
asyncItems = function (schema, candidate, callback) {
			if (!(schema.items instanceof Object) || !(candidate instanceof Object)) {
				return callback();
			}
			var self = this;
			var items = schema.items;
			var i, l;

			if (_typeIs.array(items) && _typeIs.array(candidate)) {
				async.timesSeries(items.length, function (i, done) {
					self._deeperArray(i);
					self._asyncValidate(items[i], candidate[i], function (err, res) {
						self._back();
						done(err, res);
					});
					self._back();
				}, callback);
			}
			else {
				async.eachSeries(Object.keys(candidate), function (key, done) {
					self._deeperArray(key);
					self._asyncValidate(items, candidate[key], function (err, res) {
						self._back();
						done(err, res);
					});
				}, callback);
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.asyncProperties"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>asyncProperties (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype.asyncProperties)
- description and source-code
```javascript
asyncProperties = function (schema, candidate, callback) {
			if (!(schema.properties instanceof Object) || !_typeIs.object(candidate)) {
				return callback();
			}
			var self = this;
			var properties = schema.properties;
			async.series([
				function (next) {
					if (properties['*'] == null) {
						return next();
					}
					async.eachSeries(Object.keys(candidate), function (i, done) {
						if (i in properties) {
							return async.nextTick(done);
						}
						self._deeperObject(i);
						self._asyncValidate(properties['*'], candidate[i], function (err) {
							self._back();
							done(err);
						});
					}, next);
				},
				function (next) {
					async.eachSeries(Object.keys(properties), function (i, done) {
						if (i === '*') {
							return async.nextTick(done);
						}
						self._deeperObject(i);
						self._asyncValidate(properties[i], candidate[i], function (err) {
							self._back();
							done(err);
						});
					}, next);
				}
			], callback);
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.eq"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>eq (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.eq)
- description and source-code
```javascript
eq = function (schema, candidate) {
			if (typeof candidate !== 'number' && typeof candidate !== 'string' && typeof candidate !== 'boolean') {
				return;
			}
			var limit = schema.eq;
			if (typeof limit !== 'number' && typeof limit !== 'string' && typeof limit !== 'boolean' && !_typeIs.array(limit)) {
				return;
			}
			if (_typeIs.array(limit)) {
				for (var i = 0; i < limit.length; i++) {
					if (candidate === limit[i]) {
						return;
					}
				}
				this.report('must be equal to [' + limit.map(function (l) {
					return '"' + l + '"';
				}).join(' or ') + '], but is equal to "' + candidate + '"', null, 'eq');
			}
			else {
				if (candidate !== limit) {
					this.report('must be equal to "' + limit + '", but is equal to "' + candidate + '"', null, 'eq');
				}
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.exactLength"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>exactLength (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.exactLength)
- description and source-code
```javascript
exactLength = function (schema, candidate) {
			if (typeof candidate !== 'string' && !_typeIs.array(candidate)) {
				return;
			}
			var exactLength = Number(schema.exactLength);
			if (isNaN(exactLength)) {
				return;
			}
			if (candidate.length !== exactLength) {
				this.report('must have exactly ' + exactLength + ' elements, but it have ' + candidate.length, null, 'exactLength');
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.exec"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>exec (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype.exec)
- description and source-code
```javascript
exec = function (schema, candidate, callback) {
			var self = this;

			if (typeof callback === 'function') {
				return this.asyncExec(schema, candidate, callback);
			}
			(_typeIs.array(schema.exec) ? schema.exec : [schema.exec]).forEach(function (exec) {
				if (typeof exec === 'function') {
					exec.call(self, schema, candidate);
				}
			});
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.gt"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>gt (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.gt)
- description and source-code
```javascript
gt = function (schema, candidate) {
			var limit = Number(schema.gt);
			if (typeof candidate !== 'number' || isNaN(limit)) {
				return;
			}
			if (candidate <= limit) {
				this.report('must be greater than ' + limit + ', but is equal to "' + candidate + '"', null, 'gt');
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.gte"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>gte (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.gte)
- description and source-code
```javascript
gte = function (schema, candidate) {
			var limit = Number(schema.gte);
			if (typeof candidate !== 'number' || isNaN(limit)) {
				return;
			}
			if (candidate < limit) {
				this.report('must be greater than or equal to ' + limit + ', but is equal to "' + candidate + '"', null, 'gte');
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.items"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>items (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype.items)
- description and source-code
```javascript
items = function (schema, candidate, callback) {
			if (typeof callback === 'function') {
				return this.asyncItems(schema, candidate, callback);
			}
			if (!(schema.items instanceof Object) || !(candidate instanceof Object)) {
				return;
			}
			var items = schema.items;
			var i, l;
			// If provided schema is an array
			// then call validate for each case
			// else it is an Object
			// then call validate for each key
			if (_typeIs.array(items) && _typeIs.array(candidate)) {
				for (i = 0, l = items.length; i < l; i++) {
					this._deeperArray(i);
					this._validate(items[i], candidate[i]);
					this._back();
				}
			}
			else {
				for (var key in candidate) {
					if (candidate.hasOwnProperty(key)){
						this._deeperArray(key);
						this._validate(items, candidate[key]);
						this._back();
					}

				}
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.lt"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>lt (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.lt)
- description and source-code
```javascript
lt = function (schema, candidate) {
			var limit = Number(schema.lt);
			if (typeof candidate !== 'number' || isNaN(limit)) {
				return;
			}
			if (candidate >= limit) {
				this.report('must be less than ' + limit + ', but is equal to "' + candidate + '"', null, 'lt');
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.lte"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>lte (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.lte)
- description and source-code
```javascript
lte = function (schema, candidate) {
			var limit = Number(schema.lte);
			if (typeof candidate !== 'number' || isNaN(limit)) {
				return;
			}
			if (candidate > limit) {
				this.report('must be less than or equal to ' + limit + ', but is equal to "' + candidate + '"', null, 'lte');
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.maxLength"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>maxLength (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.maxLength)
- description and source-code
```javascript
maxLength = function (schema, candidate) {
			if (typeof candidate !== 'string' && !_typeIs.array(candidate)) {
				return;
			}
			var maxLength = Number(schema.maxLength);
			if (isNaN(maxLength)) {
				return;
			}
			if (candidate.length > maxLength) {
				this.report('must be shorter than ' + maxLength + ' elements, but it has ' + candidate.length, null, 'maxLength');
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.minLength"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>minLength (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.minLength)
- description and source-code
```javascript
minLength = function (schema, candidate) {
			if (typeof candidate !== 'string' && !_typeIs.array(candidate)) {
				return;
			}
			var minLength = Number(schema.minLength);
			if (isNaN(minLength)) {
				return;
			}
			if (candidate.length < minLength) {
				this.report('must be longer than ' + minLength + ' elements, but it has ' + candidate.length, null, 'minLength');
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.ne"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>ne (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.ne)
- description and source-code
```javascript
ne = function (schema, candidate) {
			if (typeof candidate !== 'number' && typeof candidate !== 'string') {
				return;
			}
			var limit = schema.ne;
			if (typeof limit !== 'number' && typeof limit !== 'string' && !_typeIs.array(limit)) {
				return;
			}
			if (_typeIs.array(limit)) {
				for (var i = 0; i < limit.length; i++) {
					if (candidate === limit[i]) {
						this.report('must not be equal to "' + limit[i] + '"', null, 'ne');
						return;
					}
				}
			}
			else {
				if (candidate === limit) {
					this.report('must not be equal to "' + limit + '"', null, 'ne');
				}
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.optional"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>optional (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.optional)
- description and source-code
```javascript
optional = function (schema, candidate) {
			var opt = typeof schema.optional === 'boolean' ? schema.optional : (schema.optional === 'true'); // Default is false

			if (opt === true) {
				return;
			}
			if (typeof candidate === 'undefined') {
				this.report('is missing and not optional', null, 'optional');
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.pattern"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>pattern (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.pattern)
- description and source-code
```javascript
pattern = function (schema, candidate) {
			var self = this;
			var regexs = schema.pattern;
			if (typeof candidate !== 'string') {
				return;
			}
			var matches = false;
			if (!_typeIs.array(regexs)) {
				regexs = [regexs];
			}
			regexs.forEach(function (regex) {
				if (typeof regex === 'string' && regex in _formats) {
					regex = _formats[regex];
				}
				if (regex instanceof RegExp) {
					if (regex.test(candidate)) {
						matches = true;
					}
				}
			});
			if (!matches) {
				self.report('must match [' + regexs.join(' or ') + '], but is equal to "' + candidate + '"', null, 'pattern');
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.properties"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>properties (schema, candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype.properties)
- description and source-code
```javascript
properties = function (schema, candidate, callback) {
			if (typeof callback === 'function') {
				return this.asyncProperties(schema, candidate, callback);
			}
			if (!(schema.properties instanceof Object) || !(candidate instanceof Object)) {
				return;
			}
			var properties = schema.properties,
					i;
			if (properties['*'] != null) {
				for (i in candidate) {
					if (i in properties) {
						continue;
					}
					this._deeperObject(i);
					this._validate(properties['*'], candidate[i]);
					this._back();
				}
			}
			for (i in properties) {
				if (i === '*') {
					continue;
				}
				this._deeperObject(i);
				this._validate(properties[i], candidate[i]);
				this._back();
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.someKeys"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>someKeys (schema, candidat)](#apidoc.element.schema-inspector.Validation.prototype.someKeys)
- description and source-code
```javascript
someKeys = function (schema, candidat) {
			var _keys = schema.someKeys;
			if (!_typeIs.object(candidat)) {
				return;
			}
			var valid = _keys.some(function (action) {
				return (action in candidat);
			});
			if (!valid) {
				this.report('must have at least key ' + _keys.map(function (i) {
					return '"' + i + '"';
				}).join(' or '), null, 'someKeys');
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.strict"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>strict (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.strict)
- description and source-code
```javascript
strict = function (schema, candidate) {
			if (typeof schema.strict === 'string') { schema.strict = (schema.strict === 'true'); }
			if (schema.strict !== true || !_typeIs.object(candidate) || !_typeIs.object(schema.properties)) {
				return;
			}
			var self = this;
			if (typeof schema.properties['*'] === 'undefined') {
				var intruder = Object.keys(candidate).filter(function (key) {
					return (typeof schema.properties[key] === 'undefined');
				});
				if (intruder.length > 0) {
					var msg = 'should not contains ' + (intruder.length > 1 ? 'properties' : 'property') +
						' [' + intruder.map(function (i) { return '"' + i + '"'; }).join(', ') + ']';
					self.report(msg, null, 'strict');
				}
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.type"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>type (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.type)
- description and source-code
```javascript
type = function (schema, candidate) {
			// return because optional function already handle this case
			if (typeof candidate === 'undefined' || (typeof schema.type !== 'string' && !(schema.type instanceof Array) && typeof schema.
type !== 'function')) {
				return;
			}
			var types = _typeIs.array(schema.type) ? schema.type : [schema.type];
			var typeIsValid = types.some(function (type) {
				return _simpleType(type, candidate);
			});
			if (!typeIsValid) {
				types = types.map(function (t) {return typeof t === 'function' ? 'and instance of ' + t.name : t; });
				this.report('must be ' + types.join(' or ') + ', but is ' + _realType(candidate), null, 'type');
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.uniqueness"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>uniqueness (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.uniqueness)
- description and source-code
```javascript
uniqueness = function (schema, candidate) {
			if (typeof schema.uniqueness === 'string') { schema.uniqueness = (schema.uniqueness === 'true'); }
			if (typeof schema.uniqueness !== 'boolean' || schema.uniqueness === false || (!_typeIs.array(candidate) && typeof candidate !== '
string')) {
				return;
			}
			var reported = [];
			for (var i = 0; i < candidate.length; i++) {
				if (reported.indexOf(candidate[i]) >= 0) {
					continue;
				}
				var indexes = getIndexes(candidate, candidate[i]);
				if (indexes.length > 1) {
					reported.push(candidate[i]);
					this.report('has value [' + candidate[i] + '] more than once at indexes [' + indexes.join(', ') + ']', null, 'uniqueness');
				}
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.validDate"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>validDate (schema, candidate)](#apidoc.element.schema-inspector.Validation.prototype.validDate)
- description and source-code
```javascript
validDate = function (schema, candidate) {
			if (String(schema.validDate) === 'true' && candidate instanceof Date && isNaN(candidate.getTime())) {
				this.report('must be a valid date', null, 'validDate');
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.schema-inspector.Validation.prototype.validate"></a>[function <span class="apidocSignatureSpan">schema-inspector.Validation.prototype.</span>validate (candidate, callback)](#apidoc.element.schema-inspector.Validation.prototype.validate)
- description and source-code
```javascript
validate = function (candidate, callback) {
		this.origin = candidate;
		if (typeof callback === 'function') {
			var self = this;
			return async.nextTick(function () {
				self._asyncValidate(self._schema, candidate, function (err) {
					self.origin = null;
					callback(err, self.result());
				});
			});
		}
		return this._validate(this._schema, candidate).result();
	}
```
- example usage
```shell
...
		jobs: {
			type: 'array',
			items: { type: 'string', minLength: 1 }
		},
		email: { type: 'string', pattern: 'email' }
	}
};
var result = inspector.validate(validation, data);
if (!result.valid)
	console.log(result.format());
/*
	Property @.email: must match [email], but is equal to "never!"
*/
'''
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
