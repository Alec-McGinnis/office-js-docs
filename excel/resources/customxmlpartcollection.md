# CustomXmlPartCollection Object (JavaScript API for Excel)

_Excel 2016, Excel Online, Excel for iPad, Excel for Mac_

A collection of custom XML parts.

## Properties

| Property	   | Type	|Description| Req. Set|
|:---------------|:--------|:----------|:----|
|items|[CustomXmlPart[]](customxmlpart.md)|A collection of customXmlPart objects. Read-only.|1.3||

_See property access [examples.](#property-access-examples)_

## Relationships
None


## Methods

| Method		   | Return Type	|Description| Req. Set|
|:---------------|:--------|:----------|:----|
|[add(xml: string)](#addxml-string)|[CustomXmlPart](customxmlpart.md)|Creates a new custom XML part and adds it to the collection.|1.3|
|[getByNamespace(namespaceUri: string)](#getbynamespacenamespaceuri-string)|[CustomXmlPartScopedCollection](customxmlpartscopedcollection.md)|Gets a new collection of custom XML parts whose namespaces match the given namespace.|1.3|
|[getItem(id: string)](#getitemid-string)|[CustomXmlPart](customxmlpart.md)|Gets a custom XML part based on its ID.|1.3|
|[load(param: object)](#loadparam-object)|void|Fills the proxy object created in JavaScript layer with property and object values specified in the parameter.|1.1|

## Method Details


### add(xml: string)
Creates a new custom XML part and adds it to the collection.

#### Syntax
```js
customXmlPartCollectionObject.add(xml);
```

#### Parameters
| Parameter	   | Type	|Description|
|:---------------|:--------|:----------|:---|
|xml|string|Custom XML content. Must be a valid XML fragment.|

#### Returns
[CustomXmlPart](customxmlpart.md)

### getByNamespace(namespaceUri: string)
Gets a new collection of custom XML parts whose namespaces match the given namespace.

#### Syntax
```js
customXmlPartCollectionObject.getByNamespace(namespaceUri);
```

#### Parameters
| Parameter	   | Type	|Description|
|:---------------|:--------|:----------|:---|
|namespaceUri|string||

#### Returns
[CustomXmlPartScopedCollection](customxmlpartscopedcollection.md)

### getItem(id: string)
Gets a custom XML part based on its ID.

#### Syntax
```js
customXmlPartCollectionObject.getItem(id);
```

#### Parameters
| Parameter	   | Type	|Description|
|:---------------|:--------|:----------|:---|
|id|string|ID of the object to be retrieved.|

#### Returns
[CustomXmlPart](customxmlpart.md)

### load(param: object)
Fills the proxy object created in JavaScript layer with property and object values specified in the parameter.

#### Syntax
```js
object.load(param);
```

#### Parameters
| Parameter	   | Type	|Description|
|:---------------|:--------|:----------|:---|
|param|object|Optional. Accepts parameter and relationship names as delimited string or an array. Or, provide [loadOption](loadoption.md) object.|

#### Returns
void
