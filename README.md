joomla-xsd
==========

Schema Validation for Joomla 1.6/1.7/2.5/3.0/3.1 Extensions

Without them, Joomla accept any entry in manifest xml and never complains about

* Mistyping, like a valid xml but that the Joomla installer do not understand or only partially,
* Wrong constructs, xml tag child misplaced,
* Invalid data type, like a path not being a valid path, an expected integer being a text and so on…
Joomla just silently die during install or install only partially extensions. These days are over as developers with any
decent IDE will be able to validate while typing and enjoy auto completion.

* Joomla tracker http://joomlacode.org/gf/project/joomla/tracker/?action=TrackerItemEdit&tracker_id=8549&tracker_item_id=30358
* GitHub issue https://github.com/joomla/joomla-cms/issues/838

To use them NOW  before Joomla accept my pull request just include them in all your manifest like this:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<extension type="component" version="3.1" method="upgrade"
	xsi:noNamespaceSchemaLocation="http://raw.github.com/cedricwalter/joomla-xsd/master/component.xsd"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
```
```xml
<?xml version="1.0" encoding="utf-8"?>
<metafile version="3.1"  client="site"
	xsi:noNamespaceSchemaLocation="http://raw.github.com/cedricwalter/joomla-xsd/master/language.xsd"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
```
```xml
<?xml version="1.0" encoding="UTF-8"?>
<extension type="module" version="3.1" client="site" method="upgrade"
	xsi:noNamespaceSchemaLocation="http://raw.github.com/cedricwalter/joomla-xsd/master/module.xsd"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
```
```xml
<?xml version="1.0" encoding="utf-8"?>
<extension version="3.1" type="plugin" group="system" method="upgrade"
	xsi:noNamespaceSchemaLocation="http://raw.github.com/cedricwalter/joomla-xsd/master/plugin.xsd"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
```
```xml
<?xml version="1.0" encoding="utf-8"?>
<extension version="3.1" type="template" method="upgrade"
    xsi:noNamespaceSchemaLocation="http://raw.github.com/cedricwalter/joomla-xsd/master/templateDetails.xsd"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
```
```xml
<?xml version="1.0" encoding="utf-8"?>
<extension version="3.1" type="library" method="upgrade"
    xsi:noNamespaceSchemaLocation="http://raw.github.com/cedricwalter/joomla-xsd/master/library.xsd"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
```
```xml
<?xml version="1.0" encoding="utf-8"?>
<extension version="3.1" type="package" method="upgrade"
    xsi:noNamespaceSchemaLocation="http://raw.github.com/cedricwalter/joomla-xsd/master/package.xsd"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
```
