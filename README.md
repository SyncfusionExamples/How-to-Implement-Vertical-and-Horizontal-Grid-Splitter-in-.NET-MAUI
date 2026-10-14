# How to Implement Vertical and Horizontal Grid Splitter in .NET MAUI

## Overview

The Grid Splitter control in .NET MAUI enables users to resize adjacent panes dynamically at runtime, creating flexible and interactive layouts. Depending on the application requirements, developers may need to arrange content vertically or horizontally to provide a better user experience. The Syncfusion Grid Splitter control supports both vertical and horizontal orientations, making it easy to create resizable layouts in different directions.

A vertical Grid Splitter divides content into top and bottom panes, allowing users to adjust the height of each section by dragging the splitter. This layout is commonly used in applications that display stacked content, such as log viewers, report viewers, dashboards, and data analysis tools. Users can allocate more space to important sections while reducing the size of less frequently used areas.

A horizontal Grid Splitter divides content into left and right panes, enabling users to resize the width of adjacent regions. This layout is widely used in file explorers, navigation-based applications, editors, and management systems where users need to customize the amount of space allocated to different content areas.

In many applications, both vertical and horizontal layouts may be required to support different workflows. The Grid Splitter control allows developers to easily configure the desired orientation using the `Orientation` property. This flexibility helps create professional desktop-style interfaces that maximize screen utilization while maintaining a clean and organized user experience.

The Syncfusion Grid Splitter control automatically manages the resizing behavior of neighboring panes, ensuring smooth user interactions. Developers can define multiple panes inside the Grid Splitter and allow users to adjust their size dynamically without manually updating layout measurements. This simplifies implementation while providing a highly responsive layout system.

This article demonstrates how to implement both vertical and horizontal Grid Splitter layouts in a .NET MAUI application. The example displays a vertical splitter in one section of the page and a horizontal splitter in another section, allowing users to experience both resizing modes within the same interface. By understanding these orientations, developers can build adaptable layouts that improve usability and provide greater control over content presentation.

## Sample

```xml
<?xml version="1.0" encoding="utf-8" ?>
<ContentPage
    xmlns="http://schemas.microsoft.com/dotnet/2021/maui"
    xmlns:x="http://schemas.microsoft.com/winfx/2009/xaml"
    xmlns:gridSplitter="clr-namespace:Syncfusion.Maui.GridSplitter;assembly=Syncfusion.Maui.GridSplitter"
    x:Class="GridSplitter.MainPage">

    <Grid RowDefinitions="*"
          ColumnDefinitions="*,*">

        <!-- Vertical Grid Spl*tter -->
        <gridSplitter:SfG*idSplitter Grid.Column="0"
       *                             Orien*ation="Vertical">

            <gr*dSplitter:SplitterPane>
          *     <Border Background="#D6EAF8">*                    <Label Text="T*p Pane"
                          *HorizontalOptions="Center"
       *                   VerticalOptions*"Center" />
                </Bord*r>
            </gridSplitter:Spli*terPane>

            <gridSplitte*:SplitterPane>
                <Bo*der Background="#FADBD8">
        *           <Label Text="Bottom Pan*"
                           Horiz*ntalOptions="Center"
             *             VerticalOptions="Cent*r" />
                </Border>
  *         </gridSplitter:SplitterPa*e>

        </gridSplitter:SfGridS*litter>

        <!-- Horizontal G*id Splitter -->
        <gridSplit*er:SfGridSplitter Grid.Column="1"
*                                  * Orientation="Horizontal">

      *     <gridSplitter:SplitterPane>
 *              <Border Background="*D5F5E3">
                    <Labe* Text="Left Pane"
                *          HorizontalOptions="Cente*"
                           Verti*alOptions="Center" />
            *   </Border>
            </gridSpl*tter:SplitterPane>

            <g*idSplitter:SplitterPane>
         *      <Border Background="#FCF3CF"*
                    <Label Text="*ight Pane"
                       *   HorizontalOptions="Center"
    *                      VerticalOpti*ns="Center" />
                </B*rder>
            </gridSplitter:S*litterPane>

        </gridSplitte*:SfGridSplitter>

    </Grid>

</C*ntentPage>
```

## Output

- The l*ft section of the page displays a *ertical Grid Splitter.
- Users can*drag the vertical splitter to resi*e the top and bottom panes.
- The *ight section of the page displays * horizontal Grid Splitter.
- Users*can drag the horizontal splitter t* resize the left and right panes.
* Each Grid Splitter operates indep*ndently without affecting the othe*.
- The layout provides a responsi*e and interactive resizing experie*ce.
- Content areas automatically *djust as users move the splitters.*
## Key Benefits

- Supports both *ertical and horizontal pane resizi*g.
- Creates flexible and user-fri*ndly layouts.
- Improves screen sp*ce utilization.
- Allows users to *ustomize pane sizes at runtime.
- *educes manual layout management.
-*Suitable for dashboards, editors, *xplorers, and enterprise applicati*ns.
- Provides a professional desk*op-style user experience.

## Conclusion

The Syncfusion Grid Splitter control supports both vertical and horizontal orientations, enabling developers to create versatile and interactive layouts in .NET MAUI. By configuring the `Orientation` property, applications can provide users with flexible resizing capabilities for both top-bottom and left-right content arrangements, resulting in a more customizable and efficient user experience.