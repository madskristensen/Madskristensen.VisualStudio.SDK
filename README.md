# Complete SDK for VSIX projects

[![Build status](https://ci.appveyor.com/api/projects/status/0ul3t4y6ci95vyys?svg=true)](https://ci.appveyor.com/project/madskristensen/registryexplorer)

Makes it easier to build Visual Studio extensions by having only a single NuGet package reference for the entire SDK.

**Important!** This requires that the VSIX proect targets **.NET Framework 4.6**

To use this package, reference the version that matches the lowest version of Visual Studio your extension support. For instance, if your extension support Visual Studio 2015 (14.0) and 2017 (15.0) then you need to reference version 14.0 of the package like so:

```xml
<ItemGroup>
  <PackageReference Include="Madskristensen.VisualStudio.SDK" Version="14.0.0-alpha2" />
</ItemGroup>
```

## License
[Apache 2.0](LICENSE)