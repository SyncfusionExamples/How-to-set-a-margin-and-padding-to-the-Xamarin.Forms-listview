# How to set a margin and padding to the Xamarin.Forms listview?

This example demonstrates how to set margin and padding to Xamarin.Forms listview.

## Sample

```xaml
<Grid BackgroundColor="DarkBlue" >
    <syncfusion:SfListView x:Name="listView" SelectionMode="None" BackgroundColor="LightGray" 
                            ItemSize="70" Margin="15" Padding="25"
                            ItemsSource="{Binding contactsinfo}">
        <syncfusion:SfListView.GroupHeaderTemplate>
            <DataTemplate>
                <ViewCell>
                    <Label Text="{Binding Key}" FontAttributes="Bold" FontSize="24"/>
                </ViewCell>
            </DataTemplate>
        </syncfusion:SfListView.GroupHeaderTemplate>
        
        <syncfusion:SfListView.ItemTemplate>
            <DataTemplate>
                <ViewCell>
                    <ViewCell.View>
                        <Grid x:Name="grid" >
                            <code>
                            . . .
                            . . .
                            <code>
                        </Grid>
                    </ViewCell.View>
                </ViewCell>
            </DataTemplate>
        </syncfusion:SfListView.ItemTemplate>
    </syncfusion:SfListView>
</Grid>
```

See [How to set a margin and padding to the Xamarin.Forms listview?](https://www.syncfusion.com/kb/9958/how-to-set-a-margin-and-padding-to-the-xamarin-forms-listview) for more details.

## Requirements to run the demo

* [Visual Studio 2017](https://visualstudio.microsoft.com/downloads/) or [Visual Studio for Mac](https://visualstudio.microsoft.com/vs/mac/)
* Xamarin add-ons for Visual Studio (available via the Visual Studio installer).

## Troubleshooting

### Path too long exception

If you are facing path too long exception when building this example project, close Visual Studio and rename the repository to short and build the project.
