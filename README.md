# Co-designing Accessibility in Action

[![Netlify Status](https://api.netlify.com/api/v1/badges/2243a388-75fe-4231-ae87-2fff58464956/deploy-status)](https://app.netlify.com/sites/accessibility-in-action/deploys)

This repository contains the source files for [Co-designing Accessibility in Action](https://accessibility-in-action.inclusivedesign.ca/).

## Usage

### To run locally in development mode

1. Install the required NPM packages: `npm install`
2. Run [Eleventy](http://11ty.dev) in development mode: `npm start`.

The website will be available at [http://localhost:8080](http://localhost:8080).

### To build and serve using Docker

You can build and serve the website from a [Docker](https://docs.docker.com/get-docker) container.

Once you have Docker installed, run the following commands to build a Docker image and start a container:

* Build the image: `docker build -t co-design .`
* Run the container: `docker run --name co-design -p 8000:80 co-design`

The website will be available at [http://localhost:8000](http://localhost:8000)

If you make changes to the website, repeat the steps to build the image and start a new container.

### To build for deployment to a personal web server

1. Install the required NPM packages: `npm install`
2. Run the build script: `npm run build`
3. Upload the contents of the `./dist/` directory to the web root of your server.

If you make changes to the website, repeat step 2 to build the website and upload any changed files from the `./dist/`
directory to the web root of your server.

## Features

* Integrated [UI Options](https://docs.fluidproject.org/infusion/development/UserInterfaceOptionsAPI.html) Preferences Editor.
* Basic static site configuration for developing project websites and blogs.

## Notes

Modifications can be made to any source file or directory except for the contents of the `./dist/` directory. The
`./dist/` directory is not versioned since it contains the built website that Eleventy generates from the source files,
and  files in `dist` are overwritten at build time.

## License

This website's source code is available under the [New BSD License](https://raw.githubusercontent.com/fluid-project/trivet/master/LICENSE.md).

## Third Party Software in Trivet

Trivet is based on other publicly available software, categorized by license:

### MIT License

* [Eleventastic](https://github.com/maxboeck/eleventastic)
* [eleventy-webpack](https://github.com/clenemt/eleventy-webpack)
* [Hylia](https://github.com/hankchizljaw/hylia)
* [Supermaya](https://github.com/MadeByMike/supermaya)
