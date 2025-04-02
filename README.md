# swiftly-action

A GitHub Action for installing the [Swiftly toolchain manager for Swift](https://swift-server.github.io/swiftly/).

## Usage

To use Swiftly in your workflow, specify the repository followed by a tag as with any action:

```yaml
steps:
  - uses: actions/checkout@v4
  - uses: vapor/swiftly-action@v0.2.0
    with:
      toolchain: latest # optional
```

On completion, `swiftly`'s executable will be present in `PATH`, and the `SWIFTLY_HOME_DIR` and `SWIFTLY_BIN_DIR` environment variables will be available to all following steps.

## Arguments

At this time, the only argument supported is `toolchain`, which specifies a Swift toolchain name for Swiftly to install along with Swiftly itself. If the argument is omitted, only Swiftly itself is installed.

## Contributing

Contributions are welcome! Check out Vapor's [Contribution Guide](https://github.com/vapor/.github/blob/main/CONTRIBUTING.md).

## License

All code in this repository is released under the [MIT License](https://github.com/vapor/swiftly-action/blob/main/LICENSE).
