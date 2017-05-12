# SASS

## Topics

* media queries
* SASS
* % vs px
* Responsive design

## SASS Installation Instructions

To add SASS install the following dependencies: `npm i --save-dev npm-run-all node-sass`

Then change your `package.json` to show these scripts:

``` 
"scripts": {
	"build-css": "node-sass src/ -o src/",
	"watch-css": "npm run build-css && node-sass src/ -o src/ --watch --recursive",
	"start-js": "react-scripts start",
	"start": "npm-run-all -p watch-css start-js",
	"build": "npm run build-css && react-scripts build",
	"test": "react-scripts test --env=jsdom",
	"eject": "react-scripts eject"
}
```

Then change your file extensions to `.scss` or `.sass` then restart your server and run `npm start` again.
