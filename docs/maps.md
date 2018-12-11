# Create a map

You create maps from the toolbar by selecting __IXIASOFT CCMS__, then __Create Map__, or from the icon toolbar. Map templates are in a system configuration template folder. They are available to admins only.

![create](../images/createTopic.png)

The create map dialog opens. Select the map type and select __Open in DITA map editor__.

You need to add the new map to a library version. When you do this, the map will have a primary version value of the version you select. The primary version has no special status, but each map must have a primary version, which cannot be deleted.

![version](../images/selectVersion.png)

If the map exists in only one version, then the map is the primary version. 

!!!Note
If you want to jump ahead to how the versions work, see [About products and libraries](#About-products-and-libraries).

## Editing and configuring new maps

When you open the map, it opens in the DITA MAP viewer. You can start adding topics to the map. To do this, you can drag topics from the search onto the map. 

!!! Note
The map must be locked to add topics. If the map is locked but you still get an error message that says "The map is not locked", then you can refresh the map by clicking the __Refresh__ button on the bottom of the DITA map viewer.

You can organize topic heirarchy by dragging topics or by using the yellow arrows above the map. 

Another way to add topics to a map is in the __Create Topic__ dialog. Check the box __Append topic to current map__.

![append](../images/appendToMap.png)

When you add a topic this way, the topic version is restricted to the same version as the current map.

### Elements and properties

You can add elements by right-clicking somewhere in the map and selecting __Add element__.

![elements](../images/insertElement.png)

For example, you can add a `<tablehead>` element to the map. You can edit the meta data of map elements with the properties view. You can open the __Properties__ window from the __Show View__ menu.

![showview](../images/showView.png)

From this view, you can add properties to map elements. Select a map element that you want to add a property to, then enter the value to the property.

![propertyvalue](../images/addPropertyValue.png)

### Adding submaps

Maps can contain other maps. These maps are therefore submaps of the main map. You add submaps by dragging them into the main map. 

If you are creating a submap from scratch, you have the option to select __Add to current map as submap__ when you are creating this map.

## Creating topic stubs

A topic stub is a map skeleton with information about what content needs to be added in the future. You create topic stubs from the topic stub menu in the DITA map viewer.

![topicStub](../images/topicStub.png)


When you create the topic stub it is placed into the map, and you can move it around like any other topic. However, the topic does not yet exist in the repository, it is more like a placeholder. It is not available from the search. 

![topicstub](../images/createTopicFromStub.png)

The only inidcation that it is a stub rather than a complete topic is from the greyed-out icon and it says type: `topic-type.xml`.

To create a topic from the topic stub, select __Generate Topics from Stubs__ from the drop-down menu.

![topicstub](../images/topicStubGenerate.png)

Once you generate the topic from the stub, it appears in the map with a normal topic icon and it is now searchable since it is added to the repository.

![topicstub](../images/afterTopicStubGenerated.png)

## Relationship tables

Relationship tables define the linking relationship among topics in a map. The relationship table keeps the link relationship outside of the topics themselves.

To create a relationship table, you do this from the relationship table [perspective](#The-user-interface).

Open the __RelTable Editing__ perspective.

From this perspective, and with a map locked, right-click in the __relationship Table Editor__ to add a new relationship table.













