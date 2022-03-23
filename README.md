# internal-rust-registry
This is a public github repo, used to interface with the [internal-crate-registry](https://github.com/issuu/internal-crate-registry)

## Using the registry

In your repository, create a file `.cargo/config.toml` with the following content
```
[registries]
issuu-registry = { index = "https://github.com/issuu/internal-rust-registry" }
```

You can then add packages from the registry to your `cargo.toml` by adding a line like
```
internal-rust-helpers = { version = "0.3.3", registry = "issuu-registry" }
```
