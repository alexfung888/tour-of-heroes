Angular.io quickstart and tutorial
config copied from web, so no CLI 
package.json defined npm scripts to launch tsc in watch mode 
and lite server, which listens on port 3000
compiles TS to .
to work with VSCode, I made the following customistaions to launch.json:
            "url": "http://localhost:3000/", 
            // instead of 4200
            "sourceMaps": true,
            "webRoot": "${workspaceRoot}/app",
            "sourceMapPathOverrides": {
                "webpack:///C:*":"C:/*"
            },
            "userDataDir": "${workspaceRoot}/.vscode/chrome",
            "runtimeArgs": [
                "--disable-session-crashed-bubble",
                "--disable-infobars"
            ]

