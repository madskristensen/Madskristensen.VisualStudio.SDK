# Complete SDK for VSIX projects

[![Build status](https://ci.appveyor.com/api/projects/status/uq0qw8tybu13df13?svg=true)](https://ci.appveyor.com/project/madskristensen/madskristensen-visualstudio-sdk)
[![NuGet Pre Release](https://img.shields.io/nuget/vpre/Madskristensen.VisualStudio.SDK.svg)](https://www.nuget.org/packages/Madskristensen.VisualStudio.SDK)

Makes it easier to build Visual Studio extensions by having only a single NuGet package reference for the entire SDK.

**Important!** This requires that the VSIX project targets **.NET Framework 4.6**

To use this package, reference the version that matches the lowest version of Visual Studio your extension support. For instance, if your extension support Visual Studio 2015 (14.0) and 2017 (15.0) then you need to reference version 14.0 of the package like so:

```xml
<ItemGroup>
  <PackageReference Include="Madskristensen.VisualStudio.SDK" Version="14.0.123-pre" />
</ItemGroup>
```

If you don't want all the referenced .dll files to end up in the /bin directory, then simply exclude them like so:

```xml
<ItemGroup>
  <PackageReference Include="Madskristensen.VisualStudio.SDK" Version="14.0.0-beta3" ExcludeAssets="runtime" />
</ItemGroup>
```

## APIs and versions

### 14.0 
.vsixmanifest version: **14.0** or **14.0.23205**

* AsyncPackage
* TextMate grammer support
* Light bulbs (aka. SuggestedActions)
* Roslyn Analyzers
* ImageMonikers (including KnownMonikers collection)

### 14.3 
.vsixmanifest version: **14.0.25407**

* InfoBar (yellow bar)

### 15.0 
.vsixmanifest version: **15.0** or **15.0.26228**

* TextMate grammars registered by .pkgdef
* ServiceHub services
* Open Folder support
* Completion Filters
* .vsixmanifest v3 format
* NGen support

### 15.3
.vsixmanifest version: **15.0.26606**

* Task Status Center

## 15.6
.vsixmanifest version: **15.0.27413**

* Async tool window

### 15.7 
.vsixmanifest version: **15.0.27703**

* Async QuickInfo API
* Editor commanding API

### 15.8 
.vsixmanifest version: **15.0.28010**

* Async Completion API
* Extension pack support (.vsext)
* Language Server Protocol

## License
[Apache 2.0](LICENSE)