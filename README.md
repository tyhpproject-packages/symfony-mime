<!-- tyhp-readme:start -->
# tyhpdef/symfony-mime

Tyhp type definitions for `symfony/mime` `7.4.19`.

```bash
composer require --dev tyhpdef/symfony-mime:7.4.19
```

This is a metapackage. Composer also installs `tyhpdef/symfony-mime-impl` (type files).
Require **this** name, not `tyhpdef/symfony-mime-impl`.

See https://tyhplang.com.

## Maintain `symfony/mime`? Ship the types yourself

If you are a Packagist maintainer of `symfony/mime`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-mime-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/mime` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-mime": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/mime` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/mime` with a real constraint,
   `"replace": { "tyhpdef/symfony-mime": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/mime` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-mime` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
