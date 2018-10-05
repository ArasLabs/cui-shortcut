# CUI Shortcut

The CUI Shortcut project demonstrates how to .

## Project Details

**Built Using:** Aras 11.0 SP12
**Browsers Tested:** Internet Explorer 11, Firefox 62, Chrome 69

> Though built and tested using Aras 11.0 SP12. The CUI tools this project was built on were introduced in 11.0 SP7.

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

1. Log in to Aras as admin.
2. Navigate to any ItemType in the TOC that has multiple items in its grid.
3. Press **Ctrl+a** on your keyboard
4. See that all of the currently visible rows in the grid are selected

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
