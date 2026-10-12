# LibFuseSharp

[![NuGet](https://img.shields.io/nuget/v/LibFuseSharp.svg?label=NuGet)](https://www.nuget.org/packages/LibFuseSharp/)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE.txt)
[![.NET 8 | 9 | 10](https://img.shields.io/badge/.NET-8%20%7C%209%20%7C%2010-512bd4.svg?logo=dotnet&logoColor=white)](https://dotnet.microsoft.com/download/dotnet)

A FUSE 3 high-level mount library for .NET on Linux ([libfuse3](https://github.com/libfuse/libfuse))
and macOS ([macFUSE](https://macfuse.io)). Implement a read-only volume, mount it with one call,
and probe the runtime before you mount.

Used by [SimpleXisoDrive](https://github.com/purelogiccode/SimpleXisoDrive) and
[CHDMounter](https://github.com/purelogiccode/CHDMounter).

## Layout

| Path | Description |
|------|-------------|
| `LibFuseSharp/` | The library (`LibFuseSharp` NuGet package, `FuseSharp` namespace) |
| `LibFuseSharp.Tests/` | xUnit tests for the library |

See [`LibFuseSharp/README.md`](LibFuseSharp/README.md) for the package readme (requirements,
quick start and API overview).

## Build, test and pack

```bash
# Build (net8.0, net9.0, net10.0)
dotnet build LibFuseSharp.slnx -c Release

# Run the tests
dotnet test LibFuseSharp.Tests/LibFuseSharp.Tests.csproj -c Release

# Pack the NuGet package
dotnet pack LibFuseSharp/LibFuseSharp.csproj -c Release
```

## License

GPLv3 — see [LICENSE.txt](LICENSE.txt).
