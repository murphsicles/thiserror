# @std/thiserror — Derive(Error) for Zeta

Auto-converted from [thiserror](https://crates.io/crates/thiserror) v2.0.18 via [Dark Factory](https://github.com/murphsicles/dark-factory).

Pairs with `@std/anyhow` for the complete error handling story.

```zeta
use @std/thiserror::Error;

#[derive(Error, Debug)]
enum MyError {
    #[error("permission denied for user {0}")]
    PermissionDenied(String),
    #[error("connection timeout after {seconds}s")]
    Timeout { seconds: u64 },
}
```

## License
MIT
