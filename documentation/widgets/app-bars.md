# App Bars

## App Bar
An app bar can be set in the appBar section of a template.

`leading`, `centre`, `actions` & `bottom` can host components and are all optional.

`bottomHeight` is required when a bottom component is set.

`pinned` changes the behaviour of the navigation bar on scroll.

### Example
```json
{
	"type": "appBarWidget",
	"leading": {},
	"center": {},
	"actions": {},
	"bottom": {},
	"bottomHeight": 50,
	"backgroundColor": "white",
	"pinned": false
}
```

## Extended App Bar
The extended app bar contains the same properties as the `appBarWidget` plus `flexibleSpace` &  `flexibleSpaceHeight` properties.

### Example
```json
{
	"type": "extendedAppBarWidget",
	"leading": {},
	"center": {},
	"actions": {},
	"bottom": {},
	"bottomHeight": 50,
	"flexibleSpace": {},
	"flexibleSpaceHeight": 100,
	"backgroundColor": "white",
	"pinned": false
}
```