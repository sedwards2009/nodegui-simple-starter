# nodegui-simple-starter
A [NodeGui](https://docs.nodegui.org/) application starter aiming to be fast and simple so that you can take it as a starting point and expand it to meet your needs.

The application itself is a very simple example which opens a window with some text and buttons in it. It is set up to probably support source maps for stacktraces, and also shows how to reference files elsewhere in the project.

This project can work with either `npm` or `yarn`.


Set up
------

Run `npm install` to download and install the dependencies.

Building
--------
`npm run build` will build the code in `src` and produce a bundle file in `dist`. It first runs the TypeScript compiler which puts its output in the `build` folder. Then `esbuild` is run to bundle the contents of `build` and out to `dist`.


Running
-------
`npm run run` will run the bundled application. Note, you will have to build it first.


Configured Scripts
------------------

* `build` - Runs all of the build steps.
* `build-code` - Just run in the TypeScript compiler.
* `build-bundle` - Run `esbuild` to create the output bundle file in `dist`.
* `clean` - Deletes the temporary files in `build` and `dist`.
* `run` - Runs the application from the `dist` folder.

License
-------

MIT

Author
------

Simon Edwards <simon@simonzone.com>
