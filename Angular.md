## error TS7006: Parameter 'user' implicitly has an 'any' type.

### fix: Change / method parrameter value to Any

onSubmit(user:any) {
console.log(user)
}

## CommonJs bundle size warning

### fix: Add “type”: “module” to your package.json

1. Open Your package.json file.
2. Just add the top-level "type" field with a value of "module"
3. This will ensure that all .js and .mjs files are interpreted as ES modules.
4. You can interpret individual files as CommonJS by using the .cjs extension.
5. add "type": "module" in the upper level as show below:// package.json

`{
"name": "my-project",
"version": "0.0.0",
"type": "module",
"scripts": { ...
},
...
}`

ref: https://exerror.com/syntaxerror-cannot-use-import-statement-outside-a-module-in-nodejs/