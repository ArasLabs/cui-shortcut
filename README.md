# CUI Shortcut

The CUI Shortcut project demonstrates how to add a keyboard shortcut to Aras Innovator.

## History

This project and the following release notes have been migrated from the old Aras Projects page.

Release | Notes
--------|--------
[v2.0](https://github.com/ArasLabs/cui-shortcut/releases/tag/v2.0) | Added new keyboard shortcuts
[v1](https://github.com/ArasLabs/cui-shortcut/releases/tag/v1) | Initial Release *

> \* The original shortcut this project demonstrated used Ctrl+A to select all items in a grid. This was added to standard product around 11.0 SP12, so it is not recommended that you use v1.

#### Supported Aras Versions

Project | Aras
--------|------
[v2.0](https://github.com/ArasLabs/cui-shortcut/releases/tag/v2.0) | 11.0 SP15
[v1](https://github.com/ArasLabs/cui-shortcut/releases/tag/v1) | 11.0 SP12, 11.0 SP9

> Though built and tested using Aras 11.0 SP15. The CUI tools this project was built on were introduced in 11.0 SP7.

## Installation

#### Important!
**Always back up your code tree and database before applying an import package or code tree patch!**

### Pre-requisites

1. Aras Innovator installed (version 11.0 SPx preferred)
2. Aras Package Import tool
3. CUI Shortcut import package

### Install Steps

1. Backup your database and store the BAK file in a safe place.
2. Open up the Aras Package Import tool.
3. Enter your login credentials and click **Login**
  * _Note: You must login as root for the package import to succeed!_
4. Enter the package name in the TargetRelease field.
  * Optional: Enter a description in the Description field.
5. Enter the path to your local `..\cui-shortcut\Import\imports.mf` file in the Manifest File field.
6. Select **aras.labs.CUI_Shortcut** in the Available for Import field.
7. Select Type = **Merge** and Mode = **Thorough Mode**.
8. Click **Import** in the top left corner.
9. Close the Aras Package Import tool.

You are now ready to login to Aras and try out this new CUI Shortcut.

## Usage

There are 9 shortcuts added in this project, showing off 3 different shortcut locations.

### Main Window Shortcuts

1. **Ctrl+Shift+C** - Copy the currently selected item's ID into your clipboard

### Item Window Shortcuts

1. **Ctrl+Shift+C** - Copy the current item's ID into your clipboard
2. **Ctrl+R** - Refresh the current item window from the dom
3. **Alt+Ctrl+S** - Open up the structure browser of the current item
4. **Alt+Ctrl+W** - Open up the where used of the current item

### Item Window Relationship Shortcuts

1. **Ctrl+Shift+C** - Copy the currently selected relationship's ID into your clipboard
2. **Ctrl+C** * - Copy the current relationship using Aras Innovator's clipboard
3. **Ctrl+V** * - Paste the relationship onto the current item using Aras Innovator's clipboard
4. **Alt+Ctrl+V** * - Uses a special paste functionality using Aras Innovator's clipboard
     * This is equivalent to using "Paste Special"

> \* These shortcuts will not interfere with the default copy/paste functionality when you copy data from a cell in the relationship grid

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

For more information on contributing to this project, another Aras Labs project, or any Aras Community project, shoot us an email at araslabs@aras.com.

## Credits

Project written, documented, and published by Christopher Gillis at Aras Labs. @csgillis-aras

## License

Aras Labs projects are published to Github under the MIT license. See the [LICENSE file](./LICENSE.md) for license rights and limitations.
