# api documentation for  [marky-markdown (v9.0.2)](https://github.com/npm/marky-markdown)  [![npm package](https://img.shields.io/npm/v/npmdoc-marky-markdown.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-marky-markdown) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-marky-markdown.svg)](https://travis-ci.org/npmdoc/node-npmdoc-marky-markdown)
#### npm's markdown parser

[![NPM](https://nodei.co/npm/marky-markdown.png?downloads=true)](https://www.npmjs.com/package/marky-markdown)

[![apidoc](https://npmdoc.github.io/node-npmdoc-marky-markdown/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-marky-markdown_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-marky-markdown/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-marky-markdown/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-marky-markdown/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Ashley Williams",
        "email": "ashley@npmjs.com",
        "url": "http://ashleygwilliams.github.io/"
    },
    "bin": {
        "marky-markdown": "./bin/marky-markdown.js"
    },
    "browser": {
        "highlights": false
    },
    "bugs": {
        "url": "https://github.com/npm/marky-markdown/issues"
    },
    "dependencies": {
        "atom-language-diff": "^1.0.0",
        "atom-language-nginx": "^0.6.1",
        "github-slugger": "^1.0.0",
        "github-url-to-object": "^2.2.3",
        "highlights": "^2.1.3",
        "highlights-tokens": "^1.0.1",
        "innertext": "^1.0.1",
        "is-badge": "^1.1.0",
        "language-dart": "^0.1.1",
        "language-erlang": "^2.0.0",
        "language-glsl": "^2.0.1",
        "language-haxe": "^0.2.1",
        "language-ini": "^1.7.0",
        "language-rust": "^0.4.7",
        "language-stylus": "^0.5.2",
        "lodash.assign": "^4.0.2",
        "lodash.defaults": "^4.0.1",
        "lodash.pickby": "^4.2.1",
        "markdown-it": "^8.0.0",
        "markdown-it-emoji": "^1.3.0",
        "markdown-it-expand-tabs": "^1.0.7",
        "markdown-it-lazy-headers": "^0.1.3",
        "markdown-it-task-lists": "^1.0.0",
        "property-ttl": "^1.0.0",
        "sanitize-html": "^1.6.1",
        "similarity": "^1.0.1"
    },
    "description": "npm's markdown parser",
    "devDependencies": {
        "browserify": "^13.0.1",
        "cheerio": "^0.22.0",
        "glob": "^7.1.1",
        "intercept-stdout": "^0.1.2",
        "mocha": "^3.1.2",
        "standard": "^8.4.0",
        "standard-format": "^2.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "cd3f20812992a5d6b440abe160bfca0f760b3ed0",
        "tarball": "https://registry.npmjs.org/marky-markdown/-/marky-markdown-9.0.2.tgz"
    },
    "gitHead": "fce972776b677ec7a6cb0bdc2f3054b0d89d328b",
    "homepage": "https://github.com/npm/marky-markdown",
    "keywords": [
        "readme",
        "markdown",
        "md",
        "documentation",
        "syntax highlighting",
        "html",
        "github",
        "npm"
    ],
    "license": "ISC",
    "main": "index.js",
    "maintainers": [
        {
            "name": "ag_dubs",
            "email": "ashley666ashley@gmail.com"
        },
        {
            "name": "bcoe",
            "email": "ben@npmjs.com"
        },
        {
            "name": "revin",
            "email": "rg@sevenite.com"
        },
        {
            "name": "rockbot",
            "email": "raquel@rckbt.me"
        },
        {
            "name": "soldair",
            "email": "soldair@gmail.com"
        }
    ],
    "name": "marky-markdown",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/npm/marky-markdown.git"
    },
    "scripts": {
        "build": "rm -rf dist && mkdir dist && touch dist/marky-markdown.js && browserify index.js -i highlights -s markyMarkdown > dist/marky-markdown.js",
        "pretest": "npm run build",
        "test": "standard-format -w && standard && mocha --timeout 8000"
    },
    "standard": {
        "ignore": "dist"
    },
    "version": "9.0.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module marky-markdown](#apidoc.module.marky-markdown)
1.  [function <span class="apidocSignatureSpan">marky-markdown.</span>parsePackageDescription (description)](#apidoc.element.marky-markdown.parsePackageDescription)
1.  [function <span class="apidocSignatureSpan">marky-markdown.</span>render (html, options)](#apidoc.element.marky-markdown.render)
1.  object <span class="apidocSignatureSpan">marky-markdown.</span>token_util

#### [module marky-markdown.render](#apidoc.module.marky-markdown.render)
1.  [function <span class="apidocSignatureSpan">marky-markdown.</span>render (html, options)](#apidoc.element.marky-markdown.render.render)
1.  [function <span class="apidocSignatureSpan">marky-markdown.render.</span>renderPackageDescription (description)](#apidoc.element.marky-markdown.render.renderPackageDescription)

#### [module marky-markdown.token_util](#apidoc.module.marky-markdown.token_util)
1.  [function <span class="apidocSignatureSpan">marky-markdown.token_util.</span>getText (token)](#apidoc.element.marky-markdown.token_util.getText)
1.  [function <span class="apidocSignatureSpan">marky-markdown.token_util.</span>isText (token)](#apidoc.element.marky-markdown.token_util.isText)
1.  [function <span class="apidocSignatureSpan">marky-markdown.token_util.</span>set (TokenConstructor)](#apidoc.element.marky-markdown.token_util.set)
1.  [function <span class="apidocSignatureSpan">marky-markdown.token_util.</span>unemoji (token)](#apidoc.element.marky-markdown.token_util.unemoji)



# <a name="apidoc.module.marky-markdown"></a>[module marky-markdown](#apidoc.module.marky-markdown)

#### <a name="apidoc.element.marky-markdown.parsePackageDescription"></a>[function <span class="apidocSignatureSpan">marky-markdown.</span>parsePackageDescription (description)](#apidoc.element.marky-markdown.parsePackageDescription)
- description and source-code
```javascript
parsePackageDescription = function (description) {
  return sanitize(render.renderPackageDescription(description))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.marky-markdown.render"></a>[function <span class="apidocSignatureSpan">marky-markdown.</span>render (html, options)](#apidoc.element.marky-markdown.render)
- description and source-code
```javascript
render = function (html, options) {
  var mdOptions = {
    html: true,
    langPrefix: 'highlight ',
    linkify: options.linkify
  }

  if (options.highlightSyntax) {
    mdOptions.highlight = function (code, lang) {
      return highlighter.highlightSync({
        fileContents: code,
        scopeName: scopeNameFromLang(highlighter, lang)
      })
    }
  }

  var parser = MD(mdOptions)
    .use(lazyHeaders)
    .use(emoji, {shortcuts: {}})
    .use(expandTabs, {tabWidth: 4})
    .use(githubTaskList)
    .use(headingLinks, options)
    .use(githubHeadings)
    .use(relaxedLinkRefs)
    .use(gravatar)
    .use(github, {package: options.package})
    .use(youtube)
    .use(badges)
    .use(packagize, {package: options.package})

  if (options.highlightSyntax) parser.use(codeWrap)
  if (options.serveImagesWithCDN) parser.use(cdnImages, {package: options.package})

  return githubLinkify(parser).render(html)
}
```
- example usage
```shell
...
    .use(youtube)
    .use(badges)
    .use(packagize, {package: options.package})

  if (options.highlightSyntax) parser.use(codeWrap)
  if (options.serveImagesWithCDN) parser.use(cdnImages, {package: options.package})

  return githubLinkify(parser).render(html)
}

var mappings = {
  sh: 'source.shell',
  markdown: 'source.gfm',
  erb: 'text.html.erb'
}
...
```



# <a name="apidoc.module.marky-markdown.render"></a>[module marky-markdown.render](#apidoc.module.marky-markdown.render)

#### <a name="apidoc.element.marky-markdown.render.render"></a>[function <span class="apidocSignatureSpan">marky-markdown.</span>render (html, options)](#apidoc.element.marky-markdown.render.render)
- description and source-code
```javascript
render = function (html, options) {
  var mdOptions = {
    html: true,
    langPrefix: 'highlight ',
    linkify: options.linkify
  }

  if (options.highlightSyntax) {
    mdOptions.highlight = function (code, lang) {
      return highlighter.highlightSync({
        fileContents: code,
        scopeName: scopeNameFromLang(highlighter, lang)
      })
    }
  }

  var parser = MD(mdOptions)
    .use(lazyHeaders)
    .use(emoji, {shortcuts: {}})
    .use(expandTabs, {tabWidth: 4})
    .use(githubTaskList)
    .use(headingLinks, options)
    .use(githubHeadings)
    .use(relaxedLinkRefs)
    .use(gravatar)
    .use(github, {package: options.package})
    .use(youtube)
    .use(badges)
    .use(packagize, {package: options.package})

  if (options.highlightSyntax) parser.use(codeWrap)
  if (options.serveImagesWithCDN) parser.use(cdnImages, {package: options.package})

  return githubLinkify(parser).render(html)
}
```
- example usage
```shell
...
    .use(youtube)
    .use(badges)
    .use(packagize, {package: options.package})

  if (options.highlightSyntax) parser.use(codeWrap)
  if (options.serveImagesWithCDN) parser.use(cdnImages, {package: options.package})

  return githubLinkify(parser).render(html)
}

var mappings = {
  sh: 'source.shell',
  markdown: 'source.gfm',
  erb: 'text.html.erb'
}
...
```

#### <a name="apidoc.element.marky-markdown.render.renderPackageDescription"></a>[function <span class="apidocSignatureSpan">marky-markdown.render.</span>renderPackageDescription (description)](#apidoc.element.marky-markdown.render.renderPackageDescription)
- description and source-code
```javascript
renderPackageDescription = function (description) {
  return MD({html: true}).renderInline(description)
}
```
- example usage
```shell
...
    html = sanitize(html)
  }

  return html
}

marky.parsePackageDescription = function (description) {
  return sanitize(render.renderPackageDescription(description))
}
...
```



# <a name="apidoc.module.marky-markdown.token_util"></a>[module marky-markdown.token_util](#apidoc.module.marky-markdown.token_util)

#### <a name="apidoc.element.marky-markdown.token_util.getText"></a>[function <span class="apidocSignatureSpan">marky-markdown.token_util.</span>getText (token)](#apidoc.element.marky-markdown.token_util.getText)
- description and source-code
```javascript
function getText(token) {
  var text = token.type === 'text' ? token.content : ''
  if (token.children && token.children.length) {
    text += token.children.reduce(function (previous, current) {
      return previous + (token.type !== 'image' ? getText(current) : '')
    }, '')
  }
  return text
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.marky-markdown.token_util.isText"></a>[function <span class="apidocSignatureSpan">marky-markdown.token_util.</span>isText (token)](#apidoc.element.marky-markdown.token_util.isText)
- description and source-code
```javascript
function isText(token) {
  var containsTextTokens = false
  if (token.children && token.children.length) {
    containsTextTokens = token.type !== 'image' && token.children.some(isText)
  }
  return containsTextTokens || token.type === 'text'
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.marky-markdown.token_util.set"></a>[function <span class="apidocSignatureSpan">marky-markdown.token_util.</span>set (TokenConstructor)](#apidoc.element.marky-markdown.token_util.set)
- description and source-code
```javascript
set = function (TokenConstructor) {
  Token = TokenConstructor
}
```
- example usage
```shell
...
  return text.charAt(0) === '(' && text.charAt(text.length - 1) === ')'
}

module.exports = function (parser) {
  if (parser) {
var linkify = parser.linkify

linkify.set({fuzzyLink: false}) // turn off auto-linking normal hostnames
linkify.add('//', null) // turn off protocol-relative links

// linkify everything hostnamey starting with 'www.', optionally in [] or ()
var scheme = {
  validate: function (text, pos, self) {
    if (!self.re.githubLinkify) {
      self.re.githubLinkify = new RegExp('^' + self.re.src_host_port_strict + self.re.src_path, 'i')
...
```

#### <a name="apidoc.element.marky-markdown.token_util.unemoji"></a>[function <span class="apidocSignatureSpan">marky-markdown.token_util.</span>unemoji (token)](#apidoc.element.marky-markdown.token_util.unemoji)
- description and source-code
```javascript
unemoji = function (token) {
  if (token.type === 'emoji') {
    return assign(new Token(), token, {content: token.markup})
  }
  return token
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
