# liferay-workspace

A highly opinionated way of structure your next Liferay 7.0 project.

#### Requirements

Install blade: https://github.com/gamerson/liferay-blade-tools

blade init

#### Modules

Put your osgi bundles in here.  We recommend that you put your portlets in apps, your hooks and integrations in extensions, and utils in shared but you can use any folder structure you choose.  All projects in the modules directory will have Liferay Gradle Plugin applied to it.

#### Themes

Themes can be created using the new node.js tools.  For more information go to: https://www.npmjs.com/package/generator-liferay-theme

Themes checked in this directory will automatically be built by gradle.  It will automatically install any required tools to build and deploy the theme.

#### Plugins SDK (Optional)

If you have an old Liferay project that used the Plugins SDK, you can include it in this project.  This will allow the project to participate in the full build lifecycle.  Gradle will call 'ant all' during a build. 
