# DemoCustomSheets [![Nuget](https://img.shields.io/nuget/v/CustomSheets?logo=Nuget)](https://www.nuget.org/packages/CustomSheets) [![Nuget](https://img.shields.io/nuget/dt/CustomSheets)](https://www.nuget.org/packages/CustomSheets) [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)


A simple customizable plugin for .NET MAUI.

Big thanks to [Matt Goldman](https://github.com/matt-goldman) by his wonderful concept of [#MAUIUIJuly](https://goforgoldman.com/2022/05/19/maui-ui-july.html), I learn so many new things in this month.

All the blogs from this [#MAUIUIJuly](https://goforgoldman.com/2022/05/19/maui-ui-july.html) are very easy to understand the .NET Maui UI structure

I saw some content from the [Naweed Akram](https://github.com/naweed/) which are pretty good, I mostly like that [MauiPlantsApp](https://github.com/naweed/MauiPlanets/) and by seeing the [BottomSheet](https://blogs.xgenoapps.com/post/2022/07/23/maui-bottom-sheet) I got an idea that to create this BottomSheet as a plugin in NuGet, which is easy to use and I added some more properties for more customized UI.

With the knowledge of this program, I create one small/simple customizable sheets plugin and I hope, it while be usefull to us.

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
| Property | Data Type | Defalut Value| Info |
| :--- | :----: | :--- | :--- |
| SheetHeight | double | height of the screen - 200 | This defines the height of the sheet content area |
| SheetWidth | double | width of the screen | This defines the width of the sheet content area |
| SheetVisibel | bool | false | This property only to get that the sheet is visible or not |
| IsCloseButtonVisible | bool | true | To hide/show the Close Button |
| SheetBackground | Brush | Brush.Default | To set the gradient colors to the sheet |
| SheetBackgroundColor | Color | White | To set the colors to the sheet |
| IsRoundRectangleVisible | bool | true | To hide/show the RoundRectangel in sheet |
| BackClickClose | bool | false | When click on the background to close the sheet |

## Methods
| Method | Explanation |
| :--- | :--- |
| OpenSheet | It will open the sheet |
| CloseSheet | It will close the sheet |

## Sample Output

https://user-images.githubusercontent.com/110095923/181768492-4e530fb8-b863-48fd-b6be-352905ded9e5.mp4

**Thanks to [@mattgoldman](https://twitter.com/mattgoldman/) and [Naweed Akram](https://twitter.com/xgeno)**
