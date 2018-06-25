# TypeScript Hello World

## What is this?

My first typescript project.
It has only one feature which shows "Hello World" on console.

## Install

```console
npm install -g typescript
npm install -g tslint
tsc --init
```

## Additional Setting

on vscode(for lint setting)
```vscode
TSLint: Create a 'tslint.json' file
```

on tsling.json(for lint setting)
```diff: tslint.json
{
    "defaultSeverity": "error",
    "extends": [
        "tslint:recommended"
-    ],
+    ],
+   "jsRules": {},
+   "rules": {},
+   "rulesDirectory": [],
+   "no-console": false,
}
```

on ./.vscode/tasks.json(for quick build)
```diff: ./.vscode/tasks.json
{
    // See https://go.microsoft.com/fwlink/?LinkId=733558
    // for the documentation about the tasks.json format
    "version": "2.0.0",
    "tasks": [
        {
            "type": "typescript",
            "tsconfig": "tsconfig.json",
            "problemMatcher": [
                "$tsc"
-           ]
+           ],
+           "isBackground": true,
+           "group": {
+               "kind": "build",
+               "isDefault": true
+           }
        }
    ]
}
```

## Usage

### Transpile

`Ctrl + Shift + B`

### Debug Execute

`F5` (same as node.js)

### Break Point

Click line heads on **not js file but ts file itself**