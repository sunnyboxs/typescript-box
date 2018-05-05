# typescript-box ( Support WebGL2.0 )
An enhanced version of the original typescript compiler.
Exactly the same as the tsc command！
- Support TypeScript2.9.0-dev .
- Support WebGL1.0,WebGL2.0 .
- Support Sort ts files .
- Support Visual Studio Code Ide .
- Use npm publish，Thank！
----

# How to install
`npm install -g typescript-box`


# How to use
`tsc-x`

`tsc-x --sortFiles`

`tsc-x [input files] [options]`

- Exactly the same as the tsc command.

# Options
| options        | value   |
| --------   | -----:  |
| sortFiles      | false/true   |


# How you can add to tsconfig.json
`tsconfig.json`
```javascript
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
```

# Use VSCode tsdk:
`settings.json`
```javascript
    {
        "typescript.tsdk": "C:/Users/xxxxxxx/AppData/Roaming/npm/node_modules/typescript-box/lib/"
    }
```

# Auto generate file:
`src/reference.ts`
- This saves the sorted list of dependent references.

# About：
- Welcome to use, if you have BUG also welcome feedback