---
dep: ..\1 Configuration\onSelectionChanged.md
type: eventType
---
---
##### notUsedInTheme

##### shortDescription
Fires when a user selects/deselects a marker.

##### param(e): object
Information about the event.

##### field(e.component): object
The [widget's instance](/api-reference/10%20UI%20Widgets/Component/3%20Methods/instance().md '/Documentation/ApiReference/Data_Visualization_Widgets/dxVectorMap/Methods/#instance').

##### field(e.element): object
The widget's container.

##### field(e.target): Marker object
The selected/deselected area.

---
When implementing a handling function, use the object passed to it as its parameter. Among the fields of this object, you can find the selected/deselected marker. An object that represents this marker has fields and methods documented in the [Marker](/api-reference/20%20Data%20Visualization%20Widgets/dxVectorMap/7%20Map%20Elements/Marker '/Documentation/ApiReference/Data_Visualization_Widgets/dxVectorMap/Map_Elements/Marker/') class description.

To identify whether a marker has been selected or deselected, call its [selected()](/api-reference/20%20Data%20Visualization%20Widgets/dxVectorMap/7%20Map%20Elements/Marker/3%20Methods/selected().md '/Documentation/ApiReference/Data_Visualization_Widgets/dxVectorMap/Map_Elements/Marker/Methods/#selected') method. Pass **true** or **false** to this method to select or deselect the marker.

#####See Also#####
#include common-link-handleevents