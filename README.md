# UnityTweakableEditor
A simple class to inherit from when only minor tweaks to a component's inspector are required.
In such cases, a full custom inspector is normally overkill but, by inheriting from this class, custom tweaks become trivial.

To hide items from being drawn, simply override GetInvisibleInDefaultInspector, returning a string[] of fields to hide.
To draw/add extra GUI code/anything else you want before the default inspector is drawn, override OnBeforeDefaultInspector.
Similarly, override OnAfterDefaultInspector to draw GUI elements after the default inspector is drawn.

![image](https://user-images.githubusercontent.com/60183477/151524872-59b6b35b-ff91-45f5-b37e-b0805a846fde.png)

