# Editor Enhancer
The Editor Enhancer package is a collection of utilities aimed to enhance the Unity Editor. See the [roadmap](#roadmap) section for more information on what is coming next.

### Requirements

Unity 2019.3.0 or newer.  

### Installation

Open the Package Manager window and follow the [instructions to install a package from a Git URL](https://docs.unity3d.com/Manual/upm-ui-giturl.html). This is the URL you need to enter:

```
https://github.com/xeleh/enhancer.git
```


## Dark Theme

This is an option in Project Settings > Editor Enhancer to replace the personal Editor theme with the "Pro Editor UI theme" which is only available in [Unity Plus and Pro plans](https://store.unity.com/#plans-business). Unity defines this theme as a "Beautiful, easy on the eyes, dark UI environment". So yes, having this is pretty good.

![](https://xeleh.com/media/dark-theme.gif)

This feature has been tested with all Unity 2019.3.x versions and the latest Unity 2020.1 betas. It is a 100% legal hack, meaning **no binary patching** or something like that. You can check the source code to see how it works.

### Troubleshooting

Please make sure to leave the 'Auto Enable On Startup' unchecked until you verify that the dark theme change works for your particular Unity configuration as expected.


## Sidebar

The Sidebar is a configurable utility window that will keep docked on the left or the right side of the main editor window automatically. Its purpose is to host a series of clickable icons (items) each one of them having an associated one of the following functions:

* **Set Layout**: Load the layout associated with the item as if you would have chosen it from the Layout menu of the top right corner.
* **Execute Menu Item**: Perform the menu action associated with the item. You specify a menu action by indicating its menu path. As an example, you would specify `File/Save` to save the current scene with one click.
* **Separator**: No action, just a visual separator.

### Settings

You can fully configure the items and the rest of options of the Sidebar in the Project Settings > Editor Enhancer pane. This is a quick explanation of the less obvious options:

* **Save Layout On Change**: When enabled your current window layout will be saved before changing to another layout by clicking another Sidebar 'Set Layout' item. This is a nice convenience because "as is" Unity does not save a modified layout automatically but requires you to explicitly use the Save Layout option in the Layout menu.
* **Play Mode Layout**: You can specify here the layout you want to use during Play mode and the Sidebar will manage the change automatically. Try it.


## Menu Additions

Just some simple but convenient menu scripts that I use frequently in my projects:

| Menu Item | Key | Purpose |
|---|---|---|
| Assets/Duplicate | Ctrl+D ⌘+D |Duplicate the selected asset. I know we can do this already with the Edit/Duplicate option, but this is more convenient because the Duplicate option will be now available in the asset context menu as well. |
| GameObject/Group | Ctrl+G ⌘+G |Creates a new GameObject "Group" containing the current selection of GameObjects. The group will take the place of the last top-level GameObject in the selection. |

## Roadmap

* Double Click manager.
* Enter/Exit play mode actions.
* Overlay toolbars?
* Dockable Build Window?
* Customizable Toolbar?
* Notes?
* Notification Centre?

## Acknowledgements

Thanks to TheZombieKiller, Peter77, Grimreaper358, Kamyker and everyone who contributed with code and ideas to the [Editor skinning thread](https://forum.unity.com/threads/editor-skinning-thread.711059/) in the Unity forums. You gave the hints and inspired me to complete the work.

