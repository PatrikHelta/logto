---
'@logto/core': minor
---

add `sha256-crypt` and `sha512-crypt` legacy password hash support

Users can now be imported with SHA-crypt hashes (common format in Python `passlib`, PHP `crypt()`, and many Rust/Go libraries) by using the `Legacy` password algorithm with the expression `["sha512-crypt", ["@"], "$6$rounds=5000$salt$checksum"]`.
