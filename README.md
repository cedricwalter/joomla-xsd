joomla-xsd
==========

Schema Validation for Joomla 2.5 Extensions

to use them

```xml
<?xml version="1.0" encoding="UTF-8"?>
<extension type="component" version="1.6" method="upgrade"
	xsi:noNamespaceSchemaLocation="http://raw.github.com/cedricwalter/joomla-xsd/master/component.xsd"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
```
```xml
<?xml version="1.0" encoding="utf-8"?>
<metafile version="1.6"  client="site"
	xsi:noNamespaceSchemaLocation="http://raw.github.com/cedricwalter/joomla-xsd/master/language.xsd"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
```
```xml
<?xml version="1.0" encoding="UTF-8"?>
<extension type="module" version="1.6" client="site" method="upgrade"
	xsi:noNamespaceSchemaLocation="http://raw.github.com/cedricwalter/joomla-xsd/master/module.xsd"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
```
```xml
<?xml version="1.0" encoding="utf-8"?>
<extension version="1.6" type="plugin" group="system" method="upgrade"
	xsi:noNamespaceSchemaLocation="http://raw.github.com/cedricwalter/joomla-xsd/master/plugin.xsd"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
```
```xml
<?xml version="1.0" encoding="utf-8"?>
<extension version="1.6" type="template" method="upgrade"
    xsi:noNamespaceSchemaLocation="http://raw.github.com/cedricwalter/joomla-xsd/master/templateDetails.xsd"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
```