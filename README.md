<!-- tyhp-readme:start -->
# tyhpdef/php-http-message-factory

Tyhp type definitions for `php-http/message-factory` `1.1.0`.

```bash
composer require --dev tyhpdef/php-http-message-factory:1.1.0
```

This is a metapackage. Composer also installs `tyhpdef/php-http-message-factory-impl` (type files).
Require **this** name, not `tyhpdef/php-http-message-factory-impl`.

See https://tyhplang.com.

## Maintain `php-http/message-factory`? Ship the types yourself

If you are a Packagist maintainer of `php-http/message-factory`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/php-http-message-factory-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `php-http/message-factory` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/php-http-message-factory": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `php-http/message-factory` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `php-http/message-factory` with a real constraint,
   `"replace": { "tyhpdef/php-http-message-factory": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `php-http/message-factory` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/php-http-message-factory` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
