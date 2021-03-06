---
title: OnDevice Markup Extension
author: sonnemaf
description: The OnDevice markup extension allows you to customize UI appearance on a per-DeviceFamily basis.
keywords: windows 10, uwp, uwp community toolkit, uwp toolkit, device family, markup extension, XAML, markup 
---

# OnDevice Markup Extension
The [OnDevice Markup Extension](https://docs.microsoft.com/en-us/dotnet/api/microsoft.toolkit.uwp.ui.extensions.ondevice) allows you to customize UI appearance on a per-DeviceFamily basis. It is inspired on the [OnPlatform](https://github.com/xamarin/Xamarin.Forms/issues/2608) markup extensions from Xamarin.Forms 3.2

## Syntax

**XAML**

```xaml

   <TextBlock Text="{helpers:OnDevice Default=Hi, Desktop=Hello, Xbox=World}"
              xmlns:helpers="using:Microsoft.Toolkit.Uwp.UI.Extensions.Markup" />

```

## Properties

| Property | Type | Description |
| -- | -- | -- |
| Default | object | Gets or sets the default value for this property, used if the device family property is not set or doesn't match one of the provided values.
| Desktop | object | Gets or sets a value for this property on a Windows.Desktop device
| Holographic | object | Gets or sets a value for this property on a Windows.Holographic device
| IoT | object | Gets or sets a value for this property on a Windows.IoT device
| Team | object | Gets or sets a value for this property on a Windows.Team device
| Xbox | object | Gets or sets a value for this property on a Windows.Xbox device

## Requirements

| Device family | Universal, 10.0.16299.0 or higher   |
| -- | -- |
| Namespace | Microsoft.Toolkit.Uwp.UI.Extensions |
| NuGet package | [Microsoft.Toolkit.Uwp.UI](https://www.nuget.org/packages/Microsoft.Toolkit.Uwp.UI/) |

## API Source Code

- [OnDevice source code](https://github.com/Microsoft/WindowsCommunityToolkit//blob/master/Microsoft.Toolkit.Uwp.UI/Extensions/Markup/OnDevice.cs)

## Related Topics

- [MarkupExtension Class](https://docs.microsoft.com/en-us/uwp/api/windows.ui.xaml.markup.markupextension)
- [SystemInformation.DeviceFamily Property](https://docs.microsoft.com/en-us/dotnet/api/microsoft.toolkit.uwp.helpers.systeminformation.devicefamily)
