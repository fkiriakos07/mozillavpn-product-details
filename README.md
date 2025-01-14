![ci](https://github.com/mozilla/mozillavpn-product-details/actions/workflows/test.yml/badge.svg)

### https://mozilla.github.io/mozillavpn-product-details

Hosts a [product-details](https://github.com/mozilla-releng/product-details) style json files for the vpn.

Automatically deploys to gh pages.

* `schema.jtd.json` contains the schema that all files must validate.

The product details files are currently (Oct-28-21) used to:
* Build links to http://archive.mozilla.org/pub/vpn/ to packages for download on vpn.mozilla.org

The constraints in the schema capture constraints we've coded elsewhere e.g. in code, or in the archives
link structure.

#### Enforced restrictions
* No pushing to main
* Codeowners must approve production file changes
* Commits must be signed
* No exceptions

#### Running locally

```sh
npm i
npm test
```
