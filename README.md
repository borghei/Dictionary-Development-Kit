## Dictionary Development Kit :closed_book:

This is a mirror of Apple's Dictionary Development Kit to give more Developers access to this package.
Register a free developer account and download the auxiliary tools package from [developer.apple.com/downloads](developer.apple.com/downloads)
*It is now called: Additional Tool for Xcode (look for the latest version)

The Dictionary Development Kit lets you create your own custom dictionaries that users can access through the Dictionary application.

* Move the Dictionary Development Kit folder to /Applications/Utilities/DictionaryDevelopmentKit/ (without the spaces), and copy the project_templates folder to ~/Desktop/

* Open ~/Desktop/project_templates/Makefile and change DICT_BUILD_TOOL_DIR from /DevTools/Utilities/Dictionary Development Kit to /Applications/Utilities/DictionaryDevelopmentKit

* cd ~/Desktop/project_templates/; make && make install
The dictionary should show up in Dictionary.app after you quit and reopen it. After that, try editing MyDictionary.xml or MyDictionary.css. The dictionary name is the same as CFBundleName in the Info.plist, and the bundle name is DICT_NAME in the Makefile.
If the lookup popovers show results from an older version of the dictionary, try logging out and back in. Terminating com.apple.lookupd or removing ~/Library/Caches/com.apple.Dictionary* didn't seem to work.

## Credits
Copyright © 1997-2018 Apple Inc. All rights reserved.
