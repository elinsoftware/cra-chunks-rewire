# Disable code splitting in React apps based on CRA 2.0

> The following procedure disables code splitting in *CRA 2.0 based* React applications.

> This does not require `eject` or hard rewiring.

1. Copy `build-no-split.js` file to the root folder of your React application.
2. Update `package.json` with the following
```json
"build": "node build-no-split.js"
```
3. Run the following command:
```sh
npm install rewire
```
4. Build the application. There should be single files for js and css bundles, and no code splitting.
