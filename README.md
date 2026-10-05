<!-- tyhp-readme:start -->
# tyhpdef/illuminate-reflection

Tyhp type definitions for `illuminate/reflection` `13.33.0`.

```bash
composer require --dev tyhpdef/illuminate-reflection:13.33.0
```

This is a metapackage. Composer also installs `tyhpdef/illuminate-reflection-impl` (type files).
Require **this** name, not `tyhpdef/illuminate-reflection-impl`.

See https://tyhplang.com.

## Maintain `illuminate/reflection`? Ship the types yourself

If you are a Packagist maintainer of `illuminate/reflection`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/illuminate-reflection-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `illuminate/reflection` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/illuminate-reflection": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `illuminate/reflection` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `illuminate/reflection` with a real constraint,
   `"replace": { "tyhpdef/illuminate-reflection": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `illuminate/reflection` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/illuminate-reflection` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
