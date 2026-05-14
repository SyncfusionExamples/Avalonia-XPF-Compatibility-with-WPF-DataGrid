# AvaloniaUI-XPF-Compatibility-with-WPF-DataGrid

## Overview

This demo showcases **AvaloniaUI Compatibility with WPF DataGrid** using the Avalonia-XPF (eXtensible Platform Framework) technology. The sample demonstrates how to use Syncfusion's WPF SfDataGrid control within an AvaloniaUI application, combining the power of AvaloniaUI's cross-platform capabilities with WPF's comprehensive control library.

## About Avalonia-XPF-Compatibility

**Avalonia-XPF** is a compatibility layer that enables developers to use traditional WPF controls and frameworks within AvaloniaUI applications. It provides seamless integration between AvaloniaUI's modern, cross-platform architecture and the extensive ecosystem of WPF controls.

### Key Benefits:
- **Cross-Platform Support**: Leverage WPF controls in AvaloniaUI applications
- **Rich Component Library**: Access to Syncfusion and other WPF control libraries
- **Unified Development**: Build applications using familiar WPF APIs with AvaloniaUI's framework
- **Data Binding Integration**: Seamless MVVM pattern support with data binding

## Sample Features

This demo includes an **Employee Data Grid** with the following capabilities:

- **Data Binding**: MVVM pattern with employee data binding
- **In-place Editing**: Edit employee information directly in the grid
- **Filtering & Sorting**: Filter and sort employee records by any column
- **Multiple Column Types**: Text, template, checkbox, and percent columns
- **Custom Templates**: Display employee details with icons and formatted data
- **Multi-row Selection**: Select multiple employees using checkboxes
- **Formatted Display**: Currency formatting for salary and progress indicator for software proficiency

## NuGet Configuration

To use Avalonia-XPF with Syncfusion WPF controls, configure your NuGet sources as follows:

### Package Sources

The `NuGet.config` file should include the following package sources:

```xml
<configuration>
  <packageSources>
    <clear />
    <add key="api.nuget.org" value="https://api.nuget.org/v3/index.json" />
    <add key="xpf" value="https://xpf-nuget-feed.avaloniaui.net/v3/index.json" />
    <add key="avalonia-nightly" value="https://nuget-feed-nightly.avaloniaui.net/v3/index.json" />
  </packageSources>
</configuration>
```

### Package Source Credentials

For accessing the XPF NuGet feed, provide authentication credentials:

```xml
<packageSourceCredentials>
  <xpf>
    <add key="Username" value="Enter the Username" />
    <add key="ClearTextPassword" value="Enter the Password" />
  </xpf>
</packageSourceCredentials>
```

**Note**: Replace `Enter the Username` and `Enter the Password` with your actual XPF feed credentials.

## Project Setup

### Prerequisites:
- .NET 7.0 or later
- Visual Studio 2022 or equivalent
- XPF SDK credentials for NuGet access
- Syncfusion License Key

### Configuration Steps:

1. **Update NuGet.config**: Ensure credentials are properly configured in the `NuGet.config` file located in the project root
2. **Set License Key**: Add your AvaloniaUI.Xpf.LicenseKey in the project file:
   ```xml
   <RuntimeHostConfigurationOption Include="AvaloniaUI.Xpf.LicenseKey" Value="Your-License-Key" />
   ```
3. **Restore Packages**: Run `dotnet restore` to download required packages
4. **Build and Run**: Build the solution and run the application

## Usage

Once the application runs, the SfDataGrid displays employee data with full CRUD capabilities:
- **Select** employees using checkboxes
- **Edit** information by clicking on cells
- **Filter** data using the built-in filter row
- **Sort** by clicking column headers
- **View** formatted data with custom templates and visual indicators
