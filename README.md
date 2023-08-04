# xcode-frameworks-pkg

[hexops/xcode-frameworks](https://github.com/hexops/xcode-frameworks) is the Zig package to use when you need XCode frameworks, packaged for the Zig build system.

That package is well-designed, however there exists [a bug in the Zig package manager](https://github.com/hexops/mach/issues/903) (specifically `std.tar`) which prohibits using it: the package manager simply can't extract the tarball.

Once that issue is fixed, this package will go away. But for now, we have this temporary workaround: when you depend on this package, we use `git clone` to fetch the package - instead of the Zig package manager.

## Usage

See https://machengine.org/pkg/xcode-frameworks

## Issues

Issues are tracked in the [main Mach repository](https://github.com/hexops/mach/issues?q=is%3Aissue+is%3Aopen+label%3Axcode-frameworks).

## Community

Join the Mach engine community [on Discord](https://discord.gg/XNG3NZgCqp) to discuss this project, ask questions, get help, etc.
