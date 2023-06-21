nodegui-simple-starter
======================
A [NodeGui](https://docs.nodegui.org/) application starter aiming to be fast and simple so that you can take it as a starting point and expand it to meet your needs.

The application itself is a very simple example which opens a window with some text and buttons in it. It is set up to properly support source maps for stacktraces, and also shows how to reference files elsewhere in the project.

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


Packaging
---------
`npm run package` will run [Jam Pack NodeGui](https://github.com/sedwards2009/jam-pack-nodegui) with a configuration file to create the relevant packages for the current operating system this is running on. The output appears in `tmp-jam-pack-nodegui/jam-pack-nodegui-work/`.


Configured Scripts
------------------

* `build` - Runs all of the build steps.
* `build-code` - Just run in the TypeScript compiler.
* `build-bundle` - Run `esbuild` to create the output bundle file in `dist`.
* `clean` - Deletes the temporary files in `build` and `dist`.
* `run` - Runs the application from the `dist` folder.
* `package` - Build packages for the application. The output appears in `tmp-jam-pack-nodegui/jam-pack-nodegui-work/`


Making it Yours
---------------
If you decide to use this a starting point for your own project, you will need to first update a number of configuration files which hold details of your project.

* `package.json` - The usual `name`, `description`, `author`, `license`, `repository url`, and `keywords` fields will need to be updated.
* `packaging/jam-pack-nodegui.json` - Many of the configurations for the different package types contain meta-data and package details which need updating. Also, icons will need to be replaced.
* `README.md` - This readme file will also need some heavy editing.


License
-------

MIT

Author
------

Simon Edwards <simon@simonzone.com>
