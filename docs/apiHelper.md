# apiHelper

* [getFeaturesProperties()](#getfeaturesproperties)
* [getFeatureProperty()](#getfeatureproperty)
* [getAnchorByFeatureProperty()](#getanchorbyfeatureproperty)
* [getNearestAnchors()](#getnearestanchors)

## getFeaturesProperties()

Returns an `Array` with all the features properties' keys.

### Parameters

| Name | Type | Description |
| :---: | :---: | :---: |
| - | - | - |

### Output

| Type | Description |
| --- | --- |
|`Array` | All the features properties' keys |

### Example

`apiHelper.getFeaturesProperties()`

## getFeatureProperty(key)

Returns an `Array` with all the values from a given feature property key.

### Parameters

| Name | Type | Description |
| --- | --- | --- |
| `key` | `String` | Any key from `getFeaturesProperties()` |

### Output

| Type | Description |
| --- | --- |
|`Array` | Values from a given feature property key |

### Example

`apiHelper.getFeatureProperty('DIST')`

## getAnchorByFeatureProperty(key, value)

Returns a `Array` with `LatLng Objects` from a given feature property key and feature property value.

### Parameters

| Name | Type | Description |
| --- | --- | --- |
| `key` | `String` | Any key from `getFeaturesProperties()` |
| `value` | `String` | Any value from `getFeatureProperty(key)` |

### Output

| Type | Description |
| --- | --- |
|`Array` | `LatLng Objects`: `{ lat: Number, lng: Number }` |

### Example

`getAnchorByFeatureProperty('DIST', 'Gràcia')`

## getNearestAnchors(position, radius)

Returns a `Array` with `LatLng Objects` from a given position and a radius.

### Parameters

| Name | Type | Description |
| --- | --- | --- |
| `position` |`LatLng Object` | The position to be used as the center point |
| `radius` | `Number` | The radius in meters |

### Output

| Type | Description |
| --- | --- |
|`Array` | `LatLng Objects`: `{lat: Number, lng: Number}` |

### Example

`apiHelper.getNearestAnchors({ lat: 41.386664, lng: 2.1675844 }, 200)`