# Fixed Lists / Grids

## Fixed List
The fixed list widget will take a number of components and display them in a vertical list.

The `mainAxisAlignment` property supports the following options: `start`, `end`, `spaceBetween`, `spaceAround` & `spaceEvenly`.

The `crossAxisAlignment` property supports the following options:
`start`, `end`, `center`, `stretch` & `baseline`.

Both `mainAxisAlignment` & `crossAxisAlignment` are optional.

```json
{
	"type": "fixedListWidget",
	"mainAxisAlignment": "start",
	"crossAxisAlignment": "center",
	"components": [{},{}]
}
```

## Fixed Horizontal List
The fixed horizontal list widget will take a number of components and display them in a horizontal list.

The `mainAxisAlignment` property supports the following options: `start`, `end`, `spaceBetween`, `spaceAround` & `spaceEvenly`.

The `crossAxisAlignment` property supports the following options:
`start`, `end`, `center`, `stretch` & `baseline`.

Both `mainAxisAlignment` & `crossAxisAlignment` are optional.

```json
{
	"type": "fixedHorizontalListWidget",
	"mainAxisAlignment": "start",
	"crossAxisAlignment": "center",
	"components": [{},{}]
}
```

## Fixed Horizontal Scroll List
The fixed horizontal list scroll widget will take a number of components and display them in a horizontal list with scrolling. All properties in this component are required.

```json
{
	"type": "fixedHorizontalListScrollWidget",
	"height": 150,
	"components": [{},{}]
}
```

## Fixed Grid
The fixed grid widget can be used to take a specified number of components and display them on a grid. The `itemPadding` property is used to add a padding between the items and is optional.

```json
{
	"type": "fixedGridWidget",
	"itemPadding": "xs",
	"columns": 2,
	"components": [{},{}]
}
```