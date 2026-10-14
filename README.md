# How to Implement Vertical and Horizontal Grid Splitter in .NET MAUI

This repository contains a sample explaining how to implement vertical and horizontal Grid Splitter layouts in .NET MAUI using the Syncfusion `SfGridSplitter` control.

The Grid Splitter control allows users to resize panes dynamically at runtime, creating flexible and interactive layouts. Depending on the application requirements, panes can be arranged using either vertical or horizontal orientations. The `Orientation` property determines how the panes are displayed and how users interact with the splitter during resizing.

In this example, two Grid Splitter controls are displayed side by side. One Grid Splitter uses a vertical orientation, while the other uses a horizontal orientation. This demonstrates how different orientations can be used to create customizable and responsive layouts for various application scenarios.

## Sample

### XAML

```xml
<ContentPage xmlns="http://schemas.microsoft.com/dotnet/2021/maui"
             xmlns:x="http://schemas.microsoft.com/winfx/2009/xaml"
             xmlns:gridSplitter="clr-namespace:Syncfusion.Maui.GridSplitter;assembly=Syncfusion.Maui.GridSplitter"
             x:Class="GridSplitter.MainPage">

    <Grid RowDefinitions="*"
          ColumnDefinitions="*,*">

        <!-- Vertical Grid Splitter -->
        <gridSplitter:SfGridSplitter Grid.Column="0"
                                     Orientation="Vertical">

            <gridSplitter:SplitterPane>
                <Border Background="#D6EAF8">
                    <Label Text="Top Pane"
                           HorizontalOptions="Center"
                           VerticalOptions="Center" />
                </Border>
            </gridSplitter:SplitterPane>

            <gridSplitter:SplitterPane>
                <Border Background="#FADBD8">
                    <Label Text="Bottom Pane"
                           HorizontalOptions="Center"
                           VerticalOptions="Center" />
                </Border>
            </gridSplitter:SplitterPane>

        </gridSplitter:SfGridSplitter>

        <!-- Horizontal Grid Splitter -->
        <gridSplitter:SfGridSplitter Grid.Column="1"
                                     Orientation="Horizontal">

            <gridSplitter:SplitterPane>
                <Border Background="#D5F5E3">
                    <Label Text="Left Pane"
                           HorizontalOptions="Center"
                           VerticalOptions="Center" />
                </Border>
            </gridSplitter:SplitterPane>

            <gridSplitter:SplitterPane>
                <Border Background="#FCF3CF">
                    <Label Text="Right Pane"
                           HorizontalOptions="Center"
                           VerticalOptions="Center" />
                </Border>
            </gridSplitter:SplitterPane>

        </gridSplitter:SfGridSplitter>

    </Grid>

</ContentPage>
```

## Explanation

The `Orientation` property controls how panes are arranged within the Grid Splitter and determines the direction in which users can resize adjacent panes.

### Vertical Orientation

A Grid Splitter configured with `Orientation="Vertical"` displays panes side by side. The splitter appears between the panes, allowing users to resize the width of adjacent panes by dragging the separator horizontally.

```xml
<gridSplitter:SfGridSplitter Orientation="Vertical">
```

In this example, the vertical Grid Splitter contains:

- Top Pane
- Bottom Pane

Users can drag the splitter horizontally to adjust the width allocated to each pane.

### Horizontal Orientation

A Grid Splitter configured with `Orientation="Horizontal"` displays panes one above another. The splitter appears between the panes, allowing users to resize the height of adjacent panes by dragging the separator vertically.

```xml
<gridSplitter:SfGridSplitter Orientation="Horizontal">
```

In this example, the horizontal Grid Splitter contains:

- Left Pane
- Right Pane

Users can drag the splitter vertically to adjust the height allocated to each pane.

## How It Works

The page uses a two-column Grid layout to display both Grid Splitter orientations side by side.

The left side of the page contains:

- A Grid Splitter configured with vertical orientation.
- Two resizable panes.
- A splitter that can be dragged horizontally.

The right side of the page contains:

- A Grid Splitter configured with horizontal orientation.
- Two resizable panes.
- A splitter that can be dragged vertically.

Both Grid Splitter controls operate independently, allowing users to interact with each layout separately.

## Output

When the application runs, the following behavior can be observed:

- Two Grid Splitter controls are displayed side by side.
- The left Grid Splitter uses vertical orientation.
- The right Grid Splitter uses horizontal orientation.
- Users can drag the vertical splitter horizontally to resize adjacent panes.
- Users can drag the horizontal splitter vertically to resize adjacent panes.
- Pane sizes update dynamically during interaction.
- The content inside each pane automatically adjusts according to the available space.
- Both Grid Splitter controls function independently.
- The layout remains responsive across different screen sizes and orientations.

## Benefits

Implementing vertical and horizontal Grid Splitters provides several advantages:

- Creates flexible and customizable user interfaces.
- Improves screen space utilization.
- Enables user-controlled pane resizing.
- Enhances application usability.
- Supports responsive dashboard layouts.
- Reduces the need for complex layout calculations.
- Provides a desktop-like user experience.

## Common Use Cases

Vertical and horizontal Grid Splitters are useful in many application scenarios, including:

- Dashboard applications.
- Reporting and analytics solutions.
- File explorer interfaces.
- Project management systems.
- Administrative portals.
- Development environments.
- Data management applications.
- Enterprise productivity solutions.

## Conclusion

The Syncfusion `SfGridSplitter` control supports both vertical and horizontal orientations, enabling developers to create flexible and interactive layouts in .NET MAUI applications. By configuring the `Orientation` property, users can dynamically resize panes and optimize the layout according to their workflow and preferences.