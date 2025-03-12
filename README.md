# ShapeStealther

Developed with Unreal Engine 5


Interact/Shapeshift system info

In order for a object to be interactable it needs to implement the Interaction interface (class settings -> ﻿Implemented Interfaces) as well as have a tag called interact.  The interaction will return itself and a Interaction type enum located in /Content/Interaction, right now this enum only has 2 options instant and shapeshift but this can be built apon later if needed. there is also a small UI animation that will play to show that its interactable

Shapeshifting, actor must implement Interaction and Shapeshift interface, ShapeShiftInfo returns the researcher name, level and there skeleton mesh asset.  The name goes as a tag that gets put on the player so that researchers can check there name vs all your tags and react if matching, changieng into a diffrent object will automaticaly clear the old tag.  

The resercher class (light blue) uses both of these system if you need a example
