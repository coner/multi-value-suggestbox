# &lt;multi-value-suggestbox&gt;

A Polymer custom element that allows selection of multiple suggestions

## Demo

[Check it live!](http://coner.github.io/multi-value-suggestbox)

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install multi-value-suggestbox --save
```

Or [download as ZIP](https://github.com/my-user/my-repo/archive/master.zip).

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="bower_components/platform/platform.js"></script>
    ```

2. Import Custom Element:

    ```html
    <link rel="import" href="bower_components/multi-value-suggestbox/dist/multi-value-suggestbox.html">
    ```

3. Start using it!

    ```html
    <multi-value-suggestbox></multi-value-suggestbox>
    ```

## Options

Attribute                   | Options     | Default   | Description
---                         | ---         | ---       | ---
`options.box_width`         | *string*    | `200px`   | Width of the input box
`options.box_width`         | *string*    | `40px`    | Height of the input box
`options.allow_space`       | *bool*      | `false`   | Whether spaces are accepted
`options.allow_nonmatching` | *bool*      | `false`   | Whether non-suggested values are accepted

## Methods

Method               | Parameters   | Returns     | Description
---                  | ---          | ---         | ---
`resetSuggestions()` | None.        | Nothing.    | Removes all suggestions currently displayed in the menu.

## Events

Event           | Description
---             | ---
`input-changed` | Triggers whenever the value in the text input box is changed by user.

## Fields

Attribute             | Options    | Description
---                   | ---        | ---
`suggestions`         | *array*    | Suggestions currently displayed
`selectedItems`       | *array*    | Items selected or entered by user

## Development

In order to run it locally you'll need to fetch some dependencies and a basic server setup.

* Install [Bower](http://bower.io/) & [Grunt](http://gruntjs.com/):

    ```sh
    $ [sudo] npm install -g bower grunt-cli
    ```

* Install local dependencies:

    ```sh
    $ bower install && npm install
    ```

* To test your project, start the development server and open `http://localhost:8000`.

    ```sh
    $ grunt server
    ```

* To build the distribution files before releasing a new version.

    ```sh
    $ grunt build
    ```

* To provide a live demo, send everything to `gh-pages` branch.

    ```sh
    $ grunt deploy
    ```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

For detailed changelog, check [Releases](https://github.com/my-user/multi-value-suggestbox/releases).

## License

[BSD License](http://opensource.org/licenses/BSD-3-Clause)
