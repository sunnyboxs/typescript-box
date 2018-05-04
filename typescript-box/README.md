# typescript-box
An enhanced version of the original typescript compiler.
npm publish

# How to install
npm install -g typescript-box


# How to use
tsc-x
tsc-x --sortFiles
tsc-x [input files] [options]

# How you can add to tsconfig.json
{
	"compilerOptions": {
		"sortFiles": true,
		"target": "es5",
		"declaration": true,
		"sourceMap": true,
		"outFile": "bin/js/Main.js",
		"noImplicitAny": false,
		"removeComments": false
	},
	"exclude": [
		"node_modules",
		"bin"]
}

# Change VSCode tsdk:
settings.json
{
    "typescript.tsdk": "C:/Users/xxxxxxx/AppData/Roaming/npm/node_modules/typescript-box/lib/"
}