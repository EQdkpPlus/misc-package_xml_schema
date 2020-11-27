# misc-package_xml_schema

The `package.xml` file must be placed into the root folder of the Zip-Package. The Zip-Package contains all files of the extension, e.g. directly from a GitHub release.

```
<?xml version="1.0" encoding="utf-8"?>
<install type="{TYPE}" version="{DEP_COREVERSION}">
	<folder>{FOLDER}</folder>
	<name>{NAME}</name>
	<author>{AUTHOR}</author>
	<authorEmail>{AUTHOR-EMAIL}</authorEmail>
	<creationDate>{CREATION-DATE}</creationDate>
	<copyright>{COPYRIGHT}</copyright>
	<version>{VERSION}</version>
	<level>{LEVEL}</level>
</install>
```
* `TYPE`: `plugin`, `template`, `portal`, `game` or `language`
* `DEP_COREVERSION`: the required version of the EQdkp Plus core for this extension
* `FOLDER`: the folder of the extension. Must only contain [a-zA-Z0-9]. If you use the GitHub repositories, remove the prefix like `portal-` or `plugin-`
* `NAME`: the name of the extension
* `AUTHOR`: name of the author
* `AUTHOR-EMAIL`: contact email of the extension author
* `CREATION-DATE`: unix timestamp of release date
* `COPYRIGHT`: the copyright of the extension, might include the licence
* `VERSION`: the version of the extension, e.g. `1.2.3`
* `LEVEL`: the release level. Default is `stable`, but can be `alpha` or `beta`


## Example
Example `package.xml` file for the game "Blade & Soul"
```
<?xml version="1.0" encoding="utf-8"?>
<install type="game" version="2.2.17.0">
	<folder>bs</folder>
	<name>Blade &amp; Soul</name>
	<author>Bloodsoul</author>
	<authorEmail>redacted@redacted.org</authorEmail>
	<creationDate>1600879648</creationDate>
	<copyright>(C)2016 Bloodsoul</copyright>
	<version>1.4.0</version>
	<level>stable</level>
</install>
```
