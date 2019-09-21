# Dynamic Lists / Grids

## List
The list widget is used to display components in a vertical list from a datasource. The template will be applied on every item within the datasource.

The optional `limit` property is used to determine the maximum number of items that should be taken from the data source.

The `mainAxisAlignment` property supports the following options: `start`, `end`, `spaceBetween`, `spaceAround` & `spaceEvenly`.

The `crossAxisAlignment` property supports the following options:
`start`, `end`, `center`, `stretch` & `baseline`.

`mainAxisAlignment`, `crossAxisAlignment` are optional.

```json
{
	"type": "listWidget",
	"dataSource": "$list.items",
	"limit": 5,
	"mainAxisAlignment": "spaceBetween",
	"crossAxisAlignment": "start",
	"template": {}
}
```

## Horizontal List
The horizontal list widget is used to display components in a horizontal list from a datasource. The template will be applied on every item within the datasource.

The `mainAxisAlignment` property supports the following options: `start`, `end`, `spaceBetween`, `spaceAround` & `spaceEvenly`.

The optional `limit` property is used to determine the maximum number of items that should be taken from the data source.

```json
{
	"type": "horizontalListWidget",
	"mainAxisAlignment": "start",
	"dataSource": "$list.items",
	"limit": 5,
	"template": {}
}
```

## Horizontal Scroll List
The horizontal list scroll widget is used to display components in a horizontal scrollable list from a datasource. The template will be applied on every item within the datasource. The optional `limit` property is used to determine the maximum number of items that should be taken from the data source.

```json
{
	"type": "horizontalListScrollWidget",
	"height": 130,
	"dataSource": "$list.items",
	"limit": 5,
	"template": {}
}
```

## Grid
The grid widget is used to display a number of components from a datasource. The template will be applied on every item within the datasource. `childAspectRatio` defaults to 1.0 when unspecified. Like the `fixedGridWidget` `itemPadding` is also optional.

```json
{
	"type": "gridWidget",
	"itemPadding": "xs",
	"columns": 2,
	"childAspectRatio": 1.5,
	"dataSource": "$user.photos",
	"template": {}
}
```