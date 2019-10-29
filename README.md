# SwiftUI Issues, Limitations & Unknowns
With Apple's documentation for SwiftUI being limited, I wanted to create a central resource of all bugs, issues and limitations with SwiftUI.

## Current Issues
- Environment/observed objects lose data on list view change. This problem appear in case when parent view updated with same data in terms of hash. The bug is not appearing when the parent view updated with different data.
  - 🔨 **[Example](https://github.com/mecid/swiftui-bug)**
  - 📝 FB7411430
- Tab view resets view and navigation stack
  - 🔨 **[Example](https://github.com/pedrommcarrasco/swiftui-tabviewResetsViewsAndNavigationStack)**
  - 📝 FB7411430
- Modal views/sheets don't automatically have environment data
  - 🔨 **[Example](https://forums.developer.apple.com/thread/117651)**
- Context menu not showing on a custom view with resizable or geometry reader
  - 🔨 **[Example](https://gist.github.com/ryangittings/23936424d936ead2cb768a9b55c5228d)**
  - 📝 FB7416520
- Multiple buttons in a list row causes both buttons to be actioned upon when tapped
  - 🔨 **[Example](https://stackoverflow.com/questions/56561064/swiftui-multiple-buttons-in-a-list-row)**
  - ↪️ **[Workaround](https://stackoverflow.com/a/56561423/11651357)**
  - 📝 FFB7416322
- 'Tried to pop to a view controller that doesn't exist' crash 
  - 🔨 **[Example](https://stackoverflow.com/q/58404725/11651357)**
  - ↪️ **[Workaround](https://stackoverflow.com/a/58466670/11651357)**

## Limitations/Unknowns
- No SwiftUI equivalent to UICollectionView
- Scrollview with HStack and items have poor performance for large data sets (all child views are loaded on init).
  - 📝 FB7216618
- Unable to remove or customise list separators
  - 📝 FB7108559
- Unable to change navigation appearance for a single view
  - 📝 FB7310681
- Unable to easily support deep linking for universal links or notifications
  - 📝 FB7408717
- Unable to use a UISearchController with a SwiftUI view
  - 🔨 **[Example](https://stackoverflow.com/questions/58511758/swiftui-uisearchcontroller-searchresultscontroller-navigation-stack-issue)**
  - 📝 FB7416329
- Unable to remove a list item background altogether for one cell
  - 📝 FB7371374
- Unable to know when view becomes active again (equivalent to viewDidAppear)

Please feel free to PR and submit examples, workarounds and/or fixes so I can keep this up to date.
