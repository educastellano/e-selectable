# &lt;e-selectable&gt;

Web Component wrapper for selecting child elements


> Maintained by [Eduard C.](https://github.com/educastellano).

## Demo

> [Check it live](http://educastellano.github.io/e-selectable).

## Usage

1. Import Web Components' polyfill:

	```html
	<script src="//cdnjs.cloudflare.com/ajax/libs/polymer/0.0.20130711/polymer.min.js"></script>
	```

2. Import Custom Element:

	```html
	<link rel="import" href="src/e-selectable.html">
	```

3. Start using it!

	```html
	<e-selectable>
		<div>Item 1</div>
		<div>Item 2</div>
		<div>Item 3</div>
	</e-selectable>
	```

## Attributes

Name  			| Options                   | Default             | Description
---        			| ---                       | ---                 | ---
`selectedIndex`    | *string*                  | `undefined`               | Index of the selected item by default. If `multi` is enabled, `selectedIndex` can be a list of indexes separated by spaces.
`selectedClass`      			| *string*  	   | `e-selected`               | CSS class that'll be set in the item when selected.
`multi`   | *bool*                     | `undefined`               | Allows to select multiple items, using CMD/Control key or Shift key.
`checkboxes`   | *bool*                     | `undefined`               | When `true` and `multi` enabled, child items can be selected with a checkbox.


## Methods

Name 					| Parameters				| Return type			| Description
---						| ---						| ---					| ---
`getItems`				| `undefined`					| `array`				| Returns an array of all child items.
`getSelectedItems`		| `undefined`					| `array`				| Returns an array of selected child items.
`isItemSelected`		| `HTMLElement` *item*		| `bool`				| Returns `true` if the *item* is selected.
`selectItem`			| `HTMLElement` *item*		| `undefined`			| Selects *item*. Sets css class *selectedClass*. Fires a `polymer-signal` "e-selected".
`unSelectItem`			| `HTMLElement` *item* `bool` *silent*		| `undefined`			| Unselects *item*. Removes the css class *selectedClass*. Fires a `polymer-signal` "e-selected" if *silent* is `true`
`unSelectAll`			| `undefined`		| `undefined`			| Unselects all items.
`toggleItem`			| `HTMLElement+ *item*		| `undefined`			| Selects *item* it's not selected. Unselects otherwise.


## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

* v0.0.3 September 26, 2013
	* Multi-selection with checkboxes support
* v0.0.2 September 17, 2013
	* Multi-selection support
* v0.0.1 September 14, 2013
	* Started project using [boilerplate-element](https://github.com/customelements/boilerplate-element)

## License

[MIT License](http://opensource.org/licenses/MIT)