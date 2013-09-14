<el-selectable>
===============

Web Component wrapper for selecting its children elements


> Maintained by [Eduard C.](https://github.com/educastellano).

## Demo

> [Check it live](http://educastellano.github.io/el-selectable).

## Usage

1. Import Web Components' polyfill:

	```html
	<script src="//cdnjs.cloudflare.com/ajax/libs/polymer/0.0.20130711/polymer.min.js"></script>
	```

2. Import Custom Element:

	```html
	<link rel="import" href="src/el-selectable.html">
	```

3. Start using it!

	```html
	<el-selectable></el-selectable>
	```

## Options

Attribute  			| Options                   | Default             | Description
---        			| ---                       | ---                 | ---
`selectedIndex`    | *int*                  | `undefined`               | Index of the selected item by default
`selectedClass`      			| *string*  	   | `el-selected`               | CSS class that'll be set in the item when selected.
`multi`   | *bool*                     | `undefined`               | *not yet implemented*


## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

* v0.0.1 September 14, 2013
	* Started project using [boilerplate-element](https://github.com/customelements/boilerplate-element)

## License

[MIT License](http://opensource.org/licenses/MIT)