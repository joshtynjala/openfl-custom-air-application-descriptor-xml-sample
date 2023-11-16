# OpenFL custom _application.xml_ template for Adobe AIR

The [OpenFL](https://openfl.org) library for Haxe contains a number of template files that are used when building a project. You can find them in the [_assets/templates_](https://github.com/openfl/openfl/tree/develop/assets/templates) directory. Using the `<template>` element in _project.xml_, it's possible to replace one or more of these template files with custom versions, on a per-project basis, and without forking OpenFL.

This sample project contains a directory named [_custom-templates_](https://github.com/joshtynjala/openfl-custom-index-html-sample/tree/main/custom-templates). It is configured in [_project.xml_](https://github.com/joshtynjala/openfl-custom-index-html-sample/tree/main/project.xml) like this:

```xml
<template path="custom-templates"/>
```

Inside [_custom-templates_](https://github.com/joshtynjala/openfl-custom-index-html-sample/tree/main/custom-templates), there's a file at [_air/template/application.xml_](https://github.com/joshtynjala/openfl-custom-air-application-descriptor-xml-sample/tree/main/custom-templates/air/template/application.xml). The relative path to this file matches the file named [_air/template/application.xml_](https://github.com/openfl/lime/tree/develop/templates/air/template/application.xml) inside Lime's [_templates_](https://github.com/openfl/openfl/tree/develop/templates) directory.

To confirm that the custom [_air/template/application.xml_](https://github.com/joshtynjala/openfl-custom-air-application-descriptor-xml-sample/tree/main/custom-templates/air/template/application.xml) is being used by the project, simply compile, and you should see your changes in _bin/air_.

```sh
openfl build air
```

Sample created by [Josh Tynjala](https://github.com/sponsors/joshtynjala), the author of [Feathers UI](https://feathersui.com/) and core contributor to [OpenFL](https://openfl.org/).