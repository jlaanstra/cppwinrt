# MSBuild support

This fork contains improved MSBuild support compared to https://github.com/microsoft/cppwinrt

-------------------------

[![Build status](https://dev.azure.com/microsoft/Dart/_apis/build/status/cppwinrt%20internal%20build)](https://dev.azure.com/microsoft/Dart/_build/latest?definitionId=31784)

# The C++/WinRT language projection

C++/WinRT is an entirely standard C++ language projection for Windows Runtime (WinRT) APIs, implemented as a header-file-based library, and designed to provide you with first-class access to the modern Windows API. With C++/WinRT, you can author and consume Windows Runtime APIs using any standards-compliant C++17 compiler.

* Documentation: https://aka.ms/cppwinrt
* NuGet package: http://aka.ms/cppwinrt/nuget
* Visual Studio extension: http://aka.ms/cppwinrt/vsix
* Wikipedia: https://en.wikipedia.org/wiki/C++/WinRT

# Building C++/WinRT

Don't build C++/WinRT yourself - just download the latest version here: https://aka.ms/cppwinrt/nuget

If you really want to build it yourself, the simplest way to do so is to run the `build_test_all.cmd` script in the root directory. Developers needing to work on the C++/WinRT compiler itself should go through the following steps to arrive at an efficient inner loop:

* Open a dev command prompt pointing at the root of the repo.
* Open the `cppwinrt.sln` solution.
* Build the x64 Release configuration of the `cppwinrt` project only. Don’t attempt to build anything just yet.
* Run `build_projection.cmd` in the dev command prompt.
* Switch to the x64 Debug configuration in Visual Studio and build all projects as needed.

# Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

# Project Reunion

Project Reunion is a set of libraries, frameworks, components, and tools that you can use to access powerful Windows platform functionality from all kinds of apps on many versions of Windows. Project Reunion combines the power of Win32 native applications alongside modern APIs, so your apps light up everywhere your users are.

Other Project Reunion components include [WinUI](https://github.com/microsoft/microsoft-ui-xaml), WebView2, MSIX, [Rust/WinRT](https://github.com/microsoft/winrt-rs), and [C#/WinRT](https://github.com/microsoft/cswinrt). If you'd like to learn more, contribute to Project Reunion, or have app model questions, visit [Project Reunion on GitHub](https://github.com/microsoft/ProjectReunion).
