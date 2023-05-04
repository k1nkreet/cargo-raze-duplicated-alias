with rustix@0.37.19 cargo-raze creates `rust_library` with duplicated value in aliases field which fails to compile:

```
aliases = {
    "@raze__errno__0_3_1//:errno": "libc_errno",
    "@raze__errno__0_3_1//:errno": "libc_errno",
},
```
