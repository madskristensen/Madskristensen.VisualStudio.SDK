# Meta packages for VSIX projects

[![Build status](https://ci.appveyor.com/api/projects/status/0ul3t4y6ci95vyys?svg=true)](https://ci.appveyor.com/project/madskristensen/registryexplorer)

Makes it easier to build Visual Studio extensions by having only a single NuGet package reference for the entire SDK.

```xml
<ItemGroup>
  <PackageReference Include="Madskristensen.VisualStudio.SDK" Version="15.0.0-alpha2" />
</ItemGroup>
```

## License
[Apache 2.0](LICENSE)