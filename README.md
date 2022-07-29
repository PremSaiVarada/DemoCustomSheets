# DemoCustomSheets

A simple customizable plugin for .NET MAUI. It is purely built using .NET MAUI.

Big thanks to [Matt Goldman](https://github.com/matt-goldman) by his wonderful concept of [#MAUIUIJuly](https://goforgoldman.com/2022/05/19/maui-ui-july.html), I learn so many new thing this in this month.

All the contents that are provided for this [#MAUIUIJuly](https://goforgoldman.com/2022/05/19/maui-ui-july.html) are very easy to understand the .NET Maui UI structure

I saw some content from the [Naweed Akram](https://github.com/naweed/) which are pretty good, I mostly like that [MauiPlantsApp](https://github.com/naweed/MauiPlanets/) and by seeing the [BottomSheet](https://blogs.xgenoapps.com/post/2022/07/23/maui-bottom-sheet) I got an idea that to create this BottomSheet as a plugin in NuGet, which is easy to use and added some properties for more customized UI.

With the knowledge of this program, I create one small/simple customizable sheets plugin and I hope that it is very useful to all.

## Supported platforms

- [x] Android
- [?] Other Platforms (Should work but I haven't tested)

## How to use

1. NuGet

NuGet ID: `plugin.customsheets`

![image](https://user-images.githubusercontent.com/110095923/181755596-673a4117-c84d-4360-a3a7-a502f7f002bd.png)

You can get this from NuGet here: https://www.nuget.org/packages/CustomSheets/

Or use the Package Manager:
```
Install-Package CustomSheets -Version 1.0.4
```

2.Add the following namespace declaration in your Xaml pages

```
xmlns:sheets="clr-namespace:CustomSheets;assembly=CustomSheets"
```
3.Add the sheet to your page and set the properties as you need

```
<sheets:Sheet x:Name="CommonSheet">
  <sheets:Sheet.SheetContent>
    <Label  Text="Payment Sucess ! " FontSize="Title" FontAttributes="Italic" TextColor="ForestGreen"/>
  </sheets:Sheet.SheetContent>
</sheets:Sheet>
```
## Properties
