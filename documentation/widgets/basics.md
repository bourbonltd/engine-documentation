# Basics

## Block
The block widget is a jack of all trades. It can be used to give padding, create rounded corners, fit and scale with flex and apply background colors / images.

The only required properties are `type` and `component`.

### Example
```json
{
	"type": "blockWidget",
	"safeInsets": false,
	"padding": ["m","m","m",""],
	"backgroundColor": "white",
	"borderColor": "black",
	"borderWidth": 1,
	"borderRadius": 10,
	"height": 150,
	"backgroundImage": "$user.backgroundImage",
	"flex": 1,
	"component": {}
}
```

## Text
The `overflow` property supports: `ellipsis`, `fade`, `clip`.

The `textAlign` property supports: `center`, `left`, `right`, `end`, `start`, `justify`.

`style`, `color`, `textAlign`, `maxlines` & `overflow` are optional.

```json
{
	"type": "textWidget",
	"text": "$person.name",
	"style": "bodyText",
	"color": "black",
	"textAlign": "left",
	"maxLines": 1,
	"overflow": "ellipsis"
}
```

## Action
An action widget can be used to wrap any component and make it tappable.

The behaviour property supports:
- `push` pushes a new route into the navigation stack.
- `system` offloads the action onto the operating system. Actions like `mailto:support@bourbon.sh` will open the default email client.
- `back` pops the navigation stack one step back.
- `retain` replaces the current view with a new route.

### Example
```json
{
	"type": "actionWidget",
	"action": "/events",
	"behaviour": "push",
	"component": {}
}
```

## Conditional
This component is used to conditionally show a component based on a specified condition.

The condition property supports: `>`, `<`, `==` & `in`. If no operator is specified the condition will check if the property is null.

### Example
```json
{
	"type": "conditionalWidget",
	"condition": "$items > 2",
	"true": {},
	"false": {}
}
```

## Icon
The icon widget is used to display an icon from any loaded icon font.

Note: Icon fonts need to be loaded in the assets section of the configuration.

```json
{
	"type": "IconWidget",
	"color": "black",
	"font": "IconFont-One",
	"size": 18,
	"value": "\e012"
}
```

## Markdown
The markdown widget takes content from the `value` property and renders it on screen.

All the properties except from `type` and `value` are optional.

```json
{
	"type": "markdownWidget",
	"value": "$venue.details",
	"textColor": "black",
	"headingColor": "purple",
	"textStyleA": "bodyText",
	"colorA": "blue",
	"textStyleP": "bodyText",
	"textStyleStrong": "boldBodyText",
	"textStyleLi": "bodyText",
	"textStyleCode": "codeBodyText",
	"textStyleBlockquote": "bodyText",
	"textStyleEm": "bodyText",
	"textStyleH1": "headingTextOne",
	"textStyleH2": "headingTextTwo",
	"textStyleH3": "headingTextThree",
	"textStyleH4": "headingTextFour",
	"textStyleH5": "headingTextFive",
	"textStyleH6": "headingTextSix"
}
```