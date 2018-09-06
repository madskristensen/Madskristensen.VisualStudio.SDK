# Registry Explorer

[![Build status](https://ci.appveyor.com/api/projects/status/0ul3t4y6ci95vyys?svg=true)](https://ci.appveyor.com/project/madskristensen/registryexplorer)

**Requires Visual Studio 2017.6 or newer**

This extension provides a tool window for looking at the Visual Studio registry hive. It shows the registry from both the **UserRegistryRoot** and **ApplicationRegistryRoot** (_Config).

![Tool Window](art/window.png)

Open the tool window from the top menu **View -> Other Windows -> Registry Hive Explorer**.

To refresh any node in the tree, simply right-click it and hit the **Refresh** button.

## Contribute
Check out the [contribution guidelines](.github/CONTRIBUTING.md)
if you want to contribute to this project.

For cloning and building this project yourself, make sure
to install the
[Extensibility Tools](https://visualstudiogallery.msdn.microsoft.com/ab39a092-1343-46e2-b0f1-6a3f91155aa6)
extension for Visual Studio which enables some features
used by this project.

## License
[Apache 2.0](LICENSE)